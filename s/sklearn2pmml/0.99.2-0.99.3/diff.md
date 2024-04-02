# Comparing `tmp/sklearn2pmml-0.99.2.tar.gz` & `tmp/sklearn2pmml-0.99.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sklearn2pmml-0.99.2.tar", last modified: Wed Nov  1 05:43:51 2023, max compression
+gzip compressed data, was "dist/sklearn2pmml-0.99.3.tar", last modified: Mon Dec  4 20:31:33 2023, max compression
```

## Comparing `sklearn2pmml-0.99.2.tar` & `sklearn2pmml-0.99.3.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-11-01 05:43:51.000000 sklearn2pmml-0.99.2/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)       40 2018-03-12 15:29:56.000000 sklearn2pmml-0.99.2/setup.cfg
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    34520 2018-03-12 15:29:56.000000 sklearn2pmml-0.99.2/LICENSE.txt
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1437 2023-09-19 08:17:23.000000 sklearn2pmml-0.99.2/setup.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      739 2023-11-01 05:43:51.000000 sklearn2pmml-0.99.2/PKG-INFO
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-11-01 05:43:51.000000 sklearn2pmml-0.99.2/sklearn2pmml/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      840 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.2/sklearn2pmml/h2o.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-11-01 05:43:51.000000 sklearn2pmml-0.99.2/sklearn2pmml/ruleset/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      888 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.2/sklearn2pmml/ruleset/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-11-01 05:43:51.000000 sklearn2pmml-0.99.2/sklearn2pmml/pipeline/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     6005 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.2/sklearn2pmml/pipeline/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      769 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.2/sklearn2pmml/tpot.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    12759 2023-08-24 14:43:27.000000 sklearn2pmml-0.99.2/sklearn2pmml/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-11-01 05:43:51.000000 sklearn2pmml-0.99.2/sklearn2pmml/decoration/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    16924 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.2/sklearn2pmml/decoration/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-11-01 05:43:51.000000 sklearn2pmml-0.99.2/sklearn2pmml/neural_network/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      777 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.2/sklearn2pmml/neural_network/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      640 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.2/sklearn2pmml/pycaret.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-11-01 05:43:51.000000 sklearn2pmml-0.99.2/sklearn2pmml/util/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7471 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.2/sklearn2pmml/util/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1108 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.2/sklearn2pmml/xgboost.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-11-01 05:43:51.000000 sklearn2pmml-0.99.2/sklearn2pmml/feature_extraction/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2018-03-12 15:29:56.000000 sklearn2pmml-0.99.2/sklearn2pmml/feature_extraction/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-11-01 05:43:51.000000 sklearn2pmml-0.99.2/sklearn2pmml/feature_extraction/text/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1123 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.2/sklearn2pmml/feature_extraction/text/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-11-01 05:43:51.000000 sklearn2pmml-0.99.2/sklearn2pmml/ensemble/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    11176 2023-09-23 13:28:12.000000 sklearn2pmml-0.99.2/sklearn2pmml/ensemble/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     4533 2023-08-24 14:43:27.000000 sklearn2pmml-0.99.2/sklearn2pmml/statsmodels.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-11-01 05:43:51.000000 sklearn2pmml-0.99.2/sklearn2pmml/feature_selection/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      846 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.2/sklearn2pmml/feature_selection/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-11-01 05:43:51.000000 sklearn2pmml-0.99.2/sklearn2pmml/cross_reference/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     2417 2023-10-27 19:00:33.000000 sklearn2pmml-0.99.2/sklearn2pmml/cross_reference/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-11-01 05:43:51.000000 sklearn2pmml-0.99.2/sklearn2pmml/postprocessing/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1740 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.2/sklearn2pmml/postprocessing/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-11-01 05:43:51.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1300 2020-10-11 20:49:33.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)  3041245 2023-07-18 12:18:27.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/guava-32.1.1-jre.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   139727 2021-10-23 18:57:27.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/jaxb-core-3.0.2.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   496728 2023-10-23 19:44:49.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/pmml-sklearn-1.7.41.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     8815 2023-10-23 19:44:50.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.41.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      297 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    41125 2022-02-16 09:19:19.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/slf4j-api-1.7.36.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    51724 2023-07-22 06:57:40.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/pmml-h2o-1.2.9.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    75714 2022-07-22 17:55:51.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/jackson-annotations-2.13.3.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    69254 2018-02-17 21:50:20.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/jcommander-1.72.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   198931 2023-07-20 20:18:17.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/pmml-converter-1.5.5.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    68200 2023-07-21 08:53:01.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/pmml-lightgbm-1.4.6.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    88591 2023-10-23 19:44:50.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/pmml-sklearn-extension-1.7.41.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)  1138813 2022-08-01 13:09:48.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/pmml-model-1.6.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     4526 2023-10-23 19:38:03.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/h2o-logger-3.44.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     2235 2022-05-06 18:22:34.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/ubjson-gson-0.1.8.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     4708 2022-08-01 13:10:01.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    39662 2022-05-06 18:22:34.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/ubjson-0.1.8.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   283367 2023-07-21 09:00:16.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/gson-2.10.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   466064 2023-10-23 19:38:03.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/h2o-genmodel-3.44.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      818 2023-10-23 19:52:40.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/classpath.txt
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     8467 2023-10-23 19:44:50.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.41.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     4885 2023-10-23 19:52:42.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   209112 2023-07-21 07:47:54.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/pmml-python-1.1.17.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     6418 2023-10-23 19:44:50.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.41.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     8436 2022-02-16 09:19:19.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   913701 2021-10-23 18:57:29.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    44790 2021-06-01 08:00:08.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/serpent-1.40.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    29896 2021-10-23 18:57:27.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    62154 2021-10-23 18:57:27.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/jakarta.activation-2.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   128941 2021-10-23 18:57:27.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    30899 2023-07-21 19:03:56.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/pmml-statsmodels-1.0.5.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    54294 2023-06-11 07:47:11.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/pickle-1.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    72620 2023-07-21 09:07:53.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/pmml-xgboost-1.7.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7607 2023-10-23 19:44:50.000000 sklearn2pmml-0.99.2/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.41.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      144 2023-11-01 05:42:46.000000 sklearn2pmml-0.99.2/sklearn2pmml/metadata.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-11-01 05:43:51.000000 sklearn2pmml-0.99.2/sklearn2pmml/preprocessing/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      880 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.2/sklearn2pmml/preprocessing/h2o.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    18969 2023-11-01 05:28:13.000000 sklearn2pmml-0.99.2/sklearn2pmml/preprocessing/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1724 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.2/sklearn2pmml/preprocessing/xgboost.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1868 2023-09-20 06:52:47.000000 sklearn2pmml-0.99.2/sklearn2pmml/preprocessing/lightgbm.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-11-01 05:43:51.000000 sklearn2pmml-0.99.2/sklearn2pmml/tree/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1941 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.2/sklearn2pmml/tree/chaid.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.2/sklearn2pmml/tree/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-11-01 05:43:51.000000 sklearn2pmml-0.99.2/sklearn2pmml/expression/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     2944 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.2/sklearn2pmml/expression/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-12-04 20:31:33.000000 sklearn2pmml-0.99.3/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)       40 2018-03-12 15:29:56.000000 sklearn2pmml-0.99.3/setup.cfg
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    34520 2018-03-12 15:29:56.000000 sklearn2pmml-0.99.3/LICENSE.txt
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1437 2023-09-19 08:17:23.000000 sklearn2pmml-0.99.3/setup.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      739 2023-12-04 20:31:33.000000 sklearn2pmml-0.99.3/PKG-INFO
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-12-04 20:31:33.000000 sklearn2pmml-0.99.3/sklearn2pmml/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      840 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.3/sklearn2pmml/h2o.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-12-04 20:31:33.000000 sklearn2pmml-0.99.3/sklearn2pmml/ruleset/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      888 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.3/sklearn2pmml/ruleset/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-12-04 20:31:33.000000 sklearn2pmml-0.99.3/sklearn2pmml/pipeline/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     6005 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.3/sklearn2pmml/pipeline/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      769 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.3/sklearn2pmml/tpot.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    12759 2023-08-24 14:43:27.000000 sklearn2pmml-0.99.3/sklearn2pmml/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-12-04 20:31:33.000000 sklearn2pmml-0.99.3/sklearn2pmml/decoration/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    16700 2023-12-03 20:29:38.000000 sklearn2pmml-0.99.3/sklearn2pmml/decoration/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-12-04 20:31:33.000000 sklearn2pmml-0.99.3/sklearn2pmml/neural_network/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      777 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.3/sklearn2pmml/neural_network/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      640 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.3/sklearn2pmml/pycaret.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-12-04 20:31:33.000000 sklearn2pmml-0.99.3/sklearn2pmml/util/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7561 2023-12-04 08:48:26.000000 sklearn2pmml-0.99.3/sklearn2pmml/util/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1108 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.3/sklearn2pmml/xgboost.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-12-04 20:31:33.000000 sklearn2pmml-0.99.3/sklearn2pmml/feature_extraction/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2018-03-12 15:29:56.000000 sklearn2pmml-0.99.3/sklearn2pmml/feature_extraction/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-12-04 20:31:33.000000 sklearn2pmml-0.99.3/sklearn2pmml/feature_extraction/text/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1123 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.3/sklearn2pmml/feature_extraction/text/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-12-04 20:31:33.000000 sklearn2pmml-0.99.3/sklearn2pmml/ensemble/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    11546 2023-12-04 19:48:45.000000 sklearn2pmml-0.99.3/sklearn2pmml/ensemble/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4533 2023-08-24 14:43:27.000000 sklearn2pmml-0.99.3/sklearn2pmml/statsmodels.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-12-04 20:31:33.000000 sklearn2pmml-0.99.3/sklearn2pmml/feature_selection/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      846 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.3/sklearn2pmml/feature_selection/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-12-04 20:31:33.000000 sklearn2pmml-0.99.3/sklearn2pmml/cross_reference/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     3151 2023-11-19 10:34:49.000000 sklearn2pmml-0.99.3/sklearn2pmml/cross_reference/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-12-04 20:31:33.000000 sklearn2pmml-0.99.3/sklearn2pmml/postprocessing/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1740 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.3/sklearn2pmml/postprocessing/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-12-04 20:31:33.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1300 2020-10-11 20:49:33.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)  3041245 2023-07-18 12:18:27.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/guava-32.1.1-jre.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   139727 2021-10-23 18:57:27.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/jaxb-core-3.0.2.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4526 2023-12-03 10:07:33.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/h2o-logger-3.44.0.2.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      297 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    41125 2022-02-16 09:19:19.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/slf4j-api-1.7.36.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    51724 2023-07-22 06:57:40.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/pmml-h2o-1.2.9.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    75714 2022-07-22 17:55:51.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/jackson-annotations-2.13.3.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    69254 2018-02-17 21:50:20.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/jcommander-1.72.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   198931 2023-07-20 20:18:17.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/pmml-converter-1.5.5.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7606 2023-12-04 20:17:24.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.42.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    68200 2023-07-21 08:53:01.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/pmml-lightgbm-1.4.6.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)  1138813 2022-08-01 13:09:48.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/pmml-model-1.6.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     2235 2022-05-06 18:22:34.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/ubjson-gson-0.1.8.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4708 2022-08-01 13:10:01.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    39662 2022-05-06 18:22:34.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/ubjson-0.1.8.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   283367 2023-07-21 09:00:16.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/gson-2.10.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   500181 2023-12-04 20:17:22.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/pmml-sklearn-1.7.42.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     6416 2023-12-04 20:17:24.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.42.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      818 2023-12-04 20:28:11.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/classpath.txt
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4886 2023-12-04 20:28:12.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     8465 2023-12-04 20:17:24.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.42.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    88622 2023-12-04 20:17:23.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/pmml-sklearn-extension-1.7.42.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    54836 2023-12-02 14:08:45.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/pickle-1.5.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     8436 2022-02-16 09:19:19.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   913701 2021-10-23 18:57:29.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    44790 2021-06-01 08:00:08.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/serpent-1.40.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    29896 2021-10-23 18:57:27.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     8812 2023-12-04 20:17:23.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.42.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    62154 2021-10-23 18:57:27.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/jakarta.activation-2.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   128941 2021-10-23 18:57:27.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   466825 2023-12-03 10:07:33.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/h2o-genmodel-3.44.0.2.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   210028 2023-12-03 13:42:28.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/pmml-python-1.1.18.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    30899 2023-07-21 19:03:56.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/pmml-statsmodels-1.0.5.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    72620 2023-07-21 09:07:53.000000 sklearn2pmml-0.99.3/sklearn2pmml/resources/pmml-xgboost-1.7.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      144 2023-12-04 20:27:24.000000 sklearn2pmml-0.99.3/sklearn2pmml/metadata.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-12-04 20:31:33.000000 sklearn2pmml-0.99.3/sklearn2pmml/preprocessing/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      880 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.3/sklearn2pmml/preprocessing/h2o.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    19175 2023-12-04 19:48:45.000000 sklearn2pmml-0.99.3/sklearn2pmml/preprocessing/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1724 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.3/sklearn2pmml/preprocessing/xgboost.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1868 2023-09-20 06:52:47.000000 sklearn2pmml-0.99.3/sklearn2pmml/preprocessing/lightgbm.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-12-04 20:31:33.000000 sklearn2pmml-0.99.3/sklearn2pmml/tree/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1941 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.3/sklearn2pmml/tree/chaid.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.3/sklearn2pmml/tree/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-12-04 20:31:33.000000 sklearn2pmml-0.99.3/sklearn2pmml/expression/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     2944 2023-06-02 16:05:54.000000 sklearn2pmml-0.99.3/sklearn2pmml/expression/__init__.py
```

### Comparing `sklearn2pmml-0.99.2/LICENSE.txt` & `sklearn2pmml-0.99.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/setup.py` & `sklearn2pmml-0.99.3/setup.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/h2o.py` & `sklearn2pmml-0.99.3/sklearn2pmml/h2o.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/ruleset/__init__.py` & `sklearn2pmml-0.99.3/sklearn2pmml/ruleset/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/pipeline/__init__.py` & `sklearn2pmml-0.99.3/sklearn2pmml/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/tpot.py` & `sklearn2pmml-0.99.3/sklearn2pmml/tpot.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/__init__.py` & `sklearn2pmml-0.99.3/sklearn2pmml/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/decoration/__init__.py` & `sklearn2pmml-0.99.3/sklearn2pmml/decoration/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -222,16 +222,15 @@
 			if (low_value is None) or (high_value is None):
 				raise ValueError("Outlier treatment {0} requires low_value and high_value attributes".format(outlier_treatment))
 		self.low_value = low_value
 		self.high_value = high_value
 
 	def _valid_value_mask(self, X, where):
 		if hasattr(self, "data_min_") and hasattr(self, "data_max_"):
-			mask = (numpy.greater_equal(X, self.data_min_, where = where) & numpy.less_equal(X, self.data_max_, where = where))
-			return numpy.logical_and(mask, where)
+			return numpy.where((X >= self.data_min_) & (X <= self.data_max_), where, False)
 		return super(ContinuousDomain, self)._valid_value_mask(X, where)
 
 	def fit(self, X, y = None):
 		if self._empty_fit():
 			return self
 		if self.dtype is not None:
 			X = cast(X, self.dtype)
@@ -253,24 +252,21 @@
 				"standardDeviation" : numpy.asarray(numpy.nanstd(X, axis = 0)),
 				"median" : numpy.asarray(numpy.nanmedian(X, axis = 0)),
 				"interQuartileRange" : numpy.asarray(_interquartile_range(X, axis = 0))
 			}
 		return self
 
 	def _outlier_mask(self, X, where):
-		mask = (numpy.less(X, self.low_value, where = where) | numpy.greater(X, self.high_value, where = where))
-		return numpy.logical_and(mask, where)
+		return numpy.where((X < self.low_value) | (X > self.high_value), where, False)
 
 	def _negative_outlier_mask(self, X, where):
-		mask = numpy.less(X, self.low_value, where = where)
-		return numpy.logical_and(mask, where)
+		return numpy.where(X < self.low_value, where, False)
 
 	def _positive_outlier_mask(self, X, where):
-		mask = numpy.greater(X, self.high_value, where = where)
-		return numpy.logical_and(mask, where)
+		return numpy.where(X > self.high_value, where, False)
 
 	def _transform_valid_values(self, X, where):
 		if self.outlier_treatment == "as_missing_values":
 			mask = self._outlier_mask(X, where)
 			if self.missing_values is not None:
 				if type(self.missing_values) is list:
 					raise ValueError()
```

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/neural_network/__init__.py` & `sklearn2pmml-0.99.3/sklearn2pmml/neural_network/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/pycaret.py` & `sklearn2pmml-0.99.3/sklearn2pmml/pycaret.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/util/__init__.py` & `sklearn2pmml-0.99.3/sklearn2pmml/util/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,23 @@
 
 import inspect
 import numpy
 import pandas
 import sys
 import types
 
+try:
+	# Pandas 2.X
+	iso8601_format = "ISO8601"
+
+	pandas.to_datetime("2023-12-03", format = iso8601_format)
+except ValueError:
+	# Pandas 1.X
+	iso8601_format = "%Y-%m-%dT%H:%M:%S.%f"
+
 def cast(X, dtype):
 	if isinstance(dtype, str) and dtype.startswith("datetime64"):
 		func = lambda x: to_pydatetime(x, dtype)
 		return dt_transform(X, func)
 	else:
 		if not hasattr(X, "astype"):
 			X = numpy.asarray(X)
@@ -53,15 +62,15 @@
 	if isinstance(Xt, Index):
 		Xt = Xt.values
 	if len(shape) > 1:
 		Xt = Xt.reshape(shape)
 	return Xt
 
 def to_pydatetime(X, dtype):
-	Xt = pandas.to_datetime(X, yearfirst = True, origin = "unix")
+	Xt = pandas.to_datetime(X, yearfirst = True, format = iso8601_format, origin = "unix")
 	if hasattr(Xt, "dt"):
 		Xt = Xt.dt
 	if dtype == "datetime64[D]":
 		Xt = Xt.floor("D")
 	elif dtype == "datetime64[s]":
 		Xt = Xt.floor("S")
 	else:
@@ -145,19 +154,19 @@
 	# Import modules
 	for module in modules:
 		exec("import {}".format(module), env)
 
 	if isinstance(expr, str):
 		if "\n" not in expr:
 
-			def _eval_row(x):
+			def evaluate(x):
 				env["X"] = x
 				return eval(expr, env)
 
-			return _eval_row
+			return evaluate
 		else:
 			func = ensure_def(expr, env)
 			return lambda x: func(x)
 	elif isinstance(expr, Evaluatable):
 		expr.setup(env = env)
 		return lambda x: expr.evaluate(x, env)
 	else:
@@ -170,18 +179,14 @@
 		return X.apply(func, axis = 1)
 	nrow = X.shape[0]
 	Xt = numpy.empty(shape = (nrow, ), dtype = dtype)
 	for i in range(0, nrow):
 		Xt[i] = func(X[i])
 	return Xt
 
-def eval_expr_rows(X, expr, dtype = object):
-	func = to_expr_func(expr)
-	return eval_rows(X, func, dtype = dtype)
-
 def fqn(obj):
 	clazz = obj if inspect.isclass(obj) else obj.__class__
 	return ".".join([clazz.__module__, clazz.__name__])
 
 def is_instance_attr(obj, name):
 	if not hasattr(obj, name):
 		return False
```

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/xgboost.py` & `sklearn2pmml-0.99.3/sklearn2pmml/xgboost.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/feature_extraction/text/__init__.py` & `sklearn2pmml-0.99.3/sklearn2pmml/feature_extraction/text/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/ensemble/__init__.py` & `sklearn2pmml-0.99.3/sklearn2pmml/ensemble/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 	from sklearn.linear_model import LinearRegression
 	from sklearn.linear_model._base import LinearClassifierMixin, LinearModel, SparseCoefMixin
 except ImportError:
 	from sklearn.linear_model.base import LinearClassifierMixin, LinearModel, LinearRegression, SparseCoefMixin
 from sklearn.preprocessing import OneHotEncoder
 from sklearn.utils.metaestimators import _BaseComposition
 from sklearn2pmml import _is_ordinal
-from sklearn2pmml.util import eval_expr_rows, fqn, Predicate
+from sklearn2pmml.util import eval_rows, fqn, to_expr_func, Predicate
 
 import copy
 import numpy
 
 def _checkGBDTRegressor(gbdt):
 	if hasattr(gbdt, "apply"):
 		return gbdt
@@ -273,15 +273,16 @@
 		if len(y.shape) > 1:
 			if len(self.steps) != y.shape[1]:
 				raise ValueError()
 			y = numpy.asarray(y)
 		X_eval = self._to_evaluation_dataset(X)
 		i = 0
 		for name, estimator, predicate in self.steps:
-			step_mask = eval_expr_rows(X_eval, predicate, dtype = bool)
+			step_mask_func = to_expr_func(predicate)
+			step_mask = eval_rows(X_eval, step_mask_func, dtype = bool)
 			if numpy.sum(step_mask) < 1:
 				raise ValueError(predicate)
 			step_X = X[step_mask]
 			if len(y.shape) == 1:
 				step_y = y[step_mask]
 			elif len(y.shape) == 2:
 				step_y = y[step_mask, i]
@@ -294,15 +295,16 @@
 			i += 1
 		return self
 
 	def _predict(self, X, predict_method):
 		result = None
 		X_eval = self._to_evaluation_dataset(X)
 		for name, estimator, predicate in self.steps:
-			step_mask = eval_expr_rows(X_eval, predicate, dtype = bool)
+			step_mask_func = to_expr_func(predicate)
+			step_mask = eval_rows(X_eval, step_mask_func, dtype = bool)
 			if numpy.sum(step_mask) < 1:
 				continue
 			step_X = X[step_mask]
 			step_result = getattr(estimator, predict_method)(step_X)
 			step_result = _to_sparse(X, step_mask, step_result)
 			if self.multioutput:
 				step_result = step_result.reshape(X.shape[0], -1)
@@ -323,38 +325,46 @@
 		return self._predict(X, "predict")
 
 	def predict_proba(self, X):
 		return self._predict(X, "predict_proba")
 
 class SelectFirstEstimator(_BaseEnsemble):
 
-	def __init__(self, steps, controller):
+	def __init__(self, steps, controller, eval_rows):
 		super(SelectFirstEstimator, self).__init__(steps, controller)
+		self.eval_rows = eval_rows
+
+	def _eval_step_mask(self, X, predicate):
+		step_func = to_expr_func(predicate)
+		if self.eval_rows:
+			return eval_rows(X, step_func, dtype = bool)
+		else:
+			return step_func(X)
 
 	def fit(self, X, y, **fit_params):
 		X_eval = self._to_evaluation_dataset(X)
-		mask = numpy.zeros(X.shape[0], dtype = bool)
+		mask = numpy.full(X.shape[0], fill_value = False)
 		for name, estimator, predicate in self.steps:
-			step_mask = eval_expr_rows(X_eval, predicate, dtype = bool)
+			step_mask = self._eval_step_mask(X_eval, predicate)
 			step_mask[mask] = False
 			if numpy.sum(step_mask) < 1:
 				raise ValueError(predicate)
 			step_X = X[step_mask]
 			step_y = y[step_mask]
 			step_fit_params = _mask_params(_extract_step_params(name, fit_params), step_mask)
 			estimator.fit(step_X, step_y, **step_fit_params)
 			mask = numpy.logical_or(mask, step_mask)
 		return self
 
 	def _predict(self, X, predict_method):
 		result = None
 		X_eval = self._to_evaluation_dataset(X)
-		mask = numpy.zeros(X.shape[0], dtype = bool)
+		mask = numpy.full(X.shape[0], fill_value = False)
 		for name, estimator, predicate in self.steps:
-			step_mask = eval_expr_rows(X_eval, predicate, dtype = bool)
+			step_mask = self._eval_step_mask(X_eval, predicate)
 			step_mask[mask] = False
 			if numpy.sum(step_mask) < 1:
 				continue
 			step_X = X[step_mask]
 			step_result = getattr(estimator, predict_method)(step_X)
 			step_result = _to_sparse(X, step_mask, step_result)
 			if result is None:
@@ -368,17 +378,17 @@
 		return self._predict(X, "apply")
 
 	def predict(self, X):
 		return self._predict(X, "predict")
 
 class SelectFirstRegressor(SelectFirstEstimator, RegressorMixin):
 
-	def __init__(self, steps, controller = None):
-		super(SelectFirstRegressor, self).__init__(steps, controller)
+	def __init__(self, steps, controller = None, eval_rows = True):
+		super(SelectFirstRegressor, self).__init__(steps, controller, eval_rows)
 
 class SelectFirstClassifier(SelectFirstEstimator, ClassifierMixin):
 
-	def __init__(self, steps, controller = None):
-		super(SelectFirstClassifier, self).__init__(steps, controller)
+	def __init__(self, steps, controller = None, eval_rows = True):
+		super(SelectFirstClassifier, self).__init__(steps, controller, eval_rows)
 
 	def predict_proba(self, X):
 		return self._predict(X, "predict_proba")
```

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/statsmodels.py` & `sklearn2pmml-0.99.3/sklearn2pmml/statsmodels.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/feature_selection/__init__.py` & `sklearn2pmml-0.99.3/sklearn2pmml/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/postprocessing/__init__.py` & `sklearn2pmml-0.99.3/sklearn2pmml/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/guava-32.1.1-jre.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/guava-32.1.1-jre.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/jaxb-core-3.0.2.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/jaxb-core-3.0.2.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/pmml-sklearn-1.7.41.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/pmml-sklearn-1.7.42.jar`

 * *Files 7% similar despite different names*

#### zipinfo {}

```diff
@@ -1,429 +1,432 @@
-Zip file size: 496728 bytes, number of entries: 427
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 META-INF/
--rw-r--r--  2.0 unx      159 b- defN 23-Oct-23 22:44 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn_pandas/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 chaid/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 stop_words/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/calibration/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/pipeline/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/dummy/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/svm/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/neural_network/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/impute/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/naive_bayes/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/linear_model/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/linear_model/logistic/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/linear_model/ridge/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/linear_model/glm/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/linear_model/stochastic_gradient/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/compose/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/model_selection/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/decomposition/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/neighbors/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/multioutput/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/isotonic/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/feature_extraction/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/feature_extraction/text/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/metrics/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/ensemble/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/ensemble/bagging/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/ensemble/stacking/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/ensemble/gradient_boosting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/ensemble/forest/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/ensemble/iforest/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/ensemble/voting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/ensemble/hist_gradient_boosting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/ensemble/weight_boosting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/feature_selection/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/loss/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/discriminant_analysis/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/preprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/tree/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/tree/visitors/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/cluster/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn/multiclass/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn2pmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn2pmml/ruleset/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn2pmml/pipeline/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn2pmml/decoration/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn2pmml/neural_network/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn2pmml/util/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn2pmml/feature_extraction/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn2pmml/feature_extraction/text/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn2pmml/ensemble/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn2pmml/feature_selection/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn2pmml/cross_reference/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn2pmml/postprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn2pmml/preprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn2pmml/tree/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn2pmml/expression/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 org/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 org/jpmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 org/jpmml/sklearn/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 org/jpmml/sklearn/testing/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 META-INF/maven/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 META-INF/maven/org.jpmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 META-INF/maven/org.jpmml/pmml-sklearn/
--rw-rw-r--  2.0 unx    17154 b- defN 23-Oct-23 22:44 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx     2287 b- defN 23-Oct-23 22:44 sklearn_pandas/CategoricalImputer.class
--rw-rw-r--  2.0 unx      656 b- defN 23-Oct-23 22:44 sklearn_pandas/TransformerPipeline.class
--rw-rw-r--  2.0 unx     1154 b- defN 23-Oct-23 22:44 sklearn_pandas/DataFrameMapper$2.class
--rw-rw-r--  2.0 unx     6280 b- defN 23-Oct-23 22:44 sklearn_pandas/DataFrameMapper.class
--rw-rw-r--  2.0 unx     1126 b- defN 23-Oct-23 22:44 sklearn_pandas/DataFrameMapper$1.class
--rw-rw-r--  2.0 unx      609 b- defN 23-Oct-23 22:44 chaid/ContinuousColumn.class
--rw-rw-r--  2.0 unx      925 b- defN 23-Oct-23 22:44 chaid/Node.class
--rw-rw-r--  2.0 unx      467 b- defN 23-Oct-23 22:44 chaid/Column.class
--rw-rw-r--  2.0 unx     3283 b- defN 23-Oct-23 22:44 chaid/Split.class
--rw-rw-r--  2.0 unx      401 b- defN 23-Oct-23 22:44 chaid/InvalidSplitReason.class
--rw-rw-r--  2.0 unx      602 b- defN 23-Oct-23 22:44 chaid/NominalColumn.class
--rw-rw-r--  2.0 unx     1912 b- defN 23-Oct-23 22:44 stop_words/english.txt
--rw-rw-r--  2.0 unx      140 b- defN 23-Oct-23 22:44 sklearn/HasHead.class
--rw-rw-r--  2.0 unx     1959 b- defN 23-Oct-23 22:44 sklearn/StepUtil.class
--rw-rw-r--  2.0 unx    12886 b- defN 23-Oct-23 22:44 sklearn/calibration/CalibratedClassifier.class
--rw-rw-r--  2.0 unx     2953 b- defN 23-Oct-23 22:44 sklearn/calibration/SigmoidCalibration.class
--rw-rw-r--  2.0 unx      683 b- defN 23-Oct-23 22:44 sklearn/calibration/CalibratedClassifier$1.class
--rw-rw-r--  2.0 unx     3676 b- defN 23-Oct-23 22:44 sklearn/calibration/CalibratedClassifierCV.class
--rw-rw-r--  2.0 unx     2216 b- defN 23-Oct-23 22:44 sklearn/VersionUtil.class
--rw-rw-r--  2.0 unx     2818 b- defN 23-Oct-23 22:44 sklearn/pipeline/FeatureUnion.class
--rw-rw-r--  2.0 unx     1670 b- defN 23-Oct-23 22:44 sklearn/pipeline/SkLearnPipeline$3.class
--rw-rw-r--  2.0 unx     5196 b- defN 23-Oct-23 22:44 sklearn/pipeline/SkLearnPipeline.class
--rw-rw-r--  2.0 unx     1709 b- defN 23-Oct-23 22:44 sklearn/pipeline/SkLearnPipeline$2.class
--rw-rw-r--  2.0 unx     1772 b- defN 23-Oct-23 22:44 sklearn/pipeline/SkLearnPipeline$1.class
--rw-rw-r--  2.0 unx      682 b- defN 23-Oct-23 22:44 sklearn/SkLearnClassifier.class
--rw-rw-r--  2.0 unx     5031 b- defN 23-Oct-23 22:44 sklearn/dummy/DummyClassifier.class
--rw-rw-r--  2.0 unx     2181 b- defN 23-Oct-23 22:44 sklearn/dummy/DummyRegressor.class
--rw-rw-r--  2.0 unx      512 b- defN 23-Oct-23 22:44 sklearn/SkLearnFields.class
--rw-rw-r--  2.0 unx     2293 b- defN 23-Oct-23 22:44 sklearn/SkLearnOutlierTransformation.class
--rw-rw-r--  2.0 unx      240 b- defN 23-Oct-23 22:44 sklearn/HasEstimator.class
--rw-rw-r--  2.0 unx     3421 b- defN 23-Oct-23 22:44 sklearn/OutlierDetectorUtil.class
--rw-rw-r--  2.0 unx     1236 b- defN 23-Oct-23 22:44 sklearn/HasMultiApplyField.class
--rw-rw-r--  2.0 unx      591 b- defN 23-Oct-23 22:44 sklearn/HasMultiDecisionFunctionField.class
--rw-rw-r--  2.0 unx     2393 b- defN 23-Oct-23 22:44 sklearn/svm/SupportVectorMachineUtil.class
--rw-rw-r--  2.0 unx     1109 b- defN 23-Oct-23 22:44 sklearn/svm/LinearSVC.class
--rw-rw-r--  2.0 unx     5044 b- defN 23-Oct-23 22:44 sklearn/svm/LibSVMClassifier.class
--rw-rw-r--  2.0 unx      966 b- defN 23-Oct-23 22:44 sklearn/svm/SupportVectorMachineUtil$1.class
--rw-rw-r--  2.0 unx     1869 b- defN 23-Oct-23 22:44 sklearn/svm/OneClassSVM.class
--rw-rw-r--  2.0 unx     3601 b- defN 23-Oct-23 22:44 sklearn/svm/LibSVMRegressor.class
--rw-rw-r--  2.0 unx      678 b- defN 23-Oct-23 22:44 sklearn/SkLearnClusterer.class
--rw-rw-r--  2.0 unx     2584 b- defN 23-Oct-23 22:44 sklearn/InitializerUtil$1.class
--rw-rw-r--  2.0 unx      342 b- defN 23-Oct-23 22:44 sklearn/HasOutlierField.class
--rw-rw-r--  2.0 unx      214 b- defN 23-Oct-23 22:44 sklearn/HasNumberOfFeatures.class
--rw-rw-r--  2.0 unx     2117 b- defN 23-Oct-23 22:44 sklearn/neural_network/MLPRegressor.class
--rw-rw-r--  2.0 unx     2638 b- defN 23-Oct-23 22:44 sklearn/neural_network/MLPClassifier.class
--rw-rw-r--  2.0 unx      759 b- defN 23-Oct-23 22:44 sklearn/neural_network/MultilayerPerceptronUtil$1.class
--rw-rw-r--  2.0 unx     8927 b- defN 23-Oct-23 22:44 sklearn/neural_network/MultilayerPerceptronUtil.class
--rw-rw-r--  2.0 unx     2182 b- defN 23-Oct-23 22:44 sklearn/Step.class
--rw-rw-r--  2.0 unx      168 b- defN 23-Oct-23 22:44 sklearn/HasDefaultValue.class
--rw-rw-r--  2.0 unx       99 b- defN 23-Oct-23 22:44 sklearn/Proxy.class
--rw-rw-r--  2.0 unx     2943 b- defN 23-Oct-23 22:44 sklearn/impute/MissingIndicator.class
--rw-rw-r--  2.0 unx     4027 b- defN 23-Oct-23 22:44 sklearn/impute/ImputerUtil.class
--rw-rw-r--  2.0 unx     5710 b- defN 23-Oct-23 22:44 sklearn/impute/SimpleImputer.class
--rw-rw-r--  2.0 unx     6952 b- defN 23-Oct-23 22:44 sklearn/naive_bayes/GaussianNB.class
--rw-rw-r--  2.0 unx      678 b- defN 23-Oct-23 22:44 sklearn/SkLearnRegressor.class
--rw-rw-r--  2.0 unx      233 b- defN 23-Oct-23 22:44 sklearn/HasFeatureNamesIn.class
--rw-rw-r--  2.0 unx     4453 b- defN 23-Oct-23 22:44 sklearn/linear_model/LinearRegressor.class
--rw-rw-r--  2.0 unx     4976 b- defN 23-Oct-23 22:44 sklearn/linear_model/LinearClassifier.class
--rw-rw-r--  2.0 unx     7642 b- defN 23-Oct-23 22:44 sklearn/linear_model/logistic/LogisticRegression.class
--rw-rw-r--  2.0 unx     1042 b- defN 23-Oct-23 22:44 sklearn/linear_model/ridge/RidgeClassifier.class
--rw-rw-r--  2.0 unx      596 b- defN 23-Oct-23 22:44 sklearn/linear_model/glm/DistributionBoundary.class
--rw-rw-r--  2.0 unx     1601 b- defN 23-Oct-23 22:44 sklearn/linear_model/glm/GeneralizedLinearRegressor.class
--rw-rw-r--  2.0 unx      947 b- defN 23-Oct-23 22:44 sklearn/linear_model/stochastic_gradient/Hinge.class
--rw-rw-r--  2.0 unx     2995 b- defN 23-Oct-23 22:44 sklearn/linear_model/stochastic_gradient/SGDOneClassSVM.class
--rw-rw-r--  2.0 unx      461 b- defN 23-Oct-23 22:44 sklearn/linear_model/stochastic_gradient/LossFunction.class
--rw-rw-r--  2.0 unx      452 b- defN 23-Oct-23 22:44 sklearn/linear_model/stochastic_gradient/Log.class
--rw-rw-r--  2.0 unx     1165 b- defN 23-Oct-23 22:44 sklearn/linear_model/stochastic_gradient/SGDClassifier.class
--rw-rw-r--  2.0 unx      482 b- defN 23-Oct-23 22:44 sklearn/linear_model/stochastic_gradient/ModifiedHuber.class
--rw-rw-r--  2.0 unx      968 b- defN 23-Oct-23 22:44 sklearn/linear_model/stochastic_gradient/SquaredHinge.class
--rw-rw-r--  2.0 unx     1746 b- defN 23-Oct-23 22:44 sklearn/compose/ColumnTransformer$1.class
--rw-rw-r--  2.0 unx     3269 b- defN 23-Oct-23 22:44 sklearn/compose/TransformedTargetRegressor.class
--rw-rw-r--  2.0 unx     4386 b- defN 23-Oct-23 22:44 sklearn/compose/ColumnTransformer.class
--rw-rw-r--  2.0 unx     1534 b- defN 23-Oct-23 22:44 sklearn/compose/TransformedTargetRegressor$1.class
--rw-rw-r--  2.0 unx     1158 b- defN 23-Oct-23 22:44 sklearn/IdentityTransformer.class
--rw-rw-r--  2.0 unx     9167 b- defN 23-Oct-23 22:44 sklearn/Classifier.class
--rw-rw-r--  2.0 unx     1457 b- defN 23-Oct-23 22:44 sklearn/model_selection/EstimatorSearcher.class
--rw-rw-r--  2.0 unx     1938 b- defN 23-Oct-23 22:44 sklearn/Selector.class
--rw-rw-r--  2.0 unx      419 b- defN 23-Oct-23 22:44 sklearn/decomposition/IncrementalPCA.class
--rw-rw-r--  2.0 unx     3471 b- defN 23-Oct-23 22:44 sklearn/decomposition/TruncatedSVD.class
--rw-rw-r--  2.0 unx     4759 b- defN 23-Oct-23 22:44 sklearn/decomposition/PCA.class
--rw-rw-r--  2.0 unx      918 b- defN 23-Oct-23 22:44 sklearn/decomposition/BasePCA.class
--rw-rw-r--  2.0 unx      336 b- defN 23-Oct-23 22:44 sklearn/HasPredictField.class
--rw-rw-r--  2.0 unx     3025 b- defN 23-Oct-23 22:44 sklearn/neighbors/NearestNeighbors.class
--rw-rw-r--  2.0 unx     4512 b- defN 23-Oct-23 22:44 sklearn/neighbors/KNeighborsClassifier.class
--rw-rw-r--  2.0 unx     3801 b- defN 23-Oct-23 22:44 sklearn/neighbors/NearestCentroid.class
--rw-rw-r--  2.0 unx     2061 b- defN 23-Oct-23 22:44 sklearn/neighbors/BinaryTree.class
--rw-rw-r--  2.0 unx     1266 b- defN 23-Oct-23 22:44 sklearn/neighbors/KNeighborsUtil$1.class
--rw-rw-r--  2.0 unx      181 b- defN 23-Oct-23 22:44 sklearn/neighbors/HasMetric.class
--rw-rw-r--  2.0 unx    10745 b- defN 23-Oct-23 22:44 sklearn/neighbors/KNeighborsUtil.class
--rw-rw-r--  2.0 unx     4394 b- defN 23-Oct-23 22:44 sklearn/neighbors/KNeighborsRegressor.class
--rw-rw-r--  2.0 unx     1068 b- defN 23-Oct-23 22:44 sklearn/neighbors/DistanceMetric.class
--rw-rw-r--  2.0 unx      351 b- defN 23-Oct-23 22:44 sklearn/neighbors/HasTrainingData.class
--rw-rw-r--  2.0 unx      176 b- defN 23-Oct-23 22:44 sklearn/neighbors/HasNumberOfNeighbors.class
--rw-rw-r--  2.0 unx     1332 b- defN 23-Oct-23 22:44 sklearn/TransformerUtil.class
--rw-rw-r--  2.0 unx     2666 b- defN 23-Oct-23 22:44 sklearn/multioutput/MultiOutputUtil.class
--rw-rw-r--  2.0 unx     3522 b- defN 23-Oct-23 22:44 sklearn/multioutput/ChainUtil.class
--rw-rw-r--  2.0 unx     1631 b- defN 23-Oct-23 22:44 sklearn/multioutput/RegressorChain.class
--rw-rw-r--  2.0 unx     1347 b- defN 23-Oct-23 22:44 sklearn/multioutput/MultiOutputClassifier.class
--rw-rw-r--  2.0 unx     1340 b- defN 23-Oct-23 22:44 sklearn/multioutput/MultiOutputRegressor.class
--rw-rw-r--  2.0 unx     1776 b- defN 23-Oct-23 22:44 sklearn/multioutput/ClassifierChain.class
--rw-rw-r--  2.0 unx     4450 b- defN 23-Oct-23 22:44 sklearn/isotonic/IsotonicRegression.class
--rw-rw-r--  2.0 unx      326 b- defN 23-Oct-23 22:44 sklearn/HasApplyField.class
--rw-rw-r--  2.0 unx      273 b- defN 23-Oct-23 22:44 sklearn/HasEstimatorEnsemble.class
--rw-rw-r--  2.0 unx     2094 b- defN 23-Oct-23 22:44 sklearn/Transformer$1.class
--rw-rw-r--  2.0 unx      953 b- defN 23-Oct-23 22:44 sklearn/LabelEncoderClassifier.class
--rw-rw-r--  2.0 unx      451 b- defN 23-Oct-23 22:44 sklearn/PassThrough.class
--rw-rw-r--  2.0 unx      181 b- defN 23-Oct-23 22:44 sklearn/HasPriorProbability.class
--rw-rw-r--  2.0 unx      230 b- defN 23-Oct-23 22:44 sklearn/SkLearnSteps.class
--rw-rw-r--  2.0 unx     5693 b- defN 23-Oct-23 22:44 sklearn/feature_extraction/text/TfidfVectorizer.class
--rw-rw-r--  2.0 unx      809 b- defN 23-Oct-23 22:44 sklearn/feature_extraction/text/TfidfVectorizer$1.class
--rw-rw-r--  2.0 unx      675 b- defN 23-Oct-23 22:44 sklearn/feature_extraction/text/Tokenizer.class
--rw-rw-r--  2.0 unx    13336 b- defN 23-Oct-23 22:44 sklearn/feature_extraction/text/CountVectorizer.class
--rw-rw-r--  2.0 unx     2129 b- defN 23-Oct-23 22:44 sklearn/feature_extraction/text/CountVectorizer$1.class
--rw-rw-r--  2.0 unx     1433 b- defN 23-Oct-23 22:44 sklearn/feature_extraction/text/TfidfTransformer.class
--rw-rw-r--  2.0 unx     4409 b- defN 23-Oct-23 22:44 sklearn/feature_extraction/DictVectorizer.class
--rw-rw-r--  2.0 unx     1445 b- defN 23-Oct-23 22:44 sklearn/Clusterer.class
--rw-rw-r--  2.0 unx     1411 b- defN 23-Oct-23 22:44 sklearn/metrics/DistanceMetric.class
--rw-rw-r--  2.0 unx     1069 b- defN 23-Oct-23 22:44 sklearn/ensemble/EnsembleUtil.class
--rw-rw-r--  2.0 unx     2112 b- defN 23-Oct-23 22:44 sklearn/ensemble/bagging/BaggingRegressor.class
--rw-rw-r--  2.0 unx     3293 b- defN 23-Oct-23 22:44 sklearn/ensemble/bagging/BaggingUtil.class
--rw-rw-r--  2.0 unx     3028 b- defN 23-Oct-23 22:44 sklearn/ensemble/bagging/BaggingClassifier.class
--rw-rw-r--  2.0 unx     1446 b- defN 23-Oct-23 22:44 sklearn/ensemble/EnsembleRegressor.class
--rw-rw-r--  2.0 unx     3523 b- defN 23-Oct-23 22:44 sklearn/ensemble/stacking/StackingClassifier.class
--rw-rw-r--  2.0 unx      495 b- defN 23-Oct-23 22:44 sklearn/ensemble/stacking/StackingUtil$PredictFunction.class
--rw-rw-r--  2.0 unx     3146 b- defN 23-Oct-23 22:44 sklearn/ensemble/stacking/StackingRegressor.class
--rw-rw-r--  2.0 unx     3862 b- defN 23-Oct-23 22:44 sklearn/ensemble/stacking/StackingUtil.class
--rw-rw-r--  2.0 unx     2524 b- defN 23-Oct-23 22:44 sklearn/ensemble/stacking/StackingClassifier$1.class
--rw-rw-r--  2.0 unx     2254 b- defN 23-Oct-23 22:44 sklearn/ensemble/stacking/StackingRegressor$1.class
--rw-rw-r--  2.0 unx      495 b- defN 23-Oct-23 22:44 sklearn/ensemble/gradient_boosting/ScaledLogOddsEstimator.class
--rw-rw-r--  2.0 unx     1440 b- defN 23-Oct-23 22:44 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$GradientBoostingClassifierProxy.class
--rw-rw-r--  2.0 unx     1862 b- defN 23-Oct-23 22:44 sklearn/ensemble/gradient_boosting/MultinomialDeviance.class
--rw-rw-r--  2.0 unx     2577 b- defN 23-Oct-23 22:44 sklearn/ensemble/gradient_boosting/GradientBoostingRegressor.class
--rw-rw-r--  2.0 unx      858 b- defN 23-Oct-23 22:44 sklearn/ensemble/gradient_boosting/LossFunction.class
--rw-rw-r--  2.0 unx     1588 b- defN 23-Oct-23 22:44 sklearn/ensemble/gradient_boosting/ExponentialLoss.class
--rw-rw-r--  2.0 unx     1317 b- defN 23-Oct-23 22:44 sklearn/ensemble/gradient_boosting/PriorProbabilityEstimator.class
--rw-rw-r--  2.0 unx     7944 b- defN 23-Oct-23 22:44 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier.class
--rw-rw-r--  2.0 unx     1288 b- defN 23-Oct-23 22:44 sklearn/ensemble/gradient_boosting/LogOddsEstimator.class
--rw-rw-r--  2.0 unx      960 b- defN 23-Oct-23 22:44 sklearn/ensemble/gradient_boosting/MeanEstimator.class
--rw-rw-r--  2.0 unx     1265 b- defN 23-Oct-23 22:44 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$1.class
--rw-rw-r--  2.0 unx      980 b- defN 23-Oct-23 22:44 sklearn/ensemble/gradient_boosting/QuantileEstimator.class
--rw-rw-r--  2.0 unx     1578 b- defN 23-Oct-23 22:44 sklearn/ensemble/gradient_boosting/BinomialDeviance.class
--rw-rw-r--  2.0 unx      811 b- defN 23-Oct-23 22:44 sklearn/ensemble/gradient_boosting/ZeroEstimator.class
--rw-rw-r--  2.0 unx     3003 b- defN 23-Oct-23 22:44 sklearn/ensemble/gradient_boosting/GradientBoostingUtil.class
--rw-rw-r--  2.0 unx     1148 b- defN 23-Oct-23 22:44 sklearn/ensemble/EnsembleUtil$1.class
--rw-rw-r--  2.0 unx     3059 b- defN 23-Oct-23 22:44 sklearn/ensemble/forest/ForestUtil.class
--rw-rw-r--  2.0 unx     2542 b- defN 23-Oct-23 22:44 sklearn/ensemble/forest/ForestRegressor.class
--rw-rw-r--  2.0 unx     2998 b- defN 23-Oct-23 22:44 sklearn/ensemble/forest/ForestClassifier.class
--rw-rw-r--  2.0 unx     1752 b- defN 23-Oct-23 22:44 sklearn/ensemble/iforest/IsolationForest$3.class
--rw-rw-r--  2.0 unx     2206 b- defN 23-Oct-23 22:44 sklearn/ensemble/iforest/IsolationForest$1.class
--rw-rw-r--  2.0 unx     1716 b- defN 23-Oct-23 22:44 sklearn/ensemble/iforest/IsolationForest$2.class
--rw-rw-r--  2.0 unx     8756 b- defN 23-Oct-23 22:44 sklearn/ensemble/iforest/IsolationForest.class
--rw-rw-r--  2.0 unx     5090 b- defN 23-Oct-23 22:44 sklearn/ensemble/voting/VotingClassifier.class
--rw-rw-r--  2.0 unx     3753 b- defN 23-Oct-23 22:44 sklearn/ensemble/voting/VotingRegressor.class
--rw-rw-r--  2.0 unx     2821 b- defN 23-Oct-23 22:44 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingRegressor.class
--rw-rw-r--  2.0 unx     1247 b- defN 23-Oct-23 22:44 sklearn/ensemble/hist_gradient_boosting/BinMapper$1.class
--rw-rw-r--  2.0 unx     3041 b- defN 23-Oct-23 22:44 sklearn/ensemble/hist_gradient_boosting/TreePredictor.class
--rw-rw-r--  2.0 unx     6152 b- defN 23-Oct-23 22:44 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingUtil.class
--rw-rw-r--  2.0 unx      505 b- defN 23-Oct-23 22:44 sklearn/ensemble/hist_gradient_boosting/CategoricalCrossEntropy.class
--rw-rw-r--  2.0 unx      490 b- defN 23-Oct-23 22:44 sklearn/ensemble/hist_gradient_boosting/BinaryCrossEntropy.class
--rw-rw-r--  2.0 unx     1572 b- defN 23-Oct-23 22:44 sklearn/ensemble/hist_gradient_boosting/BinMapper.class
--rw-rw-r--  2.0 unx     6305 b- defN 23-Oct-23 22:44 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingClassifier.class
--rw-rw-r--  2.0 unx     8868 b- defN 23-Oct-23 22:44 sklearn/ensemble/hist_gradient_boosting/TreePredictorUtil.class
--rw-rw-r--  2.0 unx      441 b- defN 23-Oct-23 22:44 sklearn/ensemble/hist_gradient_boosting/BaseLoss.class
--rw-rw-r--  2.0 unx     1456 b- defN 23-Oct-23 22:44 sklearn/ensemble/EnsembleClassifier.class
--rw-rw-r--  2.0 unx     3564 b- defN 23-Oct-23 22:44 sklearn/ensemble/weight_boosting/AdaBoostRegressor.class
--rw-rw-r--  2.0 unx     6434 b- defN 23-Oct-23 22:44 sklearn/Transformer.class
--rw-rw-r--  2.0 unx      859 b- defN 23-Oct-23 22:44 sklearn/Transformer$1$1.class
--rw-rw-r--  2.0 unx     1519 b- defN 23-Oct-23 22:44 sklearn/Classifier$1.class
--rw-rw-r--  2.0 unx     1234 b- defN 23-Oct-23 22:44 sklearn/Drop.class
--rw-rw-r--  2.0 unx     1772 b- defN 23-Oct-23 22:44 sklearn/feature_selection/SelectKBest$Entry.class
--rw-rw-r--  2.0 unx     3536 b- defN 23-Oct-23 22:44 sklearn/feature_selection/SelectFromModel.class
--rw-rw-r--  2.0 unx     2947 b- defN 23-Oct-23 22:44 sklearn/feature_selection/SelectKBest.class
--rw-rw-r--  2.0 unx     1499 b- defN 23-Oct-23 22:44 sklearn/feature_selection/SkLearnSelector.class
--rw-rw-r--  2.0 unx      649 b- defN 23-Oct-23 22:44 sklearn/Classifier$3.class
--rw-rw-r--  2.0 unx     2571 b- defN 23-Oct-23 22:44 sklearn/CompositeClassifier.class
--rw-rw-r--  2.0 unx      607 b- defN 23-Oct-23 22:44 sklearn/Transformer$2.class
--rw-rw-r--  2.0 unx      647 b- defN 23-Oct-23 22:44 sklearn/SkLearnTransformer.class
--rw-rw-r--  2.0 unx      412 b- defN 23-Oct-23 22:44 sklearn/loss/HalfMultinomialLoss.class
--rw-rw-r--  2.0 unx      602 b- defN 23-Oct-23 22:44 sklearn/loss/CyLossFunction.class
--rw-rw-r--  2.0 unx      403 b- defN 23-Oct-23 22:44 sklearn/loss/HalfBinomialLoss.class
--rw-rw-r--  2.0 unx      387 b- defN 23-Oct-23 22:44 sklearn/loss/BaseLoss.class
--rw-rw-r--  2.0 unx      381 b- defN 23-Oct-23 22:44 sklearn/HasDecisionFunctionField.class
--rw-rw-r--  2.0 unx      338 b- defN 23-Oct-23 22:44 sklearn/SkLearnMethods.class
--rw-rw-r--  2.0 unx     1515 b- defN 23-Oct-23 22:44 sklearn/OutlierDetectorUtil$1.class
--rw-rw-r--  2.0 unx      238 b- defN 23-Oct-23 22:44 sklearn/HasClasses.class
--rw-rw-r--  2.0 unx     4569 b- defN 23-Oct-23 22:44 sklearn/discriminant_analysis/LinearDiscriminantAnalysis.class
--rw-rw-r--  2.0 unx     1373 b- defN 23-Oct-23 22:44 sklearn/Classifier$2.class
--rw-rw-r--  2.0 unx     1811 b- defN 23-Oct-23 22:44 sklearn/CompositeTransformer.class
--rw-rw-r--  2.0 unx     7517 b- defN 23-Oct-23 22:44 sklearn/Composite.class
--rw-rw-r--  2.0 unx     1194 b- defN 23-Oct-23 22:44 sklearn/preprocessing/KBinsDiscretizer$1.class
--rw-rw-r--  2.0 unx     4574 b- defN 23-Oct-23 22:44 sklearn/preprocessing/PowerTransformer.class
--rw-rw-r--  2.0 unx     2388 b- defN 23-Oct-23 22:44 sklearn/preprocessing/LabelEncoder.class
--rw-rw-r--  2.0 unx     4931 b- defN 23-Oct-23 22:44 sklearn/preprocessing/LabelBinarizer.class
--rw-rw-r--  2.0 unx     1158 b- defN 23-Oct-23 22:44 sklearn/preprocessing/EncoderUtil$3.class
--rw-rw-r--  2.0 unx      396 b- defN 23-Oct-23 22:44 sklearn/preprocessing/Scaler.class
--rw-rw-r--  2.0 unx      797 b- defN 23-Oct-23 22:44 sklearn/preprocessing/MultiOneHotEncoder$1.class
--rw-rw-r--  2.0 unx     3242 b- defN 23-Oct-23 22:44 sklearn/preprocessing/MaxAbsScaler.class
--rw-rw-r--  2.0 unx     2955 b- defN 23-Oct-23 22:44 sklearn/preprocessing/FunctionTransformer.class
--rw-rw-r--  2.0 unx     3293 b- defN 23-Oct-23 22:44 sklearn/preprocessing/BaseEncoder.class
--rw-rw-r--  2.0 unx     1270 b- defN 23-Oct-23 22:44 sklearn/preprocessing/EncoderUtil$1.class
--rw-rw-r--  2.0 unx     4549 b- defN 23-Oct-23 22:44 sklearn/preprocessing/StandardScaler.class
--rw-rw-r--  2.0 unx     9005 b- defN 23-Oct-23 22:44 sklearn/preprocessing/EncoderUtil.class
--rw-rw-r--  2.0 unx     6350 b- defN 23-Oct-23 22:44 sklearn/preprocessing/PolynomialFeatures.class
--rw-rw-r--  2.0 unx     8493 b- defN 23-Oct-23 22:44 sklearn/preprocessing/KBinsDiscretizer.class
--rw-rw-r--  2.0 unx     4678 b- defN 23-Oct-23 22:44 sklearn/preprocessing/OneHotEncoder.class
--rw-rw-r--  2.0 unx      729 b- defN 23-Oct-23 22:44 sklearn/preprocessing/EncoderUtil$4.class
--rw-rw-r--  2.0 unx     2560 b- defN 23-Oct-23 22:44 sklearn/preprocessing/Binarizer.class
--rw-rw-r--  2.0 unx     1054 b- defN 23-Oct-23 22:44 sklearn/preprocessing/EncoderUtil$2.class
--rw-rw-r--  2.0 unx     3595 b- defN 23-Oct-23 22:44 sklearn/preprocessing/MinMaxScaler.class
--rw-rw-r--  2.0 unx     4467 b- defN 23-Oct-23 22:44 sklearn/preprocessing/RobustScaler.class
--rw-rw-r--  2.0 unx     3740 b- defN 23-Oct-23 22:44 sklearn/preprocessing/OrdinalEncoder.class
--rw-rw-r--  2.0 unx      957 b- defN 23-Oct-23 22:44 sklearn/preprocessing/Imputer.class
--rw-rw-r--  2.0 unx     2033 b- defN 23-Oct-23 22:44 sklearn/preprocessing/PolynomialFeatures$1.class
--rw-rw-r--  2.0 unx    10333 b- defN 23-Oct-23 22:44 sklearn/preprocessing/MultiOneHotEncoder.class
--rw-rw-r--  2.0 unx     2157 b- defN 23-Oct-23 22:44 sklearn/tree/TreeClassifier.class
--rw-rw-r--  2.0 unx     3111 b- defN 23-Oct-23 22:44 sklearn/tree/TreeUtil$1.class
--rw-rw-r--  2.0 unx     2664 b- defN 23-Oct-23 22:44 sklearn/tree/TreeUtil$4.class
--rw-rw-r--  2.0 unx     4805 b- defN 23-Oct-23 22:44 sklearn/tree/visitors/TreeModelFlattener.class
--rw-rw-r--  2.0 unx      739 b- defN 23-Oct-23 22:44 sklearn/tree/visitors/TreeModelCompactor$1.class
--rw-rw-r--  2.0 unx     5431 b- defN 23-Oct-23 22:44 sklearn/tree/visitors/TreeModelCompactor.class
--rw-rw-r--  2.0 unx     2988 b- defN 23-Oct-23 22:44 sklearn/tree/visitors/TreeModelPruner.class
--rw-rw-r--  2.0 unx      739 b- defN 23-Oct-23 22:44 sklearn/tree/visitors/TreeModelFlattener$1.class
--rw-rw-r--  2.0 unx      730 b- defN 23-Oct-23 22:44 sklearn/tree/visitors/TreeModelPruner$1.class
--rw-rw-r--  2.0 unx      915 b- defN 23-Oct-23 22:44 sklearn/tree/RegressionCriterion.class
--rw-rw-r--  2.0 unx     1151 b- defN 23-Oct-23 22:44 sklearn/tree/TreeUtil$5.class
--rw-rw-r--  2.0 unx     1014 b- defN 23-Oct-23 22:44 sklearn/tree/PresortBestSplitter.class
--rw-rw-r--  2.0 unx     1589 b- defN 23-Oct-23 22:44 sklearn/tree/TreeUtil$6.class
--rw-rw-r--  2.0 unx     1771 b- defN 23-Oct-23 22:44 sklearn/tree/TreeRegressor.class
--rw-rw-r--  2.0 unx     1489 b- defN 23-Oct-23 22:44 sklearn/tree/TreeUtil$7.class
--rw-rw-r--  2.0 unx    19425 b- defN 23-Oct-23 22:44 sklearn/tree/TreeUtil.class
--rw-rw-r--  2.0 unx     1123 b- defN 23-Oct-23 22:44 sklearn/tree/TreeUtil$3.class
--rw-rw-r--  2.0 unx     1373 b- defN 23-Oct-23 22:44 sklearn/tree/HasTreeOptions.class
--rw-rw-r--  2.0 unx     2293 b- defN 23-Oct-23 22:44 sklearn/tree/Tree.class
--rw-rw-r--  2.0 unx      754 b- defN 23-Oct-23 22:44 sklearn/tree/TreeUtil$2.class
--rw-rw-r--  2.0 unx      150 b- defN 23-Oct-23 22:44 sklearn/tree/HasTree.class
--rw-rw-r--  2.0 unx     2547 b- defN 23-Oct-23 22:44 sklearn/InitializerUtil.class
--rw-rw-r--  2.0 unx     2745 b- defN 23-Oct-23 22:44 sklearn/Regressor.class
--rw-rw-r--  2.0 unx      211 b- defN 23-Oct-23 22:44 sklearn/HasNumberOfOutputs.class
--rw-rw-r--  2.0 unx      534 b- defN 23-Oct-23 22:44 sklearn/OutlierDetector.class
--rw-rw-r--  2.0 unx     3183 b- defN 23-Oct-23 22:44 sklearn/Calibrator.class
--rw-rw-r--  2.0 unx      735 b- defN 23-Oct-23 22:44 sklearn/Composite$1.class
--rw-rw-r--  2.0 unx      273 b- defN 23-Oct-23 22:44 sklearn/HasClassifierOptions.class
--rw-rw-r--  2.0 unx     2309 b- defN 23-Oct-23 22:44 sklearn/CompositeRegressor.class
--rw-rw-r--  2.0 unx     9083 b- defN 23-Oct-23 22:44 sklearn/EstimatorUtil.class
--rw-rw-r--  2.0 unx      199 b- defN 23-Oct-23 22:44 sklearn/HasType.class
--rw-rw-r--  2.0 unx     2417 b- defN 23-Oct-23 22:44 sklearn/CompositeClusterer.class
--rw-rw-r--  2.0 unx      678 b- defN 23-Oct-23 22:44 sklearn/cluster/MiniBatchKMeans.class
--rw-rw-r--  2.0 unx     5093 b- defN 23-Oct-23 22:44 sklearn/cluster/KMeans.class
--rw-rw-r--  2.0 unx    14063 b- defN 23-Oct-23 22:44 sklearn/Estimator.class
--rw-rw-r--  2.0 unx     1575 b- defN 23-Oct-23 22:44 sklearn/Initializer.class
--rw-rw-r--  2.0 unx     4566 b- defN 23-Oct-23 22:44 sklearn/multiclass/OneVsRestClassifier.class
--rw-rw-r--  2.0 unx     5157 b- defN 23-Oct-23 22:44 sklearn2pmml/ruleset/RuleSetClassifier.class
--rw-rw-r--  2.0 unx      386 b- defN 23-Oct-23 22:44 sklearn2pmml/HasPMMLOptions.class
--rw-rw-r--  2.0 unx     1187 b- defN 23-Oct-23 22:44 sklearn2pmml/pipeline/PMMLPipelineUtil$1.class
--rw-rw-r--  2.0 unx    20143 b- defN 23-Oct-23 22:44 sklearn2pmml/pipeline/PMMLPipeline.class
--rw-rw-r--  2.0 unx      684 b- defN 23-Oct-23 22:44 sklearn2pmml/pipeline/PMMLPipeline$2.class
--rw-rw-r--  2.0 unx      980 b- defN 23-Oct-23 22:44 sklearn2pmml/pipeline/PMMLPipeline$1.class
--rw-rw-r--  2.0 unx     1593 b- defN 23-Oct-23 22:44 sklearn2pmml/pipeline/PMMLPipelineUtil.class
--rw-rw-r--  2.0 unx     1811 b- defN 23-Oct-23 22:44 sklearn2pmml/pipeline/Verification.class
--rw-rw-r--  2.0 unx      313 b- defN 23-Oct-23 22:44 sklearn2pmml/HasPMMLName.class
--rw-rw-r--  2.0 unx     2415 b- defN 23-Oct-23 22:44 sklearn2pmml/decoration/MultiDomain.class
--rw-rw-r--  2.0 unx     1152 b- defN 23-Oct-23 22:44 sklearn2pmml/decoration/ContinuousDomainEraser.class
--rw-rw-r--  2.0 unx     1654 b- defN 23-Oct-23 22:44 sklearn2pmml/decoration/Alias.class
--rw-rw-r--  2.0 unx     1772 b- defN 23-Oct-23 22:44 sklearn2pmml/decoration/TemporalDomain.class
--rw-rw-r--  2.0 unx      779 b- defN 23-Oct-23 22:44 sklearn2pmml/decoration/ContinuousDomain$1.class
--rw-rw-r--  2.0 unx    11878 b- defN 23-Oct-23 22:44 sklearn2pmml/decoration/Domain.class
--rw-rw-r--  2.0 unx     1416 b- defN 23-Oct-23 22:44 sklearn2pmml/decoration/MultiAlias.class
--rw-rw-r--  2.0 unx     5055 b- defN 23-Oct-23 22:44 sklearn2pmml/decoration/DiscreteDomain.class
--rw-rw-r--  2.0 unx     1952 b- defN 23-Oct-23 22:44 sklearn2pmml/decoration/CategoricalDomain.class
--rw-rw-r--  2.0 unx     1717 b- defN 23-Oct-23 22:44 sklearn2pmml/decoration/DomainEraser.class
--rw-rw-r--  2.0 unx      613 b- defN 23-Oct-23 22:44 sklearn2pmml/decoration/DateTimeDomain.class
--rw-rw-r--  2.0 unx     7764 b- defN 23-Oct-23 22:44 sklearn2pmml/decoration/ContinuousDomain.class
--rw-rw-r--  2.0 unx     1077 b- defN 23-Oct-23 22:44 sklearn2pmml/decoration/DiscreteDomainEraser.class
--rw-rw-r--  2.0 unx     1590 b- defN 23-Oct-23 22:44 sklearn2pmml/decoration/TransformerWrapper.class
--rw-rw-r--  2.0 unx     1045 b- defN 23-Oct-23 22:44 sklearn2pmml/decoration/Domain$2.class
--rw-rw-r--  2.0 unx      596 b- defN 23-Oct-23 22:44 sklearn2pmml/decoration/DateDomain.class
--rw-rw-r--  2.0 unx     2374 b- defN 23-Oct-23 22:44 sklearn2pmml/decoration/DomainUtil.class
--rw-rw-r--  2.0 unx     1033 b- defN 23-Oct-23 22:44 sklearn2pmml/decoration/Domain$1.class
--rw-rw-r--  2.0 unx     1577 b- defN 23-Oct-23 22:44 sklearn2pmml/decoration/OrdinalDomain.class
--rw-rw-r--  2.0 unx      672 b- defN 23-Oct-23 22:44 sklearn2pmml/decoration/Domain$4.class
--rw-rw-r--  2.0 unx      799 b- defN 23-Oct-23 22:44 sklearn2pmml/decoration/Domain$3.class
--rw-rw-r--  2.0 unx     7879 b- defN 23-Oct-23 22:44 sklearn2pmml/neural_network/MLPTransformer.class
--rw-rw-r--  2.0 unx      391 b- defN 23-Oct-23 22:44 sklearn2pmml/SkLearn2PMMLFields.class
--rw-rw-r--  2.0 unx     1160 b- defN 23-Oct-23 22:44 sklearn2pmml/util/Evaluatable.class
--rw-rw-r--  2.0 unx     1196 b- defN 23-Oct-23 22:44 sklearn2pmml/util/Expression.class
--rw-rw-r--  2.0 unx     1189 b- defN 23-Oct-23 22:44 sklearn2pmml/util/Predicate.class
--rw-rw-r--  2.0 unx      948 b- defN 23-Oct-23 22:44 sklearn2pmml/util/Reshaper.class
--rw-rw-r--  2.0 unx     3392 b- defN 23-Oct-23 22:44 sklearn2pmml/util/EvaluatableUtil.class
--rw-rw-r--  2.0 unx     1922 b- defN 23-Oct-23 22:44 sklearn2pmml/util/Slicer.class
--rw-rw-r--  2.0 unx     2418 b- defN 23-Oct-23 22:44 sklearn2pmml/feature_extraction/text/Splitter.class
--rw-rw-r--  2.0 unx     3184 b- defN 23-Oct-23 22:44 sklearn2pmml/feature_extraction/text/Matcher.class
--rw-rw-r--  2.0 unx      343 b- defN 23-Oct-23 22:44 sklearn2pmml/HasPMMLSegmentId.class
--rw-rw-r--  2.0 unx     1425 b- defN 23-Oct-23 22:44 sklearn2pmml/ensemble/SelectFirstRegressor.class
--rw-rw-r--  2.0 unx     2083 b- defN 23-Oct-23 22:44 sklearn2pmml/ensemble/GBDTUtil$2.class
--rw-rw-r--  2.0 unx      968 b- defN 23-Oct-23 22:44 sklearn2pmml/ensemble/HasEstimatorSteps.class
--rw-rw-r--  2.0 unx     1934 b- defN 23-Oct-23 22:44 sklearn2pmml/ensemble/GBDTLMRegressor.class
--rw-rw-r--  2.0 unx      948 b- defN 23-Oct-23 22:44 sklearn2pmml/ensemble/GBDTUtil$1.class
--rw-rw-r--  2.0 unx     9003 b- defN 23-Oct-23 22:44 sklearn2pmml/ensemble/EstimatorChain.class
--rw-rw-r--  2.0 unx     6001 b- defN 23-Oct-23 22:44 sklearn2pmml/ensemble/GBDTUtil.class
--rw-rw-r--  2.0 unx     4588 b- defN 23-Oct-23 22:44 sklearn2pmml/ensemble/Link.class
--rw-rw-r--  2.0 unx     4563 b- defN 23-Oct-23 22:44 sklearn2pmml/ensemble/SelectFirstUtil.class
--rw-rw-r--  2.0 unx     6835 b- defN 23-Oct-23 22:44 sklearn2pmml/ensemble/OrdinalClassifier.class
--rw-rw-r--  2.0 unx     4382 b- defN 23-Oct-23 22:44 sklearn2pmml/ensemble/GBDTLRClassifier.class
--rw-rw-r--  2.0 unx     2594 b- defN 23-Oct-23 22:44 sklearn2pmml/ensemble/SelectFirstClassifier.class
--rw-rw-r--  2.0 unx     1438 b- defN 23-Oct-23 22:44 sklearn2pmml/EstimatorProxy$1.class
--rw-rw-r--  2.0 unx      946 b- defN 23-Oct-23 22:44 sklearn2pmml/feature_selection/SelectUnique.class
--rw-rw-r--  2.0 unx     1836 b- defN 23-Oct-23 22:44 sklearn2pmml/cross_reference/Memorizer.class
--rw-rw-r--  2.0 unx     2107 b- defN 23-Oct-23 22:44 sklearn2pmml/cross_reference/Recaller.class
--rw-rw-r--  2.0 unx     6477 b- defN 23-Oct-23 22:44 sklearn2pmml/postprocessing/BusinessDecisionTransformer.class
--rw-rw-r--  2.0 unx      791 b- defN 23-Oct-23 22:44 sklearn2pmml/postprocessing/BusinessDecisionTransformer$1.class
--rw-rw-r--  2.0 unx     1197 b- defN 23-Oct-23 22:44 sklearn2pmml/preprocessing/PatternTransformer.class
--rw-rw-r--  2.0 unx     2908 b- defN 23-Oct-23 22:44 sklearn2pmml/preprocessing/ReplaceTransformer.class
--rw-rw-r--  2.0 unx     1865 b- defN 23-Oct-23 22:44 sklearn2pmml/preprocessing/WordCountTransformer.class
--rw-rw-r--  2.0 unx      597 b- defN 23-Oct-23 22:44 sklearn2pmml/preprocessing/DateTimeFormatter.class
--rw-rw-r--  2.0 unx     1288 b- defN 23-Oct-23 22:44 sklearn2pmml/preprocessing/PMMLLabelBinarizer.class
--rw-rw-r--  2.0 unx     4621 b- defN 23-Oct-23 22:44 sklearn2pmml/preprocessing/DurationTransformer.class
--rw-rw-r--  2.0 unx      444 b- defN 23-Oct-23 22:44 sklearn2pmml/preprocessing/PMMLLabelEncoder.class
--rw-rw-r--  2.0 unx     2777 b- defN 23-Oct-23 22:44 sklearn2pmml/preprocessing/FilterLookupTransformer.class
--rw-rw-r--  2.0 unx     2545 b- defN 23-Oct-23 22:44 sklearn2pmml/preprocessing/Formatter.class
--rw-rw-r--  2.0 unx     3424 b- defN 23-Oct-23 22:44 sklearn2pmml/preprocessing/CastTransformer.class
--rw-rw-r--  2.0 unx     2758 b- defN 23-Oct-23 22:44 sklearn2pmml/preprocessing/MatchesTransformer.class
--rw-rw-r--  2.0 unx      589 b- defN 23-Oct-23 22:44 sklearn2pmml/preprocessing/NumberFormatter.class
--rw-rw-r--  2.0 unx     4149 b- defN 23-Oct-23 22:44 sklearn2pmml/preprocessing/MultiLookupTransformer.class
--rw-rw-r--  2.0 unx     3871 b- defN 23-Oct-23 22:44 sklearn2pmml/preprocessing/StringNormalizer.class
--rw-rw-r--  2.0 unx     7145 b- defN 23-Oct-23 22:44 sklearn2pmml/preprocessing/ExpressionTransformer.class
--rw-rw-r--  2.0 unx      635 b- defN 23-Oct-23 22:44 sklearn2pmml/preprocessing/DaysSinceYearTransformer.class
--rw-rw-r--  2.0 unx     3604 b- defN 23-Oct-23 22:44 sklearn2pmml/preprocessing/DataFrameConstructor.class
--rw-rw-r--  2.0 unx     2847 b- defN 23-Oct-23 22:44 sklearn2pmml/preprocessing/ConcatTransformer.class
--rw-rw-r--  2.0 unx     7099 b- defN 23-Oct-23 22:44 sklearn2pmml/preprocessing/CutTransformer.class
--rw-rw-r--  2.0 unx     7025 b- defN 23-Oct-23 22:44 sklearn2pmml/preprocessing/BSplineTransformer.class
--rw-rw-r--  2.0 unx     6410 b- defN 23-Oct-23 22:44 sklearn2pmml/preprocessing/LookupTransformer.class
--rw-rw-r--  2.0 unx     3236 b- defN 23-Oct-23 22:44 sklearn2pmml/preprocessing/SubstringTransformer.class
--rw-rw-r--  2.0 unx     3181 b- defN 23-Oct-23 22:44 sklearn2pmml/preprocessing/SecondsSinceMidnightTransformer.class
--rw-rw-r--  2.0 unx     4881 b- defN 23-Oct-23 22:44 sklearn2pmml/preprocessing/SelectFirstTransformer.class
--rw-rw-r--  2.0 unx     2132 b- defN 23-Oct-23 22:44 sklearn2pmml/preprocessing/PowerFunctionTransformer.class
--rw-rw-r--  2.0 unx     3328 b- defN 23-Oct-23 22:44 sklearn2pmml/preprocessing/Aggregator.class
--rw-rw-r--  2.0 unx      647 b- defN 23-Oct-23 22:44 sklearn2pmml/preprocessing/SecondsSinceYearTransformer.class
--rw-rw-r--  2.0 unx     1639 b- defN 23-Oct-23 22:44 sklearn2pmml/tree/CHAIDRegressor.class
--rw-rw-r--  2.0 unx    10719 b- defN 23-Oct-23 22:44 sklearn2pmml/tree/CHAIDUtil.class
--rw-rw-r--  2.0 unx     2029 b- defN 23-Oct-23 22:44 sklearn2pmml/tree/CHAIDClassifier.class
--rw-rw-r--  2.0 unx     1417 b- defN 23-Oct-23 22:44 sklearn2pmml/tree/CHAIDUtil$1.class
--rw-rw-r--  2.0 unx     5967 b- defN 23-Oct-23 22:44 sklearn2pmml/EstimatorProxy.class
--rw-rw-r--  2.0 unx     1479 b- defN 23-Oct-23 22:44 sklearn2pmml/SelectorProxy.class
--rw-rw-r--  2.0 unx     2046 b- defN 23-Oct-23 22:44 sklearn2pmml/expression/ExpressionUtil.class
--rw-rw-r--  2.0 unx     3799 b- defN 23-Oct-23 22:44 sklearn2pmml/expression/ExpressionRegressor.class
--rw-rw-r--  2.0 unx      990 b- defN 23-Oct-23 22:44 sklearn2pmml/expression/ExpressionClassifier$1.class
--rw-rw-r--  2.0 unx     8684 b- defN 23-Oct-23 22:44 sklearn2pmml/expression/ExpressionClassifier.class
--rw-rw-r--  2.0 unx      948 b- defN 23-Oct-23 22:44 sklearn2pmml/expression/ExpressionUtil$1.class
--rw-rw-r--  2.0 unx      162 b- defN 23-Oct-23 22:44 org/jpmml/sklearn/Encodable.class
--rw-rw-r--  2.0 unx     1774 b- defN 23-Oct-23 22:44 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest$1.class
--rw-rw-r--  2.0 unx     2913 b- defN 23-Oct-23 22:44 org/jpmml/sklearn/testing/SkLearnEncoderBatch.class
--rw-rw-r--  2.0 unx     3549 b- defN 23-Oct-23 22:44 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest.class
--rw-rw-r--  2.0 unx    17241 b- defN 23-Oct-23 22:44 org/jpmml/sklearn/SkLearnEncoder.class
--rw-rw-r--  2.0 unx     3123 b- defN 23-Oct-23 22:44 org/jpmml/sklearn/EncodableUtil.class
--rw-rw-r--  2.0 unx      194 b- defN 23-Oct-23 22:44 org/jpmml/sklearn/FieldNames.class
--rw-rw-r--  2.0 unx      171 b- defN 23-Oct-23 22:44 org/jpmml/sklearn/HasSkLearnOptions.class
--rw-rw-r--  2.0 unx      664 b- defN 23-Oct-23 22:44 org/jpmml/sklearn/SkLearnUtil.class
--rw-rw-r--  2.0 unx     1179 b- defN 23-Oct-23 22:44 org/jpmml/sklearn/SkLearnEncoder$1.class
--rw-rw-r--  2.0 unx     1859 b- defN 23-Oct-23 22:44 META-INF/maven/org.jpmml/pmml-sklearn/pom.xml
--rw-rw-r--  2.0 unx       57 b- defN 23-Oct-23 22:44 META-INF/maven/org.jpmml/pmml-sklearn/pom.properties
-427 files, 980257 bytes uncompressed, 431340 bytes compressed:  56.0%
+Zip file size: 500181 bytes, number of entries: 430
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 META-INF/
+-rw-r--r--  2.0 unx      159 b- defN 23-Dec-04 22:17 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn_pandas/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 chaid/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 stop_words/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/calibration/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/pipeline/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/dummy/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/svm/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/neural_network/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/impute/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/naive_bayes/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/linear_model/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/linear_model/logistic/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/linear_model/ridge/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/linear_model/glm/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/linear_model/stochastic_gradient/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/compose/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/model_selection/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/decomposition/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/neighbors/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/multioutput/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/isotonic/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/feature_extraction/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/feature_extraction/text/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/metrics/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/ensemble/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/ensemble/bagging/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/ensemble/stacking/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/ensemble/gradient_boosting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/ensemble/forest/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/ensemble/iforest/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/ensemble/voting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/ensemble/hist_gradient_boosting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/ensemble/weight_boosting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/feature_selection/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/loss/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/discriminant_analysis/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/preprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/tree/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/tree/visitors/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/cluster/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn/multiclass/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn2pmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn2pmml/ruleset/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn2pmml/pipeline/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn2pmml/decoration/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn2pmml/neural_network/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn2pmml/util/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn2pmml/feature_extraction/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn2pmml/feature_extraction/text/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn2pmml/ensemble/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn2pmml/feature_selection/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn2pmml/cross_reference/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn2pmml/postprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn2pmml/preprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn2pmml/tree/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn2pmml/expression/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 org/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 org/jpmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 org/jpmml/sklearn/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 org/jpmml/sklearn/testing/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 META-INF/maven/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 META-INF/maven/org.jpmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 META-INF/maven/org.jpmml/pmml-sklearn/
+-rw-rw-r--  2.0 unx    17154 b- defN 23-Dec-04 22:17 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx     2287 b- defN 23-Dec-04 22:17 sklearn_pandas/CategoricalImputer.class
+-rw-rw-r--  2.0 unx      656 b- defN 23-Dec-04 22:17 sklearn_pandas/TransformerPipeline.class
+-rw-rw-r--  2.0 unx     1154 b- defN 23-Dec-04 22:17 sklearn_pandas/DataFrameMapper$2.class
+-rw-rw-r--  2.0 unx     6280 b- defN 23-Dec-04 22:17 sklearn_pandas/DataFrameMapper.class
+-rw-rw-r--  2.0 unx     1126 b- defN 23-Dec-04 22:17 sklearn_pandas/DataFrameMapper$1.class
+-rw-rw-r--  2.0 unx      609 b- defN 23-Dec-04 22:17 chaid/ContinuousColumn.class
+-rw-rw-r--  2.0 unx      925 b- defN 23-Dec-04 22:17 chaid/Node.class
+-rw-rw-r--  2.0 unx      467 b- defN 23-Dec-04 22:17 chaid/Column.class
+-rw-rw-r--  2.0 unx     3283 b- defN 23-Dec-04 22:17 chaid/Split.class
+-rw-rw-r--  2.0 unx      401 b- defN 23-Dec-04 22:17 chaid/InvalidSplitReason.class
+-rw-rw-r--  2.0 unx      602 b- defN 23-Dec-04 22:17 chaid/NominalColumn.class
+-rw-rw-r--  2.0 unx     1912 b- defN 23-Dec-04 22:17 stop_words/english.txt
+-rw-rw-r--  2.0 unx      140 b- defN 23-Dec-04 22:17 sklearn/HasHead.class
+-rw-rw-r--  2.0 unx     1959 b- defN 23-Dec-04 22:17 sklearn/StepUtil.class
+-rw-rw-r--  2.0 unx    12886 b- defN 23-Dec-04 22:17 sklearn/calibration/CalibratedClassifier.class
+-rw-rw-r--  2.0 unx     2953 b- defN 23-Dec-04 22:17 sklearn/calibration/SigmoidCalibration.class
+-rw-rw-r--  2.0 unx      683 b- defN 23-Dec-04 22:17 sklearn/calibration/CalibratedClassifier$1.class
+-rw-rw-r--  2.0 unx     3676 b- defN 23-Dec-04 22:17 sklearn/calibration/CalibratedClassifierCV.class
+-rw-rw-r--  2.0 unx     2216 b- defN 23-Dec-04 22:17 sklearn/VersionUtil.class
+-rw-rw-r--  2.0 unx     2818 b- defN 23-Dec-04 22:17 sklearn/pipeline/FeatureUnion.class
+-rw-rw-r--  2.0 unx     1670 b- defN 23-Dec-04 22:17 sklearn/pipeline/SkLearnPipeline$3.class
+-rw-rw-r--  2.0 unx     5196 b- defN 23-Dec-04 22:17 sklearn/pipeline/SkLearnPipeline.class
+-rw-rw-r--  2.0 unx     1709 b- defN 23-Dec-04 22:17 sklearn/pipeline/SkLearnPipeline$2.class
+-rw-rw-r--  2.0 unx     1772 b- defN 23-Dec-04 22:17 sklearn/pipeline/SkLearnPipeline$1.class
+-rw-rw-r--  2.0 unx      682 b- defN 23-Dec-04 22:17 sklearn/SkLearnClassifier.class
+-rw-rw-r--  2.0 unx     5031 b- defN 23-Dec-04 22:17 sklearn/dummy/DummyClassifier.class
+-rw-rw-r--  2.0 unx     2181 b- defN 23-Dec-04 22:17 sklearn/dummy/DummyRegressor.class
+-rw-rw-r--  2.0 unx      512 b- defN 23-Dec-04 22:17 sklearn/SkLearnFields.class
+-rw-rw-r--  2.0 unx     2293 b- defN 23-Dec-04 22:17 sklearn/SkLearnOutlierTransformation.class
+-rw-rw-r--  2.0 unx      240 b- defN 23-Dec-04 22:17 sklearn/HasEstimator.class
+-rw-rw-r--  2.0 unx     3421 b- defN 23-Dec-04 22:17 sklearn/OutlierDetectorUtil.class
+-rw-rw-r--  2.0 unx     1236 b- defN 23-Dec-04 22:17 sklearn/HasMultiApplyField.class
+-rw-rw-r--  2.0 unx      591 b- defN 23-Dec-04 22:17 sklearn/HasMultiDecisionFunctionField.class
+-rw-rw-r--  2.0 unx     2393 b- defN 23-Dec-04 22:17 sklearn/svm/SupportVectorMachineUtil.class
+-rw-rw-r--  2.0 unx     1109 b- defN 23-Dec-04 22:17 sklearn/svm/LinearSVC.class
+-rw-rw-r--  2.0 unx     5044 b- defN 23-Dec-04 22:17 sklearn/svm/LibSVMClassifier.class
+-rw-rw-r--  2.0 unx      966 b- defN 23-Dec-04 22:17 sklearn/svm/SupportVectorMachineUtil$1.class
+-rw-rw-r--  2.0 unx     1869 b- defN 23-Dec-04 22:17 sklearn/svm/OneClassSVM.class
+-rw-rw-r--  2.0 unx     3601 b- defN 23-Dec-04 22:17 sklearn/svm/LibSVMRegressor.class
+-rw-rw-r--  2.0 unx      678 b- defN 23-Dec-04 22:17 sklearn/SkLearnClusterer.class
+-rw-rw-r--  2.0 unx     2584 b- defN 23-Dec-04 22:17 sklearn/InitializerUtil$1.class
+-rw-rw-r--  2.0 unx      342 b- defN 23-Dec-04 22:17 sklearn/HasOutlierField.class
+-rw-rw-r--  2.0 unx      214 b- defN 23-Dec-04 22:17 sklearn/HasNumberOfFeatures.class
+-rw-rw-r--  2.0 unx     2117 b- defN 23-Dec-04 22:17 sklearn/neural_network/MLPRegressor.class
+-rw-rw-r--  2.0 unx     2638 b- defN 23-Dec-04 22:17 sklearn/neural_network/MLPClassifier.class
+-rw-rw-r--  2.0 unx      759 b- defN 23-Dec-04 22:17 sklearn/neural_network/MultilayerPerceptronUtil$1.class
+-rw-rw-r--  2.0 unx     8927 b- defN 23-Dec-04 22:17 sklearn/neural_network/MultilayerPerceptronUtil.class
+-rw-rw-r--  2.0 unx     2182 b- defN 23-Dec-04 22:17 sklearn/Step.class
+-rw-rw-r--  2.0 unx      168 b- defN 23-Dec-04 22:17 sklearn/HasDefaultValue.class
+-rw-rw-r--  2.0 unx       99 b- defN 23-Dec-04 22:17 sklearn/Proxy.class
+-rw-rw-r--  2.0 unx     2943 b- defN 23-Dec-04 22:17 sklearn/impute/MissingIndicator.class
+-rw-rw-r--  2.0 unx     4027 b- defN 23-Dec-04 22:17 sklearn/impute/ImputerUtil.class
+-rw-rw-r--  2.0 unx     5710 b- defN 23-Dec-04 22:17 sklearn/impute/SimpleImputer.class
+-rw-rw-r--  2.0 unx     6952 b- defN 23-Dec-04 22:17 sklearn/naive_bayes/GaussianNB.class
+-rw-rw-r--  2.0 unx      678 b- defN 23-Dec-04 22:17 sklearn/SkLearnRegressor.class
+-rw-rw-r--  2.0 unx      233 b- defN 23-Dec-04 22:17 sklearn/HasFeatureNamesIn.class
+-rw-rw-r--  2.0 unx     4453 b- defN 23-Dec-04 22:17 sklearn/linear_model/LinearRegressor.class
+-rw-rw-r--  2.0 unx     4976 b- defN 23-Dec-04 22:17 sklearn/linear_model/LinearClassifier.class
+-rw-rw-r--  2.0 unx     7642 b- defN 23-Dec-04 22:17 sklearn/linear_model/logistic/LogisticRegression.class
+-rw-rw-r--  2.0 unx     1042 b- defN 23-Dec-04 22:17 sklearn/linear_model/ridge/RidgeClassifier.class
+-rw-rw-r--  2.0 unx      596 b- defN 23-Dec-04 22:17 sklearn/linear_model/glm/DistributionBoundary.class
+-rw-rw-r--  2.0 unx     1601 b- defN 23-Dec-04 22:17 sklearn/linear_model/glm/GeneralizedLinearRegressor.class
+-rw-rw-r--  2.0 unx      947 b- defN 23-Dec-04 22:17 sklearn/linear_model/stochastic_gradient/Hinge.class
+-rw-rw-r--  2.0 unx     2995 b- defN 23-Dec-04 22:17 sklearn/linear_model/stochastic_gradient/SGDOneClassSVM.class
+-rw-rw-r--  2.0 unx      461 b- defN 23-Dec-04 22:17 sklearn/linear_model/stochastic_gradient/LossFunction.class
+-rw-rw-r--  2.0 unx      452 b- defN 23-Dec-04 22:17 sklearn/linear_model/stochastic_gradient/Log.class
+-rw-rw-r--  2.0 unx     1165 b- defN 23-Dec-04 22:17 sklearn/linear_model/stochastic_gradient/SGDClassifier.class
+-rw-rw-r--  2.0 unx      482 b- defN 23-Dec-04 22:17 sklearn/linear_model/stochastic_gradient/ModifiedHuber.class
+-rw-rw-r--  2.0 unx      968 b- defN 23-Dec-04 22:17 sklearn/linear_model/stochastic_gradient/SquaredHinge.class
+-rw-rw-r--  2.0 unx     1746 b- defN 23-Dec-04 22:17 sklearn/compose/ColumnTransformer$1.class
+-rw-rw-r--  2.0 unx     3269 b- defN 23-Dec-04 22:17 sklearn/compose/TransformedTargetRegressor.class
+-rw-rw-r--  2.0 unx     4386 b- defN 23-Dec-04 22:17 sklearn/compose/ColumnTransformer.class
+-rw-rw-r--  2.0 unx     1534 b- defN 23-Dec-04 22:17 sklearn/compose/TransformedTargetRegressor$1.class
+-rw-rw-r--  2.0 unx     1158 b- defN 23-Dec-04 22:17 sklearn/IdentityTransformer.class
+-rw-rw-r--  2.0 unx     9167 b- defN 23-Dec-04 22:17 sklearn/Classifier.class
+-rw-rw-r--  2.0 unx     1457 b- defN 23-Dec-04 22:17 sklearn/model_selection/EstimatorSearcher.class
+-rw-rw-r--  2.0 unx     1938 b- defN 23-Dec-04 22:17 sklearn/Selector.class
+-rw-rw-r--  2.0 unx      419 b- defN 23-Dec-04 22:17 sklearn/decomposition/IncrementalPCA.class
+-rw-rw-r--  2.0 unx     3471 b- defN 23-Dec-04 22:17 sklearn/decomposition/TruncatedSVD.class
+-rw-rw-r--  2.0 unx     4759 b- defN 23-Dec-04 22:17 sklearn/decomposition/PCA.class
+-rw-rw-r--  2.0 unx      918 b- defN 23-Dec-04 22:17 sklearn/decomposition/BasePCA.class
+-rw-rw-r--  2.0 unx      336 b- defN 23-Dec-04 22:17 sklearn/HasPredictField.class
+-rw-rw-r--  2.0 unx     3025 b- defN 23-Dec-04 22:17 sklearn/neighbors/NearestNeighbors.class
+-rw-rw-r--  2.0 unx     4512 b- defN 23-Dec-04 22:17 sklearn/neighbors/KNeighborsClassifier.class
+-rw-rw-r--  2.0 unx     3801 b- defN 23-Dec-04 22:17 sklearn/neighbors/NearestCentroid.class
+-rw-rw-r--  2.0 unx     2061 b- defN 23-Dec-04 22:17 sklearn/neighbors/BinaryTree.class
+-rw-rw-r--  2.0 unx     1266 b- defN 23-Dec-04 22:17 sklearn/neighbors/KNeighborsUtil$1.class
+-rw-rw-r--  2.0 unx      181 b- defN 23-Dec-04 22:17 sklearn/neighbors/HasMetric.class
+-rw-rw-r--  2.0 unx    10745 b- defN 23-Dec-04 22:17 sklearn/neighbors/KNeighborsUtil.class
+-rw-rw-r--  2.0 unx     4394 b- defN 23-Dec-04 22:17 sklearn/neighbors/KNeighborsRegressor.class
+-rw-rw-r--  2.0 unx     1068 b- defN 23-Dec-04 22:17 sklearn/neighbors/DistanceMetric.class
+-rw-rw-r--  2.0 unx      351 b- defN 23-Dec-04 22:17 sklearn/neighbors/HasTrainingData.class
+-rw-rw-r--  2.0 unx      176 b- defN 23-Dec-04 22:17 sklearn/neighbors/HasNumberOfNeighbors.class
+-rw-rw-r--  2.0 unx     1332 b- defN 23-Dec-04 22:17 sklearn/TransformerUtil.class
+-rw-rw-r--  2.0 unx     2666 b- defN 23-Dec-04 22:17 sklearn/multioutput/MultiOutputUtil.class
+-rw-rw-r--  2.0 unx     3522 b- defN 23-Dec-04 22:17 sklearn/multioutput/ChainUtil.class
+-rw-rw-r--  2.0 unx     1631 b- defN 23-Dec-04 22:17 sklearn/multioutput/RegressorChain.class
+-rw-rw-r--  2.0 unx     1347 b- defN 23-Dec-04 22:17 sklearn/multioutput/MultiOutputClassifier.class
+-rw-rw-r--  2.0 unx     1340 b- defN 23-Dec-04 22:17 sklearn/multioutput/MultiOutputRegressor.class
+-rw-rw-r--  2.0 unx     1776 b- defN 23-Dec-04 22:17 sklearn/multioutput/ClassifierChain.class
+-rw-rw-r--  2.0 unx     4450 b- defN 23-Dec-04 22:17 sklearn/isotonic/IsotonicRegression.class
+-rw-rw-r--  2.0 unx      326 b- defN 23-Dec-04 22:17 sklearn/HasApplyField.class
+-rw-rw-r--  2.0 unx      273 b- defN 23-Dec-04 22:17 sklearn/HasEstimatorEnsemble.class
+-rw-rw-r--  2.0 unx     2094 b- defN 23-Dec-04 22:17 sklearn/Transformer$1.class
+-rw-rw-r--  2.0 unx      953 b- defN 23-Dec-04 22:17 sklearn/LabelEncoderClassifier.class
+-rw-rw-r--  2.0 unx      451 b- defN 23-Dec-04 22:17 sklearn/PassThrough.class
+-rw-rw-r--  2.0 unx      181 b- defN 23-Dec-04 22:17 sklearn/HasPriorProbability.class
+-rw-rw-r--  2.0 unx      230 b- defN 23-Dec-04 22:17 sklearn/SkLearnSteps.class
+-rw-rw-r--  2.0 unx     5693 b- defN 23-Dec-04 22:17 sklearn/feature_extraction/text/TfidfVectorizer.class
+-rw-rw-r--  2.0 unx      809 b- defN 23-Dec-04 22:17 sklearn/feature_extraction/text/TfidfVectorizer$1.class
+-rw-rw-r--  2.0 unx      675 b- defN 23-Dec-04 22:17 sklearn/feature_extraction/text/Tokenizer.class
+-rw-rw-r--  2.0 unx    13336 b- defN 23-Dec-04 22:17 sklearn/feature_extraction/text/CountVectorizer.class
+-rw-rw-r--  2.0 unx     2129 b- defN 23-Dec-04 22:17 sklearn/feature_extraction/text/CountVectorizer$1.class
+-rw-rw-r--  2.0 unx     1433 b- defN 23-Dec-04 22:17 sklearn/feature_extraction/text/TfidfTransformer.class
+-rw-rw-r--  2.0 unx     4409 b- defN 23-Dec-04 22:17 sklearn/feature_extraction/DictVectorizer.class
+-rw-rw-r--  2.0 unx     1445 b- defN 23-Dec-04 22:17 sklearn/Clusterer.class
+-rw-rw-r--  2.0 unx     1411 b- defN 23-Dec-04 22:17 sklearn/metrics/DistanceMetric.class
+-rw-rw-r--  2.0 unx     1069 b- defN 23-Dec-04 22:17 sklearn/ensemble/EnsembleUtil.class
+-rw-rw-r--  2.0 unx     2112 b- defN 23-Dec-04 22:17 sklearn/ensemble/bagging/BaggingRegressor.class
+-rw-rw-r--  2.0 unx     3293 b- defN 23-Dec-04 22:17 sklearn/ensemble/bagging/BaggingUtil.class
+-rw-rw-r--  2.0 unx     3028 b- defN 23-Dec-04 22:17 sklearn/ensemble/bagging/BaggingClassifier.class
+-rw-rw-r--  2.0 unx     1446 b- defN 23-Dec-04 22:17 sklearn/ensemble/EnsembleRegressor.class
+-rw-rw-r--  2.0 unx     3523 b- defN 23-Dec-04 22:17 sklearn/ensemble/stacking/StackingClassifier.class
+-rw-rw-r--  2.0 unx      495 b- defN 23-Dec-04 22:17 sklearn/ensemble/stacking/StackingUtil$PredictFunction.class
+-rw-rw-r--  2.0 unx     3146 b- defN 23-Dec-04 22:17 sklearn/ensemble/stacking/StackingRegressor.class
+-rw-rw-r--  2.0 unx     3862 b- defN 23-Dec-04 22:17 sklearn/ensemble/stacking/StackingUtil.class
+-rw-rw-r--  2.0 unx     2524 b- defN 23-Dec-04 22:17 sklearn/ensemble/stacking/StackingClassifier$1.class
+-rw-rw-r--  2.0 unx     2254 b- defN 23-Dec-04 22:17 sklearn/ensemble/stacking/StackingRegressor$1.class
+-rw-rw-r--  2.0 unx      495 b- defN 23-Dec-04 22:17 sklearn/ensemble/gradient_boosting/ScaledLogOddsEstimator.class
+-rw-rw-r--  2.0 unx     1440 b- defN 23-Dec-04 22:17 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$GradientBoostingClassifierProxy.class
+-rw-rw-r--  2.0 unx     1862 b- defN 23-Dec-04 22:17 sklearn/ensemble/gradient_boosting/MultinomialDeviance.class
+-rw-rw-r--  2.0 unx     2577 b- defN 23-Dec-04 22:17 sklearn/ensemble/gradient_boosting/GradientBoostingRegressor.class
+-rw-rw-r--  2.0 unx      858 b- defN 23-Dec-04 22:17 sklearn/ensemble/gradient_boosting/LossFunction.class
+-rw-rw-r--  2.0 unx     1588 b- defN 23-Dec-04 22:17 sklearn/ensemble/gradient_boosting/ExponentialLoss.class
+-rw-rw-r--  2.0 unx     1317 b- defN 23-Dec-04 22:17 sklearn/ensemble/gradient_boosting/PriorProbabilityEstimator.class
+-rw-rw-r--  2.0 unx     7944 b- defN 23-Dec-04 22:17 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier.class
+-rw-rw-r--  2.0 unx     1288 b- defN 23-Dec-04 22:17 sklearn/ensemble/gradient_boosting/LogOddsEstimator.class
+-rw-rw-r--  2.0 unx      960 b- defN 23-Dec-04 22:17 sklearn/ensemble/gradient_boosting/MeanEstimator.class
+-rw-rw-r--  2.0 unx     1265 b- defN 23-Dec-04 22:17 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$1.class
+-rw-rw-r--  2.0 unx      980 b- defN 23-Dec-04 22:17 sklearn/ensemble/gradient_boosting/QuantileEstimator.class
+-rw-rw-r--  2.0 unx     1578 b- defN 23-Dec-04 22:17 sklearn/ensemble/gradient_boosting/BinomialDeviance.class
+-rw-rw-r--  2.0 unx      811 b- defN 23-Dec-04 22:17 sklearn/ensemble/gradient_boosting/ZeroEstimator.class
+-rw-rw-r--  2.0 unx     3003 b- defN 23-Dec-04 22:17 sklearn/ensemble/gradient_boosting/GradientBoostingUtil.class
+-rw-rw-r--  2.0 unx     1148 b- defN 23-Dec-04 22:17 sklearn/ensemble/EnsembleUtil$1.class
+-rw-rw-r--  2.0 unx     3059 b- defN 23-Dec-04 22:17 sklearn/ensemble/forest/ForestUtil.class
+-rw-rw-r--  2.0 unx     2542 b- defN 23-Dec-04 22:17 sklearn/ensemble/forest/ForestRegressor.class
+-rw-rw-r--  2.0 unx     2998 b- defN 23-Dec-04 22:17 sklearn/ensemble/forest/ForestClassifier.class
+-rw-rw-r--  2.0 unx     1752 b- defN 23-Dec-04 22:17 sklearn/ensemble/iforest/IsolationForest$3.class
+-rw-rw-r--  2.0 unx     2206 b- defN 23-Dec-04 22:17 sklearn/ensemble/iforest/IsolationForest$1.class
+-rw-rw-r--  2.0 unx     1716 b- defN 23-Dec-04 22:17 sklearn/ensemble/iforest/IsolationForest$2.class
+-rw-rw-r--  2.0 unx     8756 b- defN 23-Dec-04 22:17 sklearn/ensemble/iforest/IsolationForest.class
+-rw-rw-r--  2.0 unx     5090 b- defN 23-Dec-04 22:17 sklearn/ensemble/voting/VotingClassifier.class
+-rw-rw-r--  2.0 unx     3753 b- defN 23-Dec-04 22:17 sklearn/ensemble/voting/VotingRegressor.class
+-rw-rw-r--  2.0 unx     2821 b- defN 23-Dec-04 22:17 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingRegressor.class
+-rw-rw-r--  2.0 unx     1247 b- defN 23-Dec-04 22:17 sklearn/ensemble/hist_gradient_boosting/BinMapper$1.class
+-rw-rw-r--  2.0 unx     3041 b- defN 23-Dec-04 22:17 sklearn/ensemble/hist_gradient_boosting/TreePredictor.class
+-rw-rw-r--  2.0 unx     6152 b- defN 23-Dec-04 22:17 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingUtil.class
+-rw-rw-r--  2.0 unx      505 b- defN 23-Dec-04 22:17 sklearn/ensemble/hist_gradient_boosting/CategoricalCrossEntropy.class
+-rw-rw-r--  2.0 unx      490 b- defN 23-Dec-04 22:17 sklearn/ensemble/hist_gradient_boosting/BinaryCrossEntropy.class
+-rw-rw-r--  2.0 unx     1572 b- defN 23-Dec-04 22:17 sklearn/ensemble/hist_gradient_boosting/BinMapper.class
+-rw-rw-r--  2.0 unx     6305 b- defN 23-Dec-04 22:17 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingClassifier.class
+-rw-rw-r--  2.0 unx     8868 b- defN 23-Dec-04 22:17 sklearn/ensemble/hist_gradient_boosting/TreePredictorUtil.class
+-rw-rw-r--  2.0 unx      441 b- defN 23-Dec-04 22:17 sklearn/ensemble/hist_gradient_boosting/BaseLoss.class
+-rw-rw-r--  2.0 unx     1456 b- defN 23-Dec-04 22:17 sklearn/ensemble/EnsembleClassifier.class
+-rw-rw-r--  2.0 unx     3564 b- defN 23-Dec-04 22:17 sklearn/ensemble/weight_boosting/AdaBoostRegressor.class
+-rw-rw-r--  2.0 unx     6434 b- defN 23-Dec-04 22:17 sklearn/Transformer.class
+-rw-rw-r--  2.0 unx      859 b- defN 23-Dec-04 22:17 sklearn/Transformer$1$1.class
+-rw-rw-r--  2.0 unx     1519 b- defN 23-Dec-04 22:17 sklearn/Classifier$1.class
+-rw-rw-r--  2.0 unx     1234 b- defN 23-Dec-04 22:17 sklearn/Drop.class
+-rw-rw-r--  2.0 unx     1772 b- defN 23-Dec-04 22:17 sklearn/feature_selection/SelectKBest$Entry.class
+-rw-rw-r--  2.0 unx     3536 b- defN 23-Dec-04 22:17 sklearn/feature_selection/SelectFromModel.class
+-rw-rw-r--  2.0 unx     2947 b- defN 23-Dec-04 22:17 sklearn/feature_selection/SelectKBest.class
+-rw-rw-r--  2.0 unx     1499 b- defN 23-Dec-04 22:17 sklearn/feature_selection/SkLearnSelector.class
+-rw-rw-r--  2.0 unx      649 b- defN 23-Dec-04 22:17 sklearn/Classifier$3.class
+-rw-rw-r--  2.0 unx     2571 b- defN 23-Dec-04 22:17 sklearn/CompositeClassifier.class
+-rw-rw-r--  2.0 unx      607 b- defN 23-Dec-04 22:17 sklearn/Transformer$2.class
+-rw-rw-r--  2.0 unx      647 b- defN 23-Dec-04 22:17 sklearn/SkLearnTransformer.class
+-rw-rw-r--  2.0 unx      412 b- defN 23-Dec-04 22:17 sklearn/loss/HalfMultinomialLoss.class
+-rw-rw-r--  2.0 unx      602 b- defN 23-Dec-04 22:17 sklearn/loss/CyLossFunction.class
+-rw-rw-r--  2.0 unx      403 b- defN 23-Dec-04 22:17 sklearn/loss/HalfBinomialLoss.class
+-rw-rw-r--  2.0 unx      387 b- defN 23-Dec-04 22:17 sklearn/loss/BaseLoss.class
+-rw-rw-r--  2.0 unx      381 b- defN 23-Dec-04 22:17 sklearn/HasDecisionFunctionField.class
+-rw-rw-r--  2.0 unx      338 b- defN 23-Dec-04 22:17 sklearn/SkLearnMethods.class
+-rw-rw-r--  2.0 unx     1515 b- defN 23-Dec-04 22:17 sklearn/OutlierDetectorUtil$1.class
+-rw-rw-r--  2.0 unx      238 b- defN 23-Dec-04 22:17 sklearn/HasClasses.class
+-rw-rw-r--  2.0 unx     4569 b- defN 23-Dec-04 22:17 sklearn/discriminant_analysis/LinearDiscriminantAnalysis.class
+-rw-rw-r--  2.0 unx     1373 b- defN 23-Dec-04 22:17 sklearn/Classifier$2.class
+-rw-rw-r--  2.0 unx     1811 b- defN 23-Dec-04 22:17 sklearn/CompositeTransformer.class
+-rw-rw-r--  2.0 unx     7517 b- defN 23-Dec-04 22:17 sklearn/Composite.class
+-rw-rw-r--  2.0 unx     1194 b- defN 23-Dec-04 22:17 sklearn/preprocessing/KBinsDiscretizer$1.class
+-rw-rw-r--  2.0 unx     4574 b- defN 23-Dec-04 22:17 sklearn/preprocessing/PowerTransformer.class
+-rw-rw-r--  2.0 unx     2388 b- defN 23-Dec-04 22:17 sklearn/preprocessing/LabelEncoder.class
+-rw-rw-r--  2.0 unx     4931 b- defN 23-Dec-04 22:17 sklearn/preprocessing/LabelBinarizer.class
+-rw-rw-r--  2.0 unx     1158 b- defN 23-Dec-04 22:17 sklearn/preprocessing/EncoderUtil$3.class
+-rw-rw-r--  2.0 unx      396 b- defN 23-Dec-04 22:17 sklearn/preprocessing/Scaler.class
+-rw-rw-r--  2.0 unx      797 b- defN 23-Dec-04 22:17 sklearn/preprocessing/MultiOneHotEncoder$1.class
+-rw-rw-r--  2.0 unx     3242 b- defN 23-Dec-04 22:17 sklearn/preprocessing/MaxAbsScaler.class
+-rw-rw-r--  2.0 unx     2955 b- defN 23-Dec-04 22:17 sklearn/preprocessing/FunctionTransformer.class
+-rw-rw-r--  2.0 unx     3293 b- defN 23-Dec-04 22:17 sklearn/preprocessing/BaseEncoder.class
+-rw-rw-r--  2.0 unx     1270 b- defN 23-Dec-04 22:17 sklearn/preprocessing/EncoderUtil$1.class
+-rw-rw-r--  2.0 unx     4549 b- defN 23-Dec-04 22:17 sklearn/preprocessing/StandardScaler.class
+-rw-rw-r--  2.0 unx     9005 b- defN 23-Dec-04 22:17 sklearn/preprocessing/EncoderUtil.class
+-rw-rw-r--  2.0 unx     6350 b- defN 23-Dec-04 22:17 sklearn/preprocessing/PolynomialFeatures.class
+-rw-rw-r--  2.0 unx     8493 b- defN 23-Dec-04 22:17 sklearn/preprocessing/KBinsDiscretizer.class
+-rw-rw-r--  2.0 unx     4678 b- defN 23-Dec-04 22:17 sklearn/preprocessing/OneHotEncoder.class
+-rw-rw-r--  2.0 unx      729 b- defN 23-Dec-04 22:17 sklearn/preprocessing/EncoderUtil$4.class
+-rw-rw-r--  2.0 unx     2560 b- defN 23-Dec-04 22:17 sklearn/preprocessing/Binarizer.class
+-rw-rw-r--  2.0 unx     1054 b- defN 23-Dec-04 22:17 sklearn/preprocessing/EncoderUtil$2.class
+-rw-rw-r--  2.0 unx     3595 b- defN 23-Dec-04 22:17 sklearn/preprocessing/MinMaxScaler.class
+-rw-rw-r--  2.0 unx     4467 b- defN 23-Dec-04 22:17 sklearn/preprocessing/RobustScaler.class
+-rw-rw-r--  2.0 unx     3740 b- defN 23-Dec-04 22:17 sklearn/preprocessing/OrdinalEncoder.class
+-rw-rw-r--  2.0 unx      957 b- defN 23-Dec-04 22:17 sklearn/preprocessing/Imputer.class
+-rw-rw-r--  2.0 unx     2033 b- defN 23-Dec-04 22:17 sklearn/preprocessing/PolynomialFeatures$1.class
+-rw-rw-r--  2.0 unx    10333 b- defN 23-Dec-04 22:17 sklearn/preprocessing/MultiOneHotEncoder.class
+-rw-rw-r--  2.0 unx     2157 b- defN 23-Dec-04 22:17 sklearn/tree/TreeClassifier.class
+-rw-rw-r--  2.0 unx     3111 b- defN 23-Dec-04 22:17 sklearn/tree/TreeUtil$1.class
+-rw-rw-r--  2.0 unx     2664 b- defN 23-Dec-04 22:17 sklearn/tree/TreeUtil$4.class
+-rw-rw-r--  2.0 unx     4805 b- defN 23-Dec-04 22:17 sklearn/tree/visitors/TreeModelFlattener.class
+-rw-rw-r--  2.0 unx      739 b- defN 23-Dec-04 22:17 sklearn/tree/visitors/TreeModelCompactor$1.class
+-rw-rw-r--  2.0 unx     5431 b- defN 23-Dec-04 22:17 sklearn/tree/visitors/TreeModelCompactor.class
+-rw-rw-r--  2.0 unx     2988 b- defN 23-Dec-04 22:17 sklearn/tree/visitors/TreeModelPruner.class
+-rw-rw-r--  2.0 unx      739 b- defN 23-Dec-04 22:17 sklearn/tree/visitors/TreeModelFlattener$1.class
+-rw-rw-r--  2.0 unx      730 b- defN 23-Dec-04 22:17 sklearn/tree/visitors/TreeModelPruner$1.class
+-rw-rw-r--  2.0 unx      915 b- defN 23-Dec-04 22:17 sklearn/tree/RegressionCriterion.class
+-rw-rw-r--  2.0 unx     1151 b- defN 23-Dec-04 22:17 sklearn/tree/TreeUtil$5.class
+-rw-rw-r--  2.0 unx     1014 b- defN 23-Dec-04 22:17 sklearn/tree/PresortBestSplitter.class
+-rw-rw-r--  2.0 unx     1589 b- defN 23-Dec-04 22:17 sklearn/tree/TreeUtil$6.class
+-rw-rw-r--  2.0 unx     1771 b- defN 23-Dec-04 22:17 sklearn/tree/TreeRegressor.class
+-rw-rw-r--  2.0 unx     1489 b- defN 23-Dec-04 22:17 sklearn/tree/TreeUtil$7.class
+-rw-rw-r--  2.0 unx    19425 b- defN 23-Dec-04 22:17 sklearn/tree/TreeUtil.class
+-rw-rw-r--  2.0 unx     1123 b- defN 23-Dec-04 22:17 sklearn/tree/TreeUtil$3.class
+-rw-rw-r--  2.0 unx     1373 b- defN 23-Dec-04 22:17 sklearn/tree/HasTreeOptions.class
+-rw-rw-r--  2.0 unx     2293 b- defN 23-Dec-04 22:17 sklearn/tree/Tree.class
+-rw-rw-r--  2.0 unx      754 b- defN 23-Dec-04 22:17 sklearn/tree/TreeUtil$2.class
+-rw-rw-r--  2.0 unx      150 b- defN 23-Dec-04 22:17 sklearn/tree/HasTree.class
+-rw-rw-r--  2.0 unx     2547 b- defN 23-Dec-04 22:17 sklearn/InitializerUtil.class
+-rw-rw-r--  2.0 unx     2745 b- defN 23-Dec-04 22:17 sklearn/Regressor.class
+-rw-rw-r--  2.0 unx      211 b- defN 23-Dec-04 22:17 sklearn/HasNumberOfOutputs.class
+-rw-rw-r--  2.0 unx      534 b- defN 23-Dec-04 22:17 sklearn/OutlierDetector.class
+-rw-rw-r--  2.0 unx     3183 b- defN 23-Dec-04 22:17 sklearn/Calibrator.class
+-rw-rw-r--  2.0 unx      735 b- defN 23-Dec-04 22:17 sklearn/Composite$1.class
+-rw-rw-r--  2.0 unx      273 b- defN 23-Dec-04 22:17 sklearn/HasClassifierOptions.class
+-rw-rw-r--  2.0 unx     2309 b- defN 23-Dec-04 22:17 sklearn/CompositeRegressor.class
+-rw-rw-r--  2.0 unx     9083 b- defN 23-Dec-04 22:17 sklearn/EstimatorUtil.class
+-rw-rw-r--  2.0 unx      199 b- defN 23-Dec-04 22:17 sklearn/HasType.class
+-rw-rw-r--  2.0 unx     2417 b- defN 23-Dec-04 22:17 sklearn/CompositeClusterer.class
+-rw-rw-r--  2.0 unx      678 b- defN 23-Dec-04 22:17 sklearn/cluster/MiniBatchKMeans.class
+-rw-rw-r--  2.0 unx     5093 b- defN 23-Dec-04 22:17 sklearn/cluster/KMeans.class
+-rw-rw-r--  2.0 unx    14063 b- defN 23-Dec-04 22:17 sklearn/Estimator.class
+-rw-rw-r--  2.0 unx     1575 b- defN 23-Dec-04 22:17 sklearn/Initializer.class
+-rw-rw-r--  2.0 unx     4566 b- defN 23-Dec-04 22:17 sklearn/multiclass/OneVsRestClassifier.class
+-rw-rw-r--  2.0 unx     5157 b- defN 23-Dec-04 22:17 sklearn2pmml/ruleset/RuleSetClassifier.class
+-rw-rw-r--  2.0 unx      386 b- defN 23-Dec-04 22:17 sklearn2pmml/HasPMMLOptions.class
+-rw-rw-r--  2.0 unx     1187 b- defN 23-Dec-04 22:17 sklearn2pmml/pipeline/PMMLPipelineUtil$1.class
+-rw-rw-r--  2.0 unx      980 b- defN 23-Dec-04 22:17 sklearn2pmml/pipeline/PMMLPipeline$3.class
+-rw-rw-r--  2.0 unx      684 b- defN 23-Dec-04 22:17 sklearn2pmml/pipeline/PMMLPipeline$4.class
+-rw-rw-r--  2.0 unx    21565 b- defN 23-Dec-04 22:17 sklearn2pmml/pipeline/PMMLPipeline.class
+-rw-rw-r--  2.0 unx     1558 b- defN 23-Dec-04 22:17 sklearn2pmml/pipeline/PMMLPipeline$2.class
+-rw-rw-r--  2.0 unx     1460 b- defN 23-Dec-04 22:17 sklearn2pmml/pipeline/PMMLPipeline$1.class
+-rw-rw-r--  2.0 unx     1593 b- defN 23-Dec-04 22:17 sklearn2pmml/pipeline/PMMLPipelineUtil.class
+-rw-rw-r--  2.0 unx     1811 b- defN 23-Dec-04 22:17 sklearn2pmml/pipeline/Verification.class
+-rw-rw-r--  2.0 unx      313 b- defN 23-Dec-04 22:17 sklearn2pmml/HasPMMLName.class
+-rw-rw-r--  2.0 unx     2415 b- defN 23-Dec-04 22:17 sklearn2pmml/decoration/MultiDomain.class
+-rw-rw-r--  2.0 unx     1152 b- defN 23-Dec-04 22:17 sklearn2pmml/decoration/ContinuousDomainEraser.class
+-rw-rw-r--  2.0 unx     1654 b- defN 23-Dec-04 22:17 sklearn2pmml/decoration/Alias.class
+-rw-rw-r--  2.0 unx     1772 b- defN 23-Dec-04 22:17 sklearn2pmml/decoration/TemporalDomain.class
+-rw-rw-r--  2.0 unx      779 b- defN 23-Dec-04 22:17 sklearn2pmml/decoration/ContinuousDomain$1.class
+-rw-rw-r--  2.0 unx    11878 b- defN 23-Dec-04 22:17 sklearn2pmml/decoration/Domain.class
+-rw-rw-r--  2.0 unx     1416 b- defN 23-Dec-04 22:17 sklearn2pmml/decoration/MultiAlias.class
+-rw-rw-r--  2.0 unx     5055 b- defN 23-Dec-04 22:17 sklearn2pmml/decoration/DiscreteDomain.class
+-rw-rw-r--  2.0 unx     1952 b- defN 23-Dec-04 22:17 sklearn2pmml/decoration/CategoricalDomain.class
+-rw-rw-r--  2.0 unx     1717 b- defN 23-Dec-04 22:17 sklearn2pmml/decoration/DomainEraser.class
+-rw-rw-r--  2.0 unx      613 b- defN 23-Dec-04 22:17 sklearn2pmml/decoration/DateTimeDomain.class
+-rw-rw-r--  2.0 unx     7764 b- defN 23-Dec-04 22:17 sklearn2pmml/decoration/ContinuousDomain.class
+-rw-rw-r--  2.0 unx     1077 b- defN 23-Dec-04 22:17 sklearn2pmml/decoration/DiscreteDomainEraser.class
+-rw-rw-r--  2.0 unx     1590 b- defN 23-Dec-04 22:17 sklearn2pmml/decoration/TransformerWrapper.class
+-rw-rw-r--  2.0 unx     1045 b- defN 23-Dec-04 22:17 sklearn2pmml/decoration/Domain$2.class
+-rw-rw-r--  2.0 unx      596 b- defN 23-Dec-04 22:17 sklearn2pmml/decoration/DateDomain.class
+-rw-rw-r--  2.0 unx     2374 b- defN 23-Dec-04 22:17 sklearn2pmml/decoration/DomainUtil.class
+-rw-rw-r--  2.0 unx     1033 b- defN 23-Dec-04 22:17 sklearn2pmml/decoration/Domain$1.class
+-rw-rw-r--  2.0 unx     1577 b- defN 23-Dec-04 22:17 sklearn2pmml/decoration/OrdinalDomain.class
+-rw-rw-r--  2.0 unx      672 b- defN 23-Dec-04 22:17 sklearn2pmml/decoration/Domain$4.class
+-rw-rw-r--  2.0 unx      799 b- defN 23-Dec-04 22:17 sklearn2pmml/decoration/Domain$3.class
+-rw-rw-r--  2.0 unx     7879 b- defN 23-Dec-04 22:17 sklearn2pmml/neural_network/MLPTransformer.class
+-rw-rw-r--  2.0 unx      391 b- defN 23-Dec-04 22:17 sklearn2pmml/SkLearn2PMMLFields.class
+-rw-rw-r--  2.0 unx     1160 b- defN 23-Dec-04 22:17 sklearn2pmml/util/Evaluatable.class
+-rw-rw-r--  2.0 unx     1196 b- defN 23-Dec-04 22:17 sklearn2pmml/util/Expression.class
+-rw-rw-r--  2.0 unx     1189 b- defN 23-Dec-04 22:17 sklearn2pmml/util/Predicate.class
+-rw-rw-r--  2.0 unx      948 b- defN 23-Dec-04 22:17 sklearn2pmml/util/Reshaper.class
+-rw-rw-r--  2.0 unx     3392 b- defN 23-Dec-04 22:17 sklearn2pmml/util/EvaluatableUtil.class
+-rw-rw-r--  2.0 unx     1922 b- defN 23-Dec-04 22:17 sklearn2pmml/util/Slicer.class
+-rw-rw-r--  2.0 unx     2418 b- defN 23-Dec-04 22:17 sklearn2pmml/feature_extraction/text/Splitter.class
+-rw-rw-r--  2.0 unx     3184 b- defN 23-Dec-04 22:17 sklearn2pmml/feature_extraction/text/Matcher.class
+-rw-rw-r--  2.0 unx      343 b- defN 23-Dec-04 22:17 sklearn2pmml/HasPMMLSegmentId.class
+-rw-rw-r--  2.0 unx     1425 b- defN 23-Dec-04 22:17 sklearn2pmml/ensemble/SelectFirstRegressor.class
+-rw-rw-r--  2.0 unx     2083 b- defN 23-Dec-04 22:17 sklearn2pmml/ensemble/GBDTUtil$2.class
+-rw-rw-r--  2.0 unx      968 b- defN 23-Dec-04 22:17 sklearn2pmml/ensemble/HasEstimatorSteps.class
+-rw-rw-r--  2.0 unx     1934 b- defN 23-Dec-04 22:17 sklearn2pmml/ensemble/GBDTLMRegressor.class
+-rw-rw-r--  2.0 unx      948 b- defN 23-Dec-04 22:17 sklearn2pmml/ensemble/GBDTUtil$1.class
+-rw-rw-r--  2.0 unx     9003 b- defN 23-Dec-04 22:17 sklearn2pmml/ensemble/EstimatorChain.class
+-rw-rw-r--  2.0 unx     6001 b- defN 23-Dec-04 22:17 sklearn2pmml/ensemble/GBDTUtil.class
+-rw-rw-r--  2.0 unx     4588 b- defN 23-Dec-04 22:17 sklearn2pmml/ensemble/Link.class
+-rw-rw-r--  2.0 unx     4563 b- defN 23-Dec-04 22:17 sklearn2pmml/ensemble/SelectFirstUtil.class
+-rw-rw-r--  2.0 unx     6835 b- defN 23-Dec-04 22:17 sklearn2pmml/ensemble/OrdinalClassifier.class
+-rw-rw-r--  2.0 unx     4382 b- defN 23-Dec-04 22:17 sklearn2pmml/ensemble/GBDTLRClassifier.class
+-rw-rw-r--  2.0 unx     2594 b- defN 23-Dec-04 22:17 sklearn2pmml/ensemble/SelectFirstClassifier.class
+-rw-rw-r--  2.0 unx     1438 b- defN 23-Dec-04 22:17 sklearn2pmml/EstimatorProxy$1.class
+-rw-rw-r--  2.0 unx      946 b- defN 23-Dec-04 22:17 sklearn2pmml/feature_selection/SelectUnique.class
+-rw-rw-r--  2.0 unx     1836 b- defN 23-Dec-04 22:17 sklearn2pmml/cross_reference/Memorizer.class
+-rw-rw-r--  2.0 unx     2107 b- defN 23-Dec-04 22:17 sklearn2pmml/cross_reference/Recaller.class
+-rw-rw-r--  2.0 unx     6477 b- defN 23-Dec-04 22:17 sklearn2pmml/postprocessing/BusinessDecisionTransformer.class
+-rw-rw-r--  2.0 unx      791 b- defN 23-Dec-04 22:17 sklearn2pmml/postprocessing/BusinessDecisionTransformer$1.class
+-rw-rw-r--  2.0 unx     1197 b- defN 23-Dec-04 22:17 sklearn2pmml/preprocessing/PatternTransformer.class
+-rw-rw-r--  2.0 unx     2908 b- defN 23-Dec-04 22:17 sklearn2pmml/preprocessing/ReplaceTransformer.class
+-rw-rw-r--  2.0 unx     1865 b- defN 23-Dec-04 22:17 sklearn2pmml/preprocessing/WordCountTransformer.class
+-rw-rw-r--  2.0 unx      597 b- defN 23-Dec-04 22:17 sklearn2pmml/preprocessing/DateTimeFormatter.class
+-rw-rw-r--  2.0 unx     1288 b- defN 23-Dec-04 22:17 sklearn2pmml/preprocessing/PMMLLabelBinarizer.class
+-rw-rw-r--  2.0 unx     4621 b- defN 23-Dec-04 22:17 sklearn2pmml/preprocessing/DurationTransformer.class
+-rw-rw-r--  2.0 unx      444 b- defN 23-Dec-04 22:17 sklearn2pmml/preprocessing/PMMLLabelEncoder.class
+-rw-rw-r--  2.0 unx     2777 b- defN 23-Dec-04 22:17 sklearn2pmml/preprocessing/FilterLookupTransformer.class
+-rw-rw-r--  2.0 unx     2545 b- defN 23-Dec-04 22:17 sklearn2pmml/preprocessing/Formatter.class
+-rw-rw-r--  2.0 unx     3424 b- defN 23-Dec-04 22:17 sklearn2pmml/preprocessing/CastTransformer.class
+-rw-rw-r--  2.0 unx     2758 b- defN 23-Dec-04 22:17 sklearn2pmml/preprocessing/MatchesTransformer.class
+-rw-rw-r--  2.0 unx      589 b- defN 23-Dec-04 22:17 sklearn2pmml/preprocessing/NumberFormatter.class
+-rw-rw-r--  2.0 unx     4149 b- defN 23-Dec-04 22:17 sklearn2pmml/preprocessing/MultiLookupTransformer.class
+-rw-rw-r--  2.0 unx     3871 b- defN 23-Dec-04 22:17 sklearn2pmml/preprocessing/StringNormalizer.class
+-rw-rw-r--  2.0 unx     7145 b- defN 23-Dec-04 22:17 sklearn2pmml/preprocessing/ExpressionTransformer.class
+-rw-rw-r--  2.0 unx      635 b- defN 23-Dec-04 22:17 sklearn2pmml/preprocessing/DaysSinceYearTransformer.class
+-rw-rw-r--  2.0 unx     3604 b- defN 23-Dec-04 22:17 sklearn2pmml/preprocessing/DataFrameConstructor.class
+-rw-rw-r--  2.0 unx     2847 b- defN 23-Dec-04 22:17 sklearn2pmml/preprocessing/ConcatTransformer.class
+-rw-rw-r--  2.0 unx     7099 b- defN 23-Dec-04 22:17 sklearn2pmml/preprocessing/CutTransformer.class
+-rw-rw-r--  2.0 unx     7025 b- defN 23-Dec-04 22:17 sklearn2pmml/preprocessing/BSplineTransformer.class
+-rw-rw-r--  2.0 unx     6410 b- defN 23-Dec-04 22:17 sklearn2pmml/preprocessing/LookupTransformer.class
+-rw-rw-r--  2.0 unx     3236 b- defN 23-Dec-04 22:17 sklearn2pmml/preprocessing/SubstringTransformer.class
+-rw-rw-r--  2.0 unx     3181 b- defN 23-Dec-04 22:17 sklearn2pmml/preprocessing/SecondsSinceMidnightTransformer.class
+-rw-rw-r--  2.0 unx     4665 b- defN 23-Dec-04 22:17 sklearn2pmml/preprocessing/SelectFirstTransformer.class
+-rw-rw-r--  2.0 unx     2132 b- defN 23-Dec-04 22:17 sklearn2pmml/preprocessing/PowerFunctionTransformer.class
+-rw-rw-r--  2.0 unx     3328 b- defN 23-Dec-04 22:17 sklearn2pmml/preprocessing/Aggregator.class
+-rw-rw-r--  2.0 unx      647 b- defN 23-Dec-04 22:17 sklearn2pmml/preprocessing/SecondsSinceYearTransformer.class
+-rw-rw-r--  2.0 unx     1639 b- defN 23-Dec-04 22:17 sklearn2pmml/tree/CHAIDRegressor.class
+-rw-rw-r--  2.0 unx    10719 b- defN 23-Dec-04 22:17 sklearn2pmml/tree/CHAIDUtil.class
+-rw-rw-r--  2.0 unx     2029 b- defN 23-Dec-04 22:17 sklearn2pmml/tree/CHAIDClassifier.class
+-rw-rw-r--  2.0 unx     1417 b- defN 23-Dec-04 22:17 sklearn2pmml/tree/CHAIDUtil$1.class
+-rw-rw-r--  2.0 unx     5967 b- defN 23-Dec-04 22:17 sklearn2pmml/EstimatorProxy.class
+-rw-rw-r--  2.0 unx     1479 b- defN 23-Dec-04 22:17 sklearn2pmml/SelectorProxy.class
+-rw-rw-r--  2.0 unx     2046 b- defN 23-Dec-04 22:17 sklearn2pmml/expression/ExpressionUtil.class
+-rw-rw-r--  2.0 unx     3799 b- defN 23-Dec-04 22:17 sklearn2pmml/expression/ExpressionRegressor.class
+-rw-rw-r--  2.0 unx      990 b- defN 23-Dec-04 22:17 sklearn2pmml/expression/ExpressionClassifier$1.class
+-rw-rw-r--  2.0 unx     8684 b- defN 23-Dec-04 22:17 sklearn2pmml/expression/ExpressionClassifier.class
+-rw-rw-r--  2.0 unx      948 b- defN 23-Dec-04 22:17 sklearn2pmml/expression/ExpressionUtil$1.class
+-rw-rw-r--  2.0 unx      162 b- defN 23-Dec-04 22:17 org/jpmml/sklearn/Encodable.class
+-rw-rw-r--  2.0 unx     1774 b- defN 23-Dec-04 22:17 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest$1.class
+-rw-rw-r--  2.0 unx     2913 b- defN 23-Dec-04 22:17 org/jpmml/sklearn/testing/SkLearnEncoderBatch.class
+-rw-rw-r--  2.0 unx     3549 b- defN 23-Dec-04 22:17 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest.class
+-rw-rw-r--  2.0 unx    17846 b- defN 23-Dec-04 22:17 org/jpmml/sklearn/SkLearnEncoder.class
+-rw-rw-r--  2.0 unx     3123 b- defN 23-Dec-04 22:17 org/jpmml/sklearn/EncodableUtil.class
+-rw-rw-r--  2.0 unx     1569 b- defN 23-Dec-04 22:17 org/jpmml/sklearn/IfElseBuilder.class
+-rw-rw-r--  2.0 unx      194 b- defN 23-Dec-04 22:17 org/jpmml/sklearn/FieldNames.class
+-rw-rw-r--  2.0 unx      171 b- defN 23-Dec-04 22:17 org/jpmml/sklearn/HasSkLearnOptions.class
+-rw-rw-r--  2.0 unx      664 b- defN 23-Dec-04 22:17 org/jpmml/sklearn/SkLearnUtil.class
+-rw-rw-r--  2.0 unx     1179 b- defN 23-Dec-04 22:17 org/jpmml/sklearn/SkLearnEncoder$1.class
+-rw-rw-r--  2.0 unx     1859 b- defN 23-Dec-04 22:16 META-INF/maven/org.jpmml/pmml-sklearn/pom.xml
+-rw-rw-r--  2.0 unx       57 b- defN 23-Dec-04 22:17 META-INF/maven/org.jpmml/pmml-sklearn/pom.properties
+430 files, 986655 bytes uncompressed, 434323 bytes compressed:  56.0%
```

#### zipnote «TEMP»/diffoscope_wqp9k9w__/tmpnvtoe6gm_.zip

```diff
@@ -957,14 +957,20 @@
 
 Filename: sklearn2pmml/HasPMMLOptions.class
 Comment: 
 
 Filename: sklearn2pmml/pipeline/PMMLPipelineUtil$1.class
 Comment: 
 
+Filename: sklearn2pmml/pipeline/PMMLPipeline$3.class
+Comment: 
+
+Filename: sklearn2pmml/pipeline/PMMLPipeline$4.class
+Comment: 
+
 Filename: sklearn2pmml/pipeline/PMMLPipeline.class
 Comment: 
 
 Filename: sklearn2pmml/pipeline/PMMLPipeline$2.class
 Comment: 
 
 Filename: sklearn2pmml/pipeline/PMMLPipeline$1.class
@@ -1257,14 +1263,17 @@
 
 Filename: org/jpmml/sklearn/SkLearnEncoder.class
 Comment: 
 
 Filename: org/jpmml/sklearn/EncodableUtil.class
 Comment: 
 
+Filename: org/jpmml/sklearn/IfElseBuilder.class
+Comment: 
+
 Filename: org/jpmml/sklearn/FieldNames.class
 Comment: 
 
 Filename: org/jpmml/sklearn/HasSkLearnOptions.class
 Comment: 
 
 Filename: org/jpmml/sklearn/SkLearnUtil.class
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,6 @@
 Manifest-Version: 1.0
 Implementation-Title: JPMML-SkLearn library
-Implementation-Version: 1.7.41
+Implementation-Version: 1.7.42
 Build-Jdk-Spec: 1.8
 Created-By: Maven JAR Plugin 3.3.0
```

#### sklearn2pmml/pipeline/PMMLPipeline.class

##### procyon -ec {}

```diff
@@ -2,18 +2,21 @@
 package sklearn2pmml.pipeline;
 
 import org.slf4j.LoggerFactory;
 import com.google.common.base.Function;
 import com.google.common.collect.Lists;
 import sklearn.Step;
 import numpy.core.NDArrayUtil;
+import org.dmg.pmml.Field;
 import org.dmg.pmml.DefineFunction;
-import org.dmg.pmml.ResultFeature;
+import java.util.Comparator;
 import org.jpmml.converter.DerivedOutputField;
 import org.dmg.pmml.DerivedField;
+import org.dmg.pmml.Expression;
+import org.dmg.pmml.ResultFeature;
 import org.dmg.pmml.Header;
 import org.jpmml.converter.PMMLUtil;
 import org.dmg.pmml.Extension;
 import org.dmg.pmml.MiningBuildTask;
 import java.util.Iterator;
 import org.dmg.pmml.Output;
 import org.jpmml.converter.Label;
@@ -173,15 +176,15 @@
                     final int[] targetValuesShape = verification.getTargetValuesShape();
                     ClassDictUtil.checkShapes(0, new int[][] { activeValuesShape, targetValuesShape });
                     ClassDictUtil.checkSize(new Collection[] { targetFields, scalarLabels2 });
                     for (int l = 0; l < targetFields.size(); ++l) {
                         final VerificationField verificationField3 = ModelUtil.createVerificationField((String)targetFields.get(l));
                         final ScalarLabel scalarLabel3 = (ScalarLabel)scalarLabels2.get(l);
                         final DataType dataType = scalarLabel3.getDataType();
-                        switch (PMMLPipeline.PMMLPipeline$2.$SwitchMap$org$dmg$pmml$DataType[dataType.ordinal()]) {
+                        switch (PMMLPipeline.PMMLPipeline$4.$SwitchMap$org$dmg$pmml$DataType[dataType.ordinal()]) {
                             case 1:
                             case 2: {
                                 verificationField3.setPrecision(precision).setZeroThreshold(zeroThreshold);
                                 break;
                             }
                         }
                         final Domain domain2 = encoder.getDomain(verificationField3.requireField());
@@ -206,39 +209,53 @@
             final MiningBuildTask miningBuildTask = new MiningBuildTask().addExtensions(new Extension[] { PMMLUtil.createExtension("repr", new Object[] { repr }) });
             pmml.setMiningBuildTask(miningBuildTask);
         }
         return pmml;
     }
     
     private void encodeOutput(final Output output, final List<OutputField> outputFields, final Transformer transformer, final SkLearnEncoder encoder) {
-        final SkLearnEncoder outputEncoder = new SkLearnEncoder();
+        final SkLearnEncoder outputEncoder = (SkLearnEncoder)new PMMLPipeline.PMMLPipeline$1(this, encoder);
         final Model model = encoder.getModel();
         if (model != null) {
             outputEncoder.setModel(model);
         }
         final List<Feature> features = new ArrayList<Feature>();
         for (final OutputField outputField : outputFields) {
             final DataField dataField = outputEncoder.createDataField(outputField.requireName(), outputField.requireOpType(), outputField.requireDataType());
             features.add((Feature)new WildcardFeature((PMMLEncoder)outputEncoder, dataField));
         }
-        transformer.encode((List)features, outputEncoder);
+        final List<Feature> outputFeatures = transformer.encode((List)features, outputEncoder);
+        final Map<String, Integer> finalResults = new LinkedHashMap<String, Integer>();
+        for (final Feature outputFeature : outputFeatures) {
+            final String name = outputFeature.getName();
+            final Field<?> field = (Field<?>)outputFeature.getField();
+            try {
+                outputEncoder.getField(field.requireName());
+            }
+            catch (final IllegalArgumentException iae) {
+                final OutputField outputField2 = new OutputField(FieldNameUtil.create("xref", new Object[] { outputFeature }), field.requireOpType(), field.requireDataType()).setResultFeature(ResultFeature.TRANSFORMED_VALUE).setFinalResult(Boolean.valueOf(true)).setExpression((Expression)outputFeature.ref());
+                output.addOutputFields(new OutputField[] { outputField2 });
+            }
+            finalResults.put(name, Integer.valueOf(finalResults.size()));
+        }
         final Collection<DerivedField> derivedFields = outputEncoder.getDerivedFields().values();
-        final Iterator<DerivedField> it = derivedFields.iterator();
-        while (it.hasNext()) {
-            final DerivedField derivedField = (DerivedField)it.next();
-            OutputField outputField2;
+        for (final DerivedField derivedField : derivedFields) {
+            OutputField outputField3;
             if (derivedField instanceof DerivedOutputField) {
                 final DerivedOutputField derivedOutputField = (DerivedOutputField)derivedField;
-                outputField2 = derivedOutputField.getOutputField();
+                outputField3 = derivedOutputField.getOutputField();
             }
             else {
-                outputField2 = new OutputField(derivedField.requireName(), derivedField.requireOpType(), derivedField.requireDataType()).setResultFeature(ResultFeature.TRANSFORMED_VALUE).setFinalResult(Boolean.valueOf(!it.hasNext())).setExpression(derivedField.requireExpression());
+                final String name2 = derivedField.requireName();
+                outputField3 = new OutputField(name2, derivedField.requireOpType(), derivedField.requireDataType()).setResultFeature(ResultFeature.TRANSFORMED_VALUE).setFinalResult(Boolean.valueOf(finalResults.containsKey((Object)name2))).setExpression(derivedField.requireExpression());
             }
-            output.addOutputFields(new OutputField[] { outputField2 });
+            output.addOutputFields(new OutputField[] { outputField3 });
         }
+        final Comparator<OutputField> comparator = (Comparator<OutputField>)new PMMLPipeline.PMMLPipeline$2(this, (Map)finalResults);
+        Collections.sort((List<Object>)output.getOutputFields(), (Comparator<? super Object>)comparator);
         final Map<String, DefineFunction> defineFunctions = outputEncoder.getDefineFunctions();
         for (final DefineFunction defineFunction : defineFunctions.values()) {
             encoder.addDefineFunction(defineFunction);
         }
     }
     
     public List<Object[]> getSteps() {
@@ -355,15 +372,15 @@
         for (final Object value : values) {
             probabilityFields.add(FieldNameUtil.create("probability", new Object[] { value }));
         }
         return probabilityFields;
     }
     
     private static List<?> cleanValues(final Domain domain, final List<?> values) {
-        final Function<Object, Object> function = (Function<Object, Object>)new PMMLPipeline.PMMLPipeline$1();
+        final Function<Object, Object> function = (Function<Object, Object>)new PMMLPipeline.PMMLPipeline$3();
         return Lists.transform((List)values, (Function)function);
     }
     
     static {
         logger = LoggerFactory.getLogger((Class)PMMLPipeline.class);
     }
 }
```

#### sklearn2pmml/pipeline/PMMLPipeline$2.class

##### procyon -ec {}

```diff
@@ -1,5 +1,15 @@
 
 package sklearn2pmml.pipeline;
 
-import org.dmg.pmml.DataType;
+import java.util.Map;
+import org.dmg.pmml.OutputField;
+import java.util.Comparator;
 
+class PMMLPipeline$2 implements Comparator<OutputField> {
+    @Override
+    public int compare(final OutputField left, final OutputField right) {
+        final int leftIndex = (int)Integer.valueOf(this.val$finalResults.getOrDefault((Object)left.requireName(), Integer.valueOf(-1)));
+        final int rightIndex = (int)Integer.valueOf(this.val$finalResults.getOrDefault((Object)right.requireName(), Integer.valueOf(-1)));
+        return Integer.compare(leftIndex, rightIndex);
+    }
+}
```

#### sklearn2pmml/pipeline/PMMLPipeline$1.class

##### procyon -ec {}

```diff
@@ -1,16 +1,26 @@
 
 package sklearn2pmml.pipeline;
 
-import org.jpmml.converter.ValueUtil;
+import org.jpmml.converter.Feature;
 import sklearn2pmml.decoration.Domain;
-import com.google.common.base.Function;
+import java.util.Map;
+import org.dmg.pmml.Model;
+import org.jpmml.sklearn.SkLearnEncoder;
 
-static final class PMMLPipeline$1 implements Function<Object, Object> {
-    public Object apply(final Object value) {
-        Domain.checkValue(value);
-        if (ValueUtil.isNaN(value)) {
-            return null;
-        }
-        return value;
+class PMMLPipeline$1 extends SkLearnEncoder {
+    public void addTransformer(final Model transformer) {
+        throw new UnsupportedOperationException();
+    }
+    
+    public boolean isFrozen(final String name) {
+        return true;
+    }
+    
+    public Map<String, Domain> getDomains() {
+        throw new UnsupportedOperationException();
+    }
+    
+    public Map<String, Feature> getMemory() {
+        return this.val$encoder.getMemory();
     }
 }
```

#### sklearn2pmml/preprocessing/SelectFirstTransformer.class

##### procyon -ec {}

```diff
@@ -1,26 +1,26 @@
 
 package sklearn2pmml.preprocessing;
 
 import org.dmg.pmml.DerivedField;
+import org.dmg.pmml.Apply;
 import org.dmg.pmml.OpType;
 import java.util.Set;
-import org.dmg.pmml.Apply;
 import org.jpmml.python.Scope;
 import org.jpmml.converter.PMMLEncoder;
 import org.dmg.pmml.Field;
 import org.jpmml.converter.FeatureUtil;
 import org.jpmml.converter.TypeUtil;
+import org.dmg.pmml.Expression;
 import java.util.Collections;
-import org.jpmml.converter.PMMLUtil;
 import sklearn2pmml.util.EvaluatableUtil;
-import org.dmg.pmml.Expression;
 import org.jpmml.python.TupleUtil;
 import java.util.EnumSet;
 import org.dmg.pmml.DataType;
+import org.jpmml.sklearn.IfElseBuilder;
 import org.jpmml.python.DataFrameScope;
 import com.google.common.collect.Iterables;
 import org.jpmml.python.ClassDictUtil;
 import java.util.Collection;
 import org.jpmml.sklearn.SkLearnEncoder;
 import org.jpmml.converter.Feature;
 import java.util.List;
@@ -41,38 +41,31 @@
         ClassDictUtil.checkSize(1, new Collection[] { features });
         final Feature feature = (Feature)Iterables.getOnlyElement((Iterable)features);
         List<Feature> controlFeatures = features;
         if (controller != null) {
             controlFeatures = controller.encode((List)controlFeatures, encoder);
         }
         final Scope scope = (Scope)new DataFrameScope("X", (List)controlFeatures);
-        Apply apply = null;
-        Apply prevIfApply = null;
+        final IfElseBuilder applyBuilder = new IfElseBuilder();
         final Set<DataType> dataTypes = EnumSet.noneOf(DataType.class);
         for (int i = 0; i < steps.size(); ++i) {
             final Object[] step = (Object[])steps.get(i);
             final String name = (String)TupleUtil.extractElement(step, 0, (Class)String.class);
             final Transformer transformer = (Transformer)TupleUtil.extractElement(step, 1, (Class)Transformer.class);
             final Object expr = TupleUtil.extractElement(step, 2, (Class)Object.class);
-            final Apply ifApply = PMMLUtil.createApply("if", new Expression[] { EvaluatableUtil.translateExpression(expr, scope) });
+            final Expression expression = EvaluatableUtil.translateExpression(expr, scope);
             final List<Feature> stepFeatures = transformer.encode((List)Collections.singletonList(feature), encoder);
             ClassDictUtil.checkSize(1, new Collection[] { stepFeatures });
             final Feature stepFeature = (Feature)Iterables.getOnlyElement((Iterable)stepFeatures);
-            ifApply.addExpressions(new Expression[] { (Expression)stepFeature.ref() });
+            applyBuilder.add(expression, (Expression)stepFeature.ref());
             dataTypes.add(stepFeature.getDataType());
-            if (apply == null) {
-                apply = ifApply;
-            }
-            if (prevIfApply != null) {
-                prevIfApply.addExpressions(new Expression[] { (Expression)ifApply });
-            }
-            prevIfApply = ifApply;
         }
         final DataType dataType = (DataType)Iterables.getOnlyElement((Iterable)dataTypes);
         final OpType opType = TypeUtil.getOpType(dataType);
+        final Apply apply = applyBuilder.build();
         final DerivedField derivedField = encoder.createDerivedField(this.createFieldName("selectFirst", new Object[] { feature }), opType, dataType, (Expression)apply);
         return Collections.singletonList(FeatureUtil.createFeature((Field)derivedField, (PMMLEncoder)encoder));
     }
     
     public Transformer getController() {
         return (Transformer)this.getOptional("controller", (Class)Transformer.class);
     }
```

#### org/jpmml/sklearn/SkLearnEncoder.class

##### procyon -ec {}

```diff
@@ -156,15 +156,22 @@
             result.add(feature);
             outputFields.removeAll(nameOutputFields);
         }
         return result;
     }
     
     public Feature exportPrediction(final Model model, final ScalarLabel scalarLabel) {
-        return this.exportPrediction(model, FieldNameUtil.create("predict", new Object[] { scalarLabel.getName() }), scalarLabel);
+        String name;
+        if (scalarLabel.isAnonymous()) {
+            name = "predict";
+        }
+        else {
+            name = FieldNameUtil.create("predict", new Object[] { scalarLabel.getName() });
+        }
+        return this.exportPrediction(model, name, scalarLabel);
     }
     
     public Feature exportPrediction(final Model model, final String name, final ScalarLabel scalarLabel) {
         final OutputField outputField = ModelUtil.createPredictedField(name, scalarLabel.getOpType(), scalarLabel.getDataType()).setFinalResult(Boolean.valueOf(false));
         final DerivedOutputField derivedOutputField = this.createDerivedField(model, outputField, false);
         return derivedOutputField.toFeature((PMMLEncoder)this);
     }
@@ -222,30 +229,37 @@
             final Feature feature = (Feature)features.get(i);
             final String renamedName = (String)renamedNames.get(i);
             this.renameFeature(feature, renamedName);
         }
     }
     
     public boolean isFrozen(final String name) {
-        return this.domains.containsKey(name);
+        final Map<String, Domain> domains = this.getDomains();
+        return domains.containsKey(name);
     }
     
     public Domain getDomain(final String name) {
-        return this.domains.get(name);
+        final Map<String, Domain> domains = this.getDomains();
+        return domains.get(name);
     }
     
     public void setDomain(final String name, final Domain domain) {
+        final Map<String, Domain> domains = this.getDomains();
         if (domain != null) {
-            this.domains.put(name, domain);
+            domains.put(name, domain);
         }
         else {
-            this.domains.remove(name);
+            domains.remove(name);
         }
     }
     
+    public Map<String, Domain> getDomains() {
+        return this.domains;
+    }
+    
     public Label getLabel() {
         return this.label;
     }
     
     public void setLabel(final Label label) {
         this.label = label;
     }
@@ -255,19 +269,25 @@
     }
     
     public void setFeatures(final List<? extends Feature> features) {
         this.features = Objects.requireNonNull(features);
     }
     
     public void memorize(final String name, final Feature feature) {
-        this.memory.put(name, feature);
+        final Map<String, Feature> memory = this.getMemory();
+        memory.put(name, feature);
     }
     
     public Feature recall(final String name) {
-        return this.memory.get(name);
+        final Map<String, Feature> memory = this.getMemory();
+        return memory.get(name);
+    }
+    
+    public Map<String, Feature> getMemory() {
+        return this.memory;
     }
     
     public Predicate getPredicate() {
         return this.predicate;
     }
     
     public void setPredicate(final Predicate predicate) {
```

#### org/jpmml/sklearn/SkLearnEncoder$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum f5c98f289cd97aa643259379fa1c7d735eea91bb4768f8e6e159bae277ac0f6c
+  SHA-256 checksum 93bfb9987ebb963a096c3f3841a2a65570dc02b82e48ff18eabc3aa523632722
   Compiled from "SkLearnEncoder.java"
 class org.jpmml.sklearn.SkLearnEncoder$1
   minor version: 0
   major version: 52
   flags: (0x1020) ACC_SUPER, ACC_SYNTHETIC
   this_class: #12                         // org/jpmml/sklearn/SkLearnEncoder$1
   super_class: #13                        // java/lang/Object
@@ -121,15 +121,15 @@
       Exception table:
          from    to  target type
              9    20    23   Class java/lang/NoSuchFieldError
             24    35    38   Class java/lang/NoSuchFieldError
             39    50    53   Class java/lang/NoSuchFieldError
             63    74    77   Class java/lang/NoSuchFieldError
       LineNumberTable:
-        line 366: 0
+        line 393: 0
         line 112: 54
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
       StackMapTable: number_of_entries = 8
         frame_type = 87 /* same_locals_1_stack_item */
           stack = [ class java/lang/NoSuchFieldError ]
         frame_type = 0 /* same */
```

#### META-INF/maven/org.jpmml/pmml-sklearn/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.41</version>
+    <version>1.7.42</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn converter</name>
   <description>JPMML Scikit-Learn to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn/pom.properties

```diff
@@ -1,3 +1,3 @@
 artifactId=pmml-sklearn
 groupId=org.jpmml
-version=1.7.41
+version=1.7.42
```

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.41.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.42.jar`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 8815 bytes, number of entries: 18
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Oct-23 22:44 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 h2o/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 h2o/utils/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 h2o/utils/metaclass/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 h2o/estimators/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn2pmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn2pmml/preprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn2pmml/preprocessing/h2o/
--rw-rw-r--  2.0 unx      748 b- defN 23-Oct-23 22:44 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx     1049 b- defN 23-Oct-23 22:44 h2o/utils/metaclass/H2OMetaConstructor.class
--rw-rw-r--  2.0 unx     9221 b- defN 23-Oct-23 22:44 h2o/estimators/H2OEstimator.class
--rw-rw-r--  2.0 unx     1958 b- defN 23-Oct-23 22:44 sklearn2pmml/preprocessing/h2o/H2OFrameConstructor.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Oct-23 22:44 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Oct-23 22:44 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Oct-23 22:44 META-INF/maven/org.jpmml/pmml-sklearn-h2o/
--rw-rw-r--  2.0 unx     1305 b- defN 23-Oct-23 22:44 META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.xml
--rw-rw-r--  2.0 unx      112 b- defN 23-Oct-23 22:44 META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.properties
-18 files, 14523 bytes uncompressed, 6423 bytes compressed:  55.8%
+Zip file size: 8812 bytes, number of entries: 18
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Dec-04 22:17 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 h2o/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 h2o/utils/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 h2o/utils/metaclass/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 h2o/estimators/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn2pmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn2pmml/preprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn2pmml/preprocessing/h2o/
+-rw-rw-r--  2.0 unx      748 b- defN 23-Dec-04 22:17 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx     1049 b- defN 23-Dec-04 22:17 h2o/utils/metaclass/H2OMetaConstructor.class
+-rw-rw-r--  2.0 unx     9221 b- defN 23-Dec-04 22:17 h2o/estimators/H2OEstimator.class
+-rw-rw-r--  2.0 unx     1958 b- defN 23-Dec-04 22:17 sklearn2pmml/preprocessing/h2o/H2OFrameConstructor.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Dec-04 22:17 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Dec-04 22:17 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Dec-04 22:17 META-INF/maven/org.jpmml/pmml-sklearn-h2o/
+-rw-rw-r--  2.0 unx     1305 b- defN 23-Dec-04 22:16 META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.xml
+-rw-rw-r--  2.0 unx      111 b- defN 23-Dec-04 22:17 META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.properties
+18 files, 14522 bytes uncompressed, 6420 bytes compressed:  55.8%
```

#### META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.41</version>
+    <version>1.7.42</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-h2o</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn H2O.ai converter</name>
   <description>JPMML Scikit-Learn H2O.ai to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Mon Oct 23 22:44:50 EEST 2023
-version=1.7.41
+#Mon Dec 04 22:17:23 EET 2023
+version=1.7.42
 groupId=org.jpmml
 artifactId=pmml-sklearn-h2o
```

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/slf4j-api-1.7.36.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/slf4j-api-1.7.36.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/pmml-h2o-1.2.9.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/pmml-h2o-1.2.9.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/jackson-annotations-2.13.3.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/jackson-annotations-2.13.3.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/jcommander-1.72.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/jcommander-1.72.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/pmml-converter-1.5.5.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/pmml-converter-1.5.5.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/pmml-lightgbm-1.4.6.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/pmml-lightgbm-1.4.6.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/pmml-sklearn-extension-1.7.41.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/pmml-sklearn-extension-1.7.42.jar`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,73 +1,73 @@
-Zip file size: 88591 bytes, number of entries: 71
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Oct-23 22:44 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 pycaret/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 pycaret/pipeline/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 pycaret/preprocess/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 tpot/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 tpot/builtins/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 boruta/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 optbinning/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 optbinning/scorecard/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 imblearn/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 imblearn/pipeline/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 category_encoders/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklego/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklego/meta/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 hpsklearn/
--rw-rw-r--  2.0 unx     4458 b- defN 23-Oct-23 22:44 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx     5202 b- defN 23-Oct-23 22:44 pycaret/pipeline/PyCaretPipeline.class
--rw-rw-r--  2.0 unx      412 b- defN 23-Oct-23 22:44 pycaret/preprocess/FixImbalancer.class
--rw-rw-r--  2.0 unx     2980 b- defN 23-Oct-23 22:44 pycaret/preprocess/RemoveMulticollinearity.class
--rw-rw-r--  2.0 unx      421 b- defN 23-Oct-23 22:44 pycaret/preprocess/CleanColumnNames.class
--rw-rw-r--  2.0 unx     1332 b- defN 23-Oct-23 22:44 pycaret/preprocess/RemoveOutliers$1.class
--rw-rw-r--  2.0 unx     2898 b- defN 23-Oct-23 22:44 pycaret/preprocess/RareCategoryGrouping.class
--rw-rw-r--  2.0 unx     3125 b- defN 23-Oct-23 22:44 pycaret/preprocess/RemoveOutliers.class
--rw-rw-r--  2.0 unx     8009 b- defN 23-Oct-23 22:44 pycaret/preprocess/TransformerWrapper.class
--rw-rw-r--  2.0 unx     4170 b- defN 23-Oct-23 22:44 pycaret/preprocess/TransformerWrapperWithInverse.class
--rw-rw-r--  2.0 unx      720 b- defN 23-Oct-23 22:44 tpot/builtins/StackingEstimator$1.class
--rw-rw-r--  2.0 unx     4050 b- defN 23-Oct-23 22:44 tpot/builtins/StackingEstimator.class
--rw-rw-r--  2.0 unx      698 b- defN 23-Oct-23 22:44 boruta/BorutaPy.class
--rw-rw-r--  2.0 unx     2433 b- defN 23-Oct-23 22:44 optbinning/BinnedFeature.class
--rw-rw-r--  2.0 unx     9558 b- defN 23-Oct-23 22:44 optbinning/scorecard/Scorecard.class
--rw-rw-r--  2.0 unx     2133 b- defN 23-Oct-23 22:44 optbinning/OptimalBinningUtil.class
--rw-rw-r--  2.0 unx     6372 b- defN 23-Oct-23 22:44 optbinning/BinningProcess.class
--rw-rw-r--  2.0 unx     2274 b- defN 23-Oct-23 22:44 optbinning/ContinuousOptimalBinning.class
--rw-rw-r--  2.0 unx     3917 b- defN 23-Oct-23 22:44 optbinning/MulticlassOptimalBinning.class
--rw-rw-r--  2.0 unx     1240 b- defN 23-Oct-23 22:44 optbinning/BinningProcess$1.class
--rw-rw-r--  2.0 unx    14050 b- defN 23-Oct-23 22:44 optbinning/OptimalBinning.class
--rw-rw-r--  2.0 unx      424 b- defN 23-Oct-23 22:44 imblearn/pipeline/ImbLearnPipeline.class
--rw-rw-r--  2.0 unx      374 b- defN 23-Oct-23 22:44 imblearn/Sampler.class
--rw-rw-r--  2.0 unx     1916 b- defN 23-Oct-23 22:44 category_encoders/MapEncoder.class
--rw-rw-r--  2.0 unx     8449 b- defN 23-Oct-23 22:44 category_encoders/MapFeature.class
--rw-rw-r--  2.0 unx      527 b- defN 23-Oct-23 22:44 category_encoders/TargetEncoder.class
--rw-rw-r--  2.0 unx     1451 b- defN 23-Oct-23 22:44 category_encoders/CountEncoder$1.class
--rw-rw-r--  2.0 unx      515 b- defN 23-Oct-23 22:44 category_encoders/WOEEncoder.class
--rw-rw-r--  2.0 unx     8474 b- defN 23-Oct-23 22:44 category_encoders/MeanEncoder.class
--rw-rw-r--  2.0 unx     8520 b- defN 23-Oct-23 22:44 category_encoders/CountEncoder.class
--rw-rw-r--  2.0 unx    12815 b- defN 23-Oct-23 22:44 category_encoders/BaseNFeature.class
--rw-rw-r--  2.0 unx     1481 b- defN 23-Oct-23 22:44 category_encoders/OrdinalMapEncoder$1.class
--rw-rw-r--  2.0 unx     1445 b- defN 23-Oct-23 22:44 category_encoders/MeanEncoder$1.class
--rw-rw-r--  2.0 unx     2119 b- defN 23-Oct-23 22:44 category_encoders/OrdinalEncoder$Mapping.class
--rw-rw-r--  2.0 unx     1323 b- defN 23-Oct-23 22:44 category_encoders/LeaveOneOutEncoder$1.class
--rw-rw-r--  2.0 unx     8108 b- defN 23-Oct-23 22:44 category_encoders/OrdinalMapEncoder.class
--rw-rw-r--  2.0 unx     9241 b- defN 23-Oct-23 22:44 category_encoders/BaseNEncoder.class
--rw-rw-r--  2.0 unx     1334 b- defN 23-Oct-23 22:44 category_encoders/BinaryEncoder.class
--rw-rw-r--  2.0 unx     3547 b- defN 23-Oct-23 22:44 category_encoders/OneHotEncoder.class
--rw-rw-r--  2.0 unx     1325 b- defN 23-Oct-23 22:44 category_encoders/CatBoostEncoder.class
--rw-rw-r--  2.0 unx     2062 b- defN 23-Oct-23 22:44 category_encoders/CategoryEncoderUtil.class
--rw-rw-r--  2.0 unx     1564 b- defN 23-Oct-23 22:44 category_encoders/OrdinalEncoder$1.class
--rw-rw-r--  2.0 unx     1047 b- defN 23-Oct-23 22:44 category_encoders/LeaveOneOutEncoder.class
--rw-rw-r--  2.0 unx     4690 b- defN 23-Oct-23 22:44 category_encoders/OrdinalEncoder.class
--rw-rw-r--  2.0 unx      742 b- defN 23-Oct-23 22:44 category_encoders/MeanEncoder$MeanFunction.class
--rw-rw-r--  2.0 unx     1378 b- defN 23-Oct-23 22:44 category_encoders/CatBoostEncoder$1.class
--rw-rw-r--  2.0 unx     2162 b- defN 23-Oct-23 22:44 category_encoders/CategoryEncoder.class
--rw-rw-r--  2.0 unx     6139 b- defN 23-Oct-23 22:44 sklego/meta/EstimatorTransformer.class
--rw-rw-r--  2.0 unx     1259 b- defN 23-Oct-23 22:44 hpsklearn/HyperoptEstimator$1.class
--rw-rw-r--  2.0 unx     3750 b- defN 23-Oct-23 22:44 hpsklearn/HyperoptEstimator.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Oct-23 22:44 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Oct-23 22:44 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Oct-23 22:44 META-INF/maven/org.jpmml/pmml-sklearn-extension/
--rw-rw-r--  2.0 unx     1226 b- defN 23-Oct-23 22:44 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml
--rw-rw-r--  2.0 unx      118 b- defN 23-Oct-23 22:44 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.properties
-71 files, 180107 bytes uncompressed, 78559 bytes compressed:  56.4%
+Zip file size: 88622 bytes, number of entries: 71
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Dec-04 22:17 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 pycaret/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 pycaret/pipeline/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 pycaret/preprocess/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 tpot/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 tpot/builtins/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 boruta/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 optbinning/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 optbinning/scorecard/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 imblearn/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 imblearn/pipeline/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 category_encoders/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklego/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklego/meta/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 hpsklearn/
+-rw-rw-r--  2.0 unx     4458 b- defN 23-Dec-04 22:17 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx     5202 b- defN 23-Dec-04 22:17 pycaret/pipeline/PyCaretPipeline.class
+-rw-rw-r--  2.0 unx      412 b- defN 23-Dec-04 22:17 pycaret/preprocess/FixImbalancer.class
+-rw-rw-r--  2.0 unx     2980 b- defN 23-Dec-04 22:17 pycaret/preprocess/RemoveMulticollinearity.class
+-rw-rw-r--  2.0 unx      421 b- defN 23-Dec-04 22:17 pycaret/preprocess/CleanColumnNames.class
+-rw-rw-r--  2.0 unx     1332 b- defN 23-Dec-04 22:17 pycaret/preprocess/RemoveOutliers$1.class
+-rw-rw-r--  2.0 unx     2898 b- defN 23-Dec-04 22:17 pycaret/preprocess/RareCategoryGrouping.class
+-rw-rw-r--  2.0 unx     3125 b- defN 23-Dec-04 22:17 pycaret/preprocess/RemoveOutliers.class
+-rw-rw-r--  2.0 unx     8009 b- defN 23-Dec-04 22:17 pycaret/preprocess/TransformerWrapper.class
+-rw-rw-r--  2.0 unx     4170 b- defN 23-Dec-04 22:17 pycaret/preprocess/TransformerWrapperWithInverse.class
+-rw-rw-r--  2.0 unx      720 b- defN 23-Dec-04 22:17 tpot/builtins/StackingEstimator$1.class
+-rw-rw-r--  2.0 unx     4050 b- defN 23-Dec-04 22:17 tpot/builtins/StackingEstimator.class
+-rw-rw-r--  2.0 unx      698 b- defN 23-Dec-04 22:17 boruta/BorutaPy.class
+-rw-rw-r--  2.0 unx     2433 b- defN 23-Dec-04 22:17 optbinning/BinnedFeature.class
+-rw-rw-r--  2.0 unx     9558 b- defN 23-Dec-04 22:17 optbinning/scorecard/Scorecard.class
+-rw-rw-r--  2.0 unx     2133 b- defN 23-Dec-04 22:17 optbinning/OptimalBinningUtil.class
+-rw-rw-r--  2.0 unx     6372 b- defN 23-Dec-04 22:17 optbinning/BinningProcess.class
+-rw-rw-r--  2.0 unx     2274 b- defN 23-Dec-04 22:17 optbinning/ContinuousOptimalBinning.class
+-rw-rw-r--  2.0 unx     3917 b- defN 23-Dec-04 22:17 optbinning/MulticlassOptimalBinning.class
+-rw-rw-r--  2.0 unx     1240 b- defN 23-Dec-04 22:17 optbinning/BinningProcess$1.class
+-rw-rw-r--  2.0 unx    14050 b- defN 23-Dec-04 22:17 optbinning/OptimalBinning.class
+-rw-rw-r--  2.0 unx      424 b- defN 23-Dec-04 22:17 imblearn/pipeline/ImbLearnPipeline.class
+-rw-rw-r--  2.0 unx      374 b- defN 23-Dec-04 22:17 imblearn/Sampler.class
+-rw-rw-r--  2.0 unx     1916 b- defN 23-Dec-04 22:17 category_encoders/MapEncoder.class
+-rw-rw-r--  2.0 unx     8449 b- defN 23-Dec-04 22:17 category_encoders/MapFeature.class
+-rw-rw-r--  2.0 unx      527 b- defN 23-Dec-04 22:17 category_encoders/TargetEncoder.class
+-rw-rw-r--  2.0 unx     1451 b- defN 23-Dec-04 22:17 category_encoders/CountEncoder$1.class
+-rw-rw-r--  2.0 unx      515 b- defN 23-Dec-04 22:17 category_encoders/WOEEncoder.class
+-rw-rw-r--  2.0 unx     8474 b- defN 23-Dec-04 22:17 category_encoders/MeanEncoder.class
+-rw-rw-r--  2.0 unx     8520 b- defN 23-Dec-04 22:17 category_encoders/CountEncoder.class
+-rw-rw-r--  2.0 unx    13032 b- defN 23-Dec-04 22:17 category_encoders/BaseNFeature.class
+-rw-rw-r--  2.0 unx     1481 b- defN 23-Dec-04 22:17 category_encoders/OrdinalMapEncoder$1.class
+-rw-rw-r--  2.0 unx     1445 b- defN 23-Dec-04 22:17 category_encoders/MeanEncoder$1.class
+-rw-rw-r--  2.0 unx     2119 b- defN 23-Dec-04 22:17 category_encoders/OrdinalEncoder$Mapping.class
+-rw-rw-r--  2.0 unx     1323 b- defN 23-Dec-04 22:17 category_encoders/LeaveOneOutEncoder$1.class
+-rw-rw-r--  2.0 unx     8108 b- defN 23-Dec-04 22:17 category_encoders/OrdinalMapEncoder.class
+-rw-rw-r--  2.0 unx     9241 b- defN 23-Dec-04 22:17 category_encoders/BaseNEncoder.class
+-rw-rw-r--  2.0 unx     1334 b- defN 23-Dec-04 22:17 category_encoders/BinaryEncoder.class
+-rw-rw-r--  2.0 unx     3547 b- defN 23-Dec-04 22:17 category_encoders/OneHotEncoder.class
+-rw-rw-r--  2.0 unx     1325 b- defN 23-Dec-04 22:17 category_encoders/CatBoostEncoder.class
+-rw-rw-r--  2.0 unx     2062 b- defN 23-Dec-04 22:17 category_encoders/CategoryEncoderUtil.class
+-rw-rw-r--  2.0 unx     1564 b- defN 23-Dec-04 22:17 category_encoders/OrdinalEncoder$1.class
+-rw-rw-r--  2.0 unx     1047 b- defN 23-Dec-04 22:17 category_encoders/LeaveOneOutEncoder.class
+-rw-rw-r--  2.0 unx     4690 b- defN 23-Dec-04 22:17 category_encoders/OrdinalEncoder.class
+-rw-rw-r--  2.0 unx      742 b- defN 23-Dec-04 22:17 category_encoders/MeanEncoder$MeanFunction.class
+-rw-rw-r--  2.0 unx     1378 b- defN 23-Dec-04 22:17 category_encoders/CatBoostEncoder$1.class
+-rw-rw-r--  2.0 unx     2162 b- defN 23-Dec-04 22:17 category_encoders/CategoryEncoder.class
+-rw-rw-r--  2.0 unx     6139 b- defN 23-Dec-04 22:17 sklego/meta/EstimatorTransformer.class
+-rw-rw-r--  2.0 unx     1259 b- defN 23-Dec-04 22:17 hpsklearn/HyperoptEstimator$1.class
+-rw-rw-r--  2.0 unx     3750 b- defN 23-Dec-04 22:17 hpsklearn/HyperoptEstimator.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Dec-04 22:17 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Dec-04 22:17 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Dec-04 22:17 META-INF/maven/org.jpmml/pmml-sklearn-extension/
+-rw-rw-r--  2.0 unx     1226 b- defN 23-Dec-04 22:16 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml
+-rw-rw-r--  2.0 unx      117 b- defN 23-Dec-04 22:17 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.properties
+71 files, 180323 bytes uncompressed, 78590 bytes compressed:  56.4%
```

#### category_encoders/BaseNFeature.class

##### procyon -ec {}

```diff
@@ -3,23 +3,24 @@
 
 import org.jpmml.model.ToStringHelper;
 import java.util.Objects;
 import java.util.function.Consumer;
 import java.util.LinkedHashSet;
 import java.util.Set;
 import java.util.function.Predicate;
-import java.util.Iterator;
 import org.dmg.pmml.Apply;
+import java.util.Iterator;
 import java.util.function.Supplier;
 import org.jpmml.converter.PMMLUtil;
 import org.dmg.pmml.FieldRef;
 import org.dmg.pmml.Expression;
 import java.util.stream.Collector;
 import java.util.stream.Collectors;
 import java.util.Map;
+import org.jpmml.sklearn.IfElseBuilder;
 import org.dmg.pmml.NormDiscrete;
 import com.google.common.collect.Iterables;
 import java.util.Collection;
 import org.jpmml.converter.ContinuousFeature;
 import org.jpmml.converter.FieldNameUtil;
 import org.dmg.pmml.DataType;
 import org.jpmml.converter.Feature;
@@ -81,16 +82,15 @@
                     final Object category = Iterables.getOnlyElement((Iterable)categories);
                     if (!missingValueAware) {
                         return (Apply)new NormDiscrete(name, category);
                     }
                 }
             }
             Integer missingBaseValue = Integer.valueOf(0);
-            Apply apply = null;
-            Apply prevIfApply = null;
+            final IfElseBuilder applyBuilder = new IfElseBuilder();
             final Collection<? extends Map.Entry<Integer, ? extends Collection<?>>> entries = valueMap.entrySet();
             Map.Entry<Integer, ? extends Collection<?>> entry = null;
             final Collection<? extends Map.Entry<Integer, ? extends Collection<?>>> entries2 = (Collection<? extends Map.Entry<Integer, ? extends Collection<?>>>)entries.stream().sorted((left, right) -> Integer.compare(Integer.valueOf(left.getKey()), Integer.valueOf(right.getKey()))).filter(entry -> Integer.valueOf(entry.getKey()) > 0).collect((Collector<? super Map.Entry<Integer, ? extends Collection<?>>, ?, Collection<? extends Map.Entry<Integer, ? extends Collection<?>>>>)Collectors.toList());
             entries2.iterator();
             final Iterator iterator;
             while (iterator.hasNext()) {
                 entry = iterator.next();
@@ -112,29 +112,23 @@
                     final Apply valueApply = PMMLUtil.createApply((categories2.size() == 1) ? "equal" : "isIn", new Expression[] { (Expression)new FieldRef(name) });
                     categories2.iterator();
                     final Iterator iterator2;
                     while (iterator2.hasNext()) {
                         final Object category2 = iterator2.next();
                         valueApply.addExpressions(new Expression[] { (Expression)PMMLUtil.createConstant(category2, dataType) });
                     }
-                    final Apply ifApply = PMMLUtil.createApply("if", new Expression[] { (Expression)valueApply, (Expression)PMMLUtil.createConstant((Number)baseValue) });
-                    if (apply == null) {
-                        apply = ifApply;
-                    }
-                    if (prevIfApply != null) {
-                        prevIfApply.addExpressions(new Expression[] { (Expression)ifApply });
-                    }
-                    prevIfApply = ifApply;
+                    applyBuilder.add((Expression)valueApply, (Expression)PMMLUtil.createConstant((Number)baseValue));
                 }
             }
-            if (apply == null) {
+            if (applyBuilder.isEmpty()) {
                 return (Apply)PMMLUtil.createConstant((Number)Integer.valueOf(0));
             }
             else {
-                prevIfApply.addExpressions(new Expression[] { (Expression)PMMLUtil.createConstant((Number)Integer.valueOf(0)) });
+                applyBuilder.terminate((Expression)PMMLUtil.createConstant((Number)Integer.valueOf(0)));
+                Apply apply = applyBuilder.build();
                 if (missingValueAware) {
                     apply = PMMLUtil.createApply("if", new Expression[] { (Expression)PMMLUtil.createApply("isNotMissing", new Expression[] { (Expression)new FieldRef(name) }), (Expression)apply, (Expression)PMMLUtil.createConstant((Number)missingBaseValue) });
                 }
                 return apply;
             }
         });
         return this.toContinuousFeature(this.getDerivedName(), DataType.INTEGER, (Supplier)expressionSupplier);
```

#### META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.41</version>
+    <version>1.7.42</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-extension</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn extensions converter</name>
   <description>JPMML Scikit-Learn extension packages to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Mon Oct 23 22:44:50 EEST 2023
-version=1.7.41
+#Mon Dec 04 22:17:23 EET 2023
+version=1.7.42
 groupId=org.jpmml
 artifactId=pmml-sklearn-extension
```

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/pmml-model-1.6.4.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/pmml-model-1.6.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/h2o-logger-3.44.0.1.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/h2o-logger-3.44.0.2.jar`

 * *Files 12% similar despite different names*

#### zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 4526 bytes, number of entries: 9
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:27 META-INF/
--rw-r--r--  2.0 unx       25 b- defN 23-Oct-16 10:27 META-INF/MANIFEST.MF
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 water/
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 water/logging/
--rw-r--r--  2.0 unx     1853 b- defN 23-Oct-16 10:26 water/logging/Slf4JLogger.class
--rw-r--r--  2.0 unx      379 b- defN 23-Oct-16 10:26 water/logging/Logger.class
--rw-r--r--  2.0 unx     2473 b- defN 23-Oct-16 10:26 water/logging/LoggerFactory.class
--rw-r--r--  2.0 unx     1686 b- defN 23-Oct-16 10:26 water/logging/ConsoleLogger.class
--rw-r--r--  2.0 unx     1114 b- defN 23-Oct-16 10:26 water/logging/LoggingLevel.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:51 META-INF/
+-rw-r--r--  2.0 unx       25 b- defN 23-Nov-08 09:51 META-INF/MANIFEST.MF
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 water/
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 water/logging/
+-rw-r--r--  2.0 unx     1853 b- defN 23-Nov-08 09:50 water/logging/Slf4JLogger.class
+-rw-r--r--  2.0 unx      379 b- defN 23-Nov-08 09:50 water/logging/Logger.class
+-rw-r--r--  2.0 unx     2473 b- defN 23-Nov-08 09:50 water/logging/LoggerFactory.class
+-rw-r--r--  2.0 unx     1686 b- defN 23-Nov-08 09:50 water/logging/ConsoleLogger.class
+-rw-r--r--  2.0 unx     1114 b- defN 23-Nov-08 09:50 water/logging/LoggingLevel.class
 9 files, 7530 bytes uncompressed, 3412 bytes compressed:  54.7%
```

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/ubjson-gson-0.1.8.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/ubjson-gson-0.1.8.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/ubjson-0.1.8.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/ubjson-0.1.8.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/gson-2.10.1.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/gson-2.10.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/h2o-genmodel-3.44.0.1.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/h2o-genmodel-3.44.0.2.jar`

 * *Files 11% similar despite different names*

#### zipinfo {}

```diff
@@ -1,393 +1,394 @@
-Zip file size: 466064 bytes, number of entries: 391
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:27 META-INF/
--rw-r--r--  2.0 unx       25 b- defN 23-Oct-16 10:27 META-INF/MANIFEST.MF
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/
--rw-r--r--  2.0 unx     1699 b- defN 23-Oct-16 10:26 hex/ModelCategory.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/descriptor/
--rw-r--r--  2.0 unx      731 b- defN 23-Oct-16 10:26 hex/genmodel/descriptor/ModelDescriptor.class
--rw-r--r--  2.0 unx     3832 b- defN 23-Oct-16 10:26 hex/genmodel/descriptor/ModelDescriptorBuilder$PojoModelDescriptor.class
--rw-r--r--  2.0 unx      262 b- defN 23-Oct-16 10:26 hex/genmodel/descriptor/ModelDescriptorBuilder$1.class
--rw-r--r--  2.0 unx     1415 b- defN 23-Oct-16 10:26 hex/genmodel/descriptor/ModelDescriptorBuilder.class
--rw-r--r--  2.0 unx     4531 b- defN 23-Oct-16 10:26 hex/genmodel/descriptor/ModelDescriptorBuilder$MojoModelDescriptor.class
--rw-r--r--  2.0 unx     1088 b- defN 23-Oct-16 10:26 hex/genmodel/ModelMojoReader$RawValue.class
--rw-r--r--  2.0 unx     5067 b- defN 23-Oct-16 10:26 hex/genmodel/MojoReaderBackendFactory.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/easy/
--rw-r--r--  2.0 unx     2069 b- defN 23-Oct-16 10:26 hex/genmodel/easy/EnumLimitedEncoderDomainMapConstructor.class
--rw-r--r--  2.0 unx     1698 b- defN 23-Oct-16 10:26 hex/genmodel/easy/EnumEncoder.class
--rw-r--r--  2.0 unx     1570 b- defN 23-Oct-16 10:26 hex/genmodel/easy/EigenEncoder.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/easy/prediction/
--rw-r--r--  2.0 unx      549 b- defN 23-Oct-16 10:26 hex/genmodel/easy/prediction/AutoEncoderModelPrediction.class
--rw-r--r--  2.0 unx      365 b- defN 23-Oct-16 10:26 hex/genmodel/easy/prediction/AbstractPrediction.class
--rw-r--r--  2.0 unx     1159 b- defN 23-Oct-16 10:26 hex/genmodel/easy/prediction/AnomalyDetectionPrediction.class
--rw-r--r--  2.0 unx      476 b- defN 23-Oct-16 10:26 hex/genmodel/easy/prediction/OrdinalModelPrediction.class
--rw-r--r--  2.0 unx      394 b- defN 23-Oct-16 10:26 hex/genmodel/easy/prediction/CoxPHModelPrediction.class
--rw-r--r--  2.0 unx      455 b- defN 23-Oct-16 10:26 hex/genmodel/easy/prediction/ClusteringModelPrediction.class
--rw-r--r--  2.0 unx      683 b- defN 23-Oct-16 10:26 hex/genmodel/easy/prediction/SortedClassProbability.class
--rw-r--r--  2.0 unx      428 b- defN 23-Oct-16 10:26 hex/genmodel/easy/prediction/UpliftBinomialModelPrediction.class
--rw-r--r--  2.0 unx      606 b- defN 23-Oct-16 10:26 hex/genmodel/easy/prediction/MultinomialModelPrediction.class
--rw-r--r--  2.0 unx      479 b- defN 23-Oct-16 10:26 hex/genmodel/easy/prediction/Word2VecPrediction.class
--rw-r--r--  2.0 unx      665 b- defN 23-Oct-16 10:26 hex/genmodel/easy/prediction/BinomialModelPrediction.class
--rw-r--r--  2.0 unx      445 b- defN 23-Oct-16 10:26 hex/genmodel/easy/prediction/DimReductionModelPrediction.class
--rw-r--r--  2.0 unx      561 b- defN 23-Oct-16 10:26 hex/genmodel/easy/prediction/RegressionModelPrediction.class
--rw-r--r--  2.0 unx      414 b- defN 23-Oct-16 10:26 hex/genmodel/easy/prediction/TargetEncoderPrediction.class
--rw-r--r--  2.0 unx      430 b- defN 23-Oct-16 10:26 hex/genmodel/easy/prediction/KLimeModelPrediction.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/easy/exception/
--rw-r--r--  2.0 unx      454 b- defN 23-Oct-16 10:26 hex/genmodel/easy/exception/PredictUnknownTypeException.class
--rw-r--r--  2.0 unx      683 b- defN 23-Oct-16 10:26 hex/genmodel/easy/exception/PredictException.class
--rw-r--r--  2.0 unx      457 b- defN 23-Oct-16 10:26 hex/genmodel/easy/exception/PredictNumberFormatException.class
--rw-r--r--  2.0 unx      475 b- defN 23-Oct-16 10:26 hex/genmodel/easy/exception/PredictWrongModelCategoryException.class
--rw-r--r--  2.0 unx      831 b- defN 23-Oct-16 10:26 hex/genmodel/easy/exception/PredictUnknownCategoricalLevelException.class
--rw-r--r--  2.0 unx     1302 b- defN 23-Oct-16 10:26 hex/genmodel/easy/EnumEncoderColumnMapper.class
--rw-r--r--  2.0 unx     1309 b- defN 23-Oct-16 10:26 hex/genmodel/easy/EigenEncoderColumnMapper.class
--rw-r--r--  2.0 unx    24456 b- defN 23-Oct-16 10:26 hex/genmodel/easy/EasyPredictModelWrapper.class
--rw-r--r--  2.0 unx     5805 b- defN 23-Oct-16 10:26 hex/genmodel/easy/EasyPredictModelWrapper$Config.class
--rw-r--r--  2.0 unx      621 b- defN 23-Oct-16 10:26 hex/genmodel/easy/EnumLimitedEncoderColumnMapper.class
--rw-r--r--  2.0 unx      241 b- defN 23-Oct-16 10:26 hex/genmodel/easy/CategoricalEncoder.class
--rw-r--r--  2.0 unx     5444 b- defN 23-Oct-16 10:26 hex/genmodel/easy/RowToRawDataConverter.class
--rw-r--r--  2.0 unx      363 b- defN 23-Oct-16 10:26 hex/genmodel/easy/RowData.class
--rw-r--r--  2.0 unx      597 b- defN 23-Oct-16 10:26 hex/genmodel/easy/EasyPredictModelWrapper$ErrorConsumer.class
--rw-r--r--  2.0 unx     1939 b- defN 23-Oct-16 10:26 hex/genmodel/easy/LabelEncoderDomainMapConstructor.class
--rw-r--r--  2.0 unx     1591 b- defN 23-Oct-16 10:26 hex/genmodel/easy/BinaryColumnMapper.class
--rw-r--r--  2.0 unx      872 b- defN 23-Oct-16 10:26 hex/genmodel/easy/DomainMapConstructor.class
--rw-r--r--  2.0 unx     1941 b- defN 23-Oct-16 10:26 hex/genmodel/easy/BinaryDomainMapConstructor.class
--rw-r--r--  2.0 unx     1570 b- defN 23-Oct-16 10:26 hex/genmodel/easy/OneHotEncoderColumnMapper.class
--rw-r--r--  2.0 unx     1962 b- defN 23-Oct-16 10:26 hex/genmodel/easy/OneHotEncoderDomainMapConstructor.class
--rw-r--r--  2.0 unx     2357 b- defN 23-Oct-16 10:26 hex/genmodel/easy/EnumLimitedEncoder.class
--rw-r--r--  2.0 unx     2209 b- defN 23-Oct-16 10:26 hex/genmodel/easy/OneHotEncoder.class
--rw-r--r--  2.0 unx     2290 b- defN 23-Oct-16 10:26 hex/genmodel/easy/BinaryEncoder.class
--rw-r--r--  2.0 unx     1633 b- defN 23-Oct-16 10:26 hex/genmodel/easy/LabelEncoder.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/easy/error/
--rw-r--r--  2.0 unx      805 b- defN 23-Oct-16 10:26 hex/genmodel/easy/error/VoidErrorConsumer.class
--rw-r--r--  2.0 unx      702 b- defN 23-Oct-16 10:26 hex/genmodel/easy/error/CountingErrorConsumer$Config.class
--rw-r--r--  2.0 unx     5332 b- defN 23-Oct-16 10:26 hex/genmodel/easy/error/CountingErrorConsumer.class
--rw-r--r--  2.0 unx     1325 b- defN 23-Oct-16 10:26 hex/genmodel/easy/EasyPredictModelWrapper$1.class
--rw-r--r--  2.0 unx     1876 b- defN 23-Oct-16 10:26 hex/genmodel/easy/EnumEncoderDomainMapConstructor.class
--rw-r--r--  2.0 unx     2146 b- defN 23-Oct-16 10:26 hex/genmodel/easy/EigenEncoderDomainMapConstructor.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/tools/
--rw-r--r--  2.0 unx     1287 b- defN 23-Oct-16 10:26 hex/genmodel/tools/PrintMojo$FloatCastingSerializer.class
--rw-r--r--  2.0 unx     1026 b- defN 23-Oct-16 10:26 hex/genmodel/tools/PredictCsv$1.class
--rw-r--r--  2.0 unx     5410 b- defN 23-Oct-16 10:26 hex/genmodel/tools/MungeCsv.class
--rw-r--r--  2.0 unx     1010 b- defN 23-Oct-16 10:26 hex/genmodel/tools/PrintMojo$PrintTreeOptions.class
--rw-r--r--  2.0 unx    20777 b- defN 23-Oct-16 10:26 hex/genmodel/tools/PredictCsv.class
--rw-r--r--  2.0 unx    14133 b- defN 23-Oct-16 10:26 hex/genmodel/tools/PrintMojo.class
--rw-r--r--  2.0 unx     1286 b- defN 23-Oct-16 10:26 hex/genmodel/tools/PredictCsv$PredictCsvCollection.class
--rw-r--r--  2.0 unx     4591 b- defN 23-Oct-16 10:26 hex/genmodel/tools/PredictCsv$PredictCsvBuilder.class
--rw-r--r--  2.0 unx      826 b- defN 23-Oct-16 10:26 hex/genmodel/tools/PrintMojo$2.class
--rw-r--r--  2.0 unx      722 b- defN 23-Oct-16 10:26 hex/genmodel/tools/PrintMojo$1.class
--rw-r--r--  2.0 unx     7956 b- defN 23-Oct-16 10:26 hex/genmodel/tools/BuildPipeline.class
--rw-r--r--  2.0 unx     1294 b- defN 23-Oct-16 10:26 hex/genmodel/tools/PredictCsv$PredictCsvCallable.class
--rw-r--r--  2.0 unx     1202 b- defN 23-Oct-16 10:26 hex/genmodel/tools/MojoPrinter$Format.class
--rw-r--r--  2.0 unx      388 b- defN 23-Oct-16 10:26 hex/genmodel/tools/MojoPrinter.class
--rw-r--r--  2.0 unx      895 b- defN 23-Oct-16 10:26 hex/genmodel/ConverterFactoryProvidingModel.class
--rw-r--r--  2.0 unx     1538 b- defN 23-Oct-16 10:26 hex/genmodel/CategoricalEncoding$6.class
--rw-r--r--  2.0 unx     2779 b- defN 23-Oct-16 10:26 hex/genmodel/MultiModelMojoReader.class
--rw-r--r--  2.0 unx     1583 b- defN 23-Oct-16 10:26 hex/genmodel/GenMunger$Step.class
--rw-r--r--  2.0 unx     1277 b- defN 23-Oct-16 10:26 hex/genmodel/GenModel$1.class
--rw-r--r--  2.0 unx     1403 b- defN 23-Oct-16 10:26 hex/genmodel/TmpMojoReaderBackend.class
--rw-r--r--  2.0 unx      215 b- defN 23-Oct-16 10:26 hex/genmodel/IClusteringModel.class
--rw-r--r--  2.0 unx     2445 b- defN 23-Oct-16 10:26 hex/genmodel/CategoricalEncoding.class
--rw-r--r--  2.0 unx     6310 b- defN 23-Oct-16 10:26 hex/genmodel/MojoPipelineBuilder.class
--rw-r--r--  2.0 unx     2276 b- defN 23-Oct-16 10:26 hex/genmodel/InMemoryMojoReaderBackend.class
--rw-r--r--  2.0 unx     5604 b- defN 23-Oct-16 10:26 hex/genmodel/MojoPipelineWriter.class
--rw-r--r--  2.0 unx     1729 b- defN 23-Oct-16 10:26 hex/genmodel/FolderMojoReaderBackend.class
--rw-r--r--  2.0 unx     1489 b- defN 23-Oct-16 10:26 hex/genmodel/CategoricalEncoding$1.class
--rw-r--r--  2.0 unx      225 b- defN 23-Oct-16 10:26 hex/genmodel/PredictContributionsFactory.class
--rw-r--r--  2.0 unx      334 b- defN 23-Oct-16 10:26 hex/genmodel/PredictContributions.class
--rw-r--r--  2.0 unx     4315 b- defN 23-Oct-16 10:26 hex/genmodel/MojoPipelineWriter$MojoPipelineDescriptor.class
--rw-r--r--  2.0 unx      234 b- defN 23-Oct-16 10:26 hex/genmodel/MultiModelMojoReader$1.class
--rw-r--r--  2.0 unx     9766 b- defN 23-Oct-16 10:26 hex/genmodel/AbstractMojoWriter.class
--rw-r--r--  2.0 unx     3008 b- defN 23-Oct-16 10:26 hex/genmodel/MojoModel.class
--rw-r--r--  2.0 unx      228 b- defN 23-Oct-16 10:26 hex/genmodel/MojoPipelineWriter$1.class
--rw-r--r--  2.0 unx      345 b- defN 23-Oct-16 10:26 hex/genmodel/MojoReaderBackend.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/utils/
--rw-r--r--  2.0 unx     1366 b- defN 23-Oct-16 10:26 hex/genmodel/utils/StringEscapeUtils.class
--rw-r--r--  2.0 unx      770 b- defN 23-Oct-16 10:26 hex/genmodel/utils/IOUtils.class
--rw-r--r--  2.0 unx     7386 b- defN 23-Oct-16 10:26 hex/genmodel/utils/ArrayUtils.class
--rw-r--r--  2.0 unx     3399 b- defN 23-Oct-16 10:26 hex/genmodel/utils/ParseUtils.class
--rw-r--r--  2.0 unx     1869 b- defN 23-Oct-16 10:26 hex/genmodel/utils/ByteBufferWrapper.class
--rw-r--r--  2.0 unx     1329 b- defN 23-Oct-16 10:26 hex/genmodel/utils/MathUtils.class
--rw-r--r--  2.0 unx      988 b- defN 23-Oct-16 10:26 hex/genmodel/utils/ArrayUtils$1.class
--rw-r--r--  2.0 unx     1361 b- defN 23-Oct-16 10:26 hex/genmodel/utils/LinkFunctionType.class
--rw-r--r--  2.0 unx     1862 b- defN 23-Oct-16 10:26 hex/genmodel/utils/DistributionFamily.class
--rw-r--r--  2.0 unx     3320 b- defN 23-Oct-16 10:26 hex/genmodel/utils/GenmodelBitSet.class
--rw-r--r--  2.0 unx     1206 b- defN 23-Oct-16 10:26 hex/genmodel/utils/ArrayUtils$2.class
--rw-r--r--  2.0 unx     1234 b- defN 23-Oct-16 10:26 hex/genmodel/MojoReaderBackendFactory$CachingStrategy.class
--rw-r--r--  2.0 unx     8569 b- defN 23-Oct-16 10:26 hex/genmodel/GenMunger.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/annotations/
--rw-r--r--  2.0 unx      521 b- defN 23-Oct-16 10:26 hex/genmodel/annotations/ModelPojo.class
--rw-r--r--  2.0 unx     1527 b- defN 23-Oct-16 10:26 hex/genmodel/CategoricalEncoding$3.class
--rw-r--r--  2.0 unx      398 b- defN 23-Oct-16 10:26 hex/genmodel/IGenModel.class
--rw-r--r--  2.0 unx     1539 b- defN 23-Oct-16 10:26 hex/genmodel/CategoricalEncoding$5.class
--rw-r--r--  2.0 unx     1268 b- defN 23-Oct-16 10:26 hex/genmodel/NestedMojoReaderBackend.class
--rw-r--r--  2.0 unx    15640 b- defN 23-Oct-16 10:26 hex/genmodel/ModelMojoReader.class
--rw-r--r--  2.0 unx     2041 b- defN 23-Oct-16 10:26 hex/genmodel/ZipfileMojoReaderBackend.class
--rw-r--r--  2.0 unx    19329 b- defN 23-Oct-16 10:26 hex/genmodel/GenModel.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/algos/
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/algos/svm/
--rw-r--r--  2.0 unx     1887 b- defN 23-Oct-16 10:26 hex/genmodel/algos/svm/SvmMojoReader.class
--rw-r--r--  2.0 unx     1340 b- defN 23-Oct-16 10:26 hex/genmodel/algos/svm/SvmMojoModel.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/algos/upliftdrf/
--rw-r--r--  2.0 unx     1699 b- defN 23-Oct-16 10:26 hex/genmodel/algos/upliftdrf/UpliftDrfMojoModel.class
--rw-r--r--  2.0 unx     2172 b- defN 23-Oct-16 10:26 hex/genmodel/algos/upliftdrf/UpliftDrfMojoReader.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/algos/klime/
--rw-r--r--  2.0 unx     2319 b- defN 23-Oct-16 10:26 hex/genmodel/algos/klime/KLimeMojoModel.class
--rw-r--r--  2.0 unx     2687 b- defN 23-Oct-16 10:26 hex/genmodel/algos/klime/KLimeMojoReader.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/algos/word2vec/
--rw-r--r--  2.0 unx     1490 b- defN 23-Oct-16 10:26 hex/genmodel/algos/word2vec/Word2VecMojoModel.class
--rw-r--r--  2.0 unx     3174 b- defN 23-Oct-16 10:26 hex/genmodel/algos/word2vec/Word2VecMojoReader.class
--rw-r--r--  2.0 unx      220 b- defN 23-Oct-16 10:26 hex/genmodel/algos/word2vec/WordEmbeddingModel.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/algos/rulefit/
--rw-r--r--  2.0 unx      863 b- defN 23-Oct-16 10:26 hex/genmodel/algos/rulefit/MojoRule.class
--rw-r--r--  2.0 unx     1620 b- defN 23-Oct-16 10:26 hex/genmodel/algos/rulefit/MojoCondition.class
--rw-r--r--  2.0 unx     2502 b- defN 23-Oct-16 10:26 hex/genmodel/algos/rulefit/RuleFitMojoModel.class
--rw-r--r--  2.0 unx     7385 b- defN 23-Oct-16 10:26 hex/genmodel/algos/rulefit/RuleFitMojoReader.class
--rw-r--r--  2.0 unx     3386 b- defN 23-Oct-16 10:26 hex/genmodel/algos/rulefit/MojoRuleEnsemble.class
--rw-r--r--  2.0 unx     1177 b- defN 23-Oct-16 10:26 hex/genmodel/algos/rulefit/MojoCondition$Type.class
--rw-r--r--  2.0 unx     1286 b- defN 23-Oct-16 10:26 hex/genmodel/algos/rulefit/RuleFitMojoModel$ModelType.class
--rw-r--r--  2.0 unx     1256 b- defN 23-Oct-16 10:26 hex/genmodel/algos/rulefit/MojoCondition$Operator.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/
--rw-r--r--  2.0 unx      263 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/TreeSHAPPredictor$Workspace.class
--rw-r--r--  2.0 unx     3299 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/SharedTreeMojoModel$AuxInfoLightReader.class
--rw-r--r--  2.0 unx      880 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/TreeSHAP$PathElement.class
--rw-r--r--  2.0 unx     4714 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/SharedTreeMojoReader.class
--rw-r--r--  2.0 unx      353 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/SharedTreeGraphConverter.class
--rw-r--r--  2.0 unx      657 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/ScoreTree0.class
--rw-r--r--  2.0 unx      202 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/ScoreTree.class
--rw-r--r--  2.0 unx      220 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/TreeSHAP$1.class
--rw-r--r--  2.0 unx      635 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/ScoreTree2.class
--rw-r--r--  2.0 unx     1101 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/ConvertTreeOptions.class
--rw-r--r--  2.0 unx     8018 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/SharedTreeSubgraph.class
--rw-r--r--  2.0 unx     3434 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/TreeSHAPEnsemble.class
--rw-r--r--  2.0 unx    11309 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/TreeSHAP.class
--rw-r--r--  2.0 unx      253 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/SharedTreeMojoModel$1.class
--rw-r--r--  2.0 unx      535 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/SharedTreeMojoModel$LeafNodeAssignments.class
--rw-r--r--  2.0 unx      438 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/SharedTreeMojoModel$DecisionPathTracker.class
--rw-r--r--  2.0 unx     2835 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/SharedTreeMojoModelWithContributions.class
--rw-r--r--  2.0 unx      657 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/ScoreTree1.class
--rw-r--r--  2.0 unx      833 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/TreeSHAPPredictor.class
--rw-r--r--  2.0 unx    16477 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/SharedTreeNode.class
--rw-r--r--  2.0 unx     1175 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/CalibrationMojoHelper.class
--rw-r--r--  2.0 unx     2634 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/ContributionComposer.class
--rw-r--r--  2.0 unx      602 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/ScoreIsolationTree0.class
--rw-r--r--  2.0 unx     1395 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/NaSplitDir.class
--rw-r--r--  2.0 unx     3003 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/SharedTreeMojoModel$LeafDecisionPathTracker.class
--rw-r--r--  2.0 unx      611 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/TreeBackedMojoModel.class
--rw-r--r--  2.0 unx     3699 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/SharedTreeGraph.class
--rw-r--r--  2.0 unx    25057 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/SharedTreeMojoModel.class
--rw-r--r--  2.0 unx     1518 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/SharedTreeMojoModelWithContributions$SharedTreeContributionsPredictor.class
--rw-r--r--  2.0 unx     1707 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/TreeSHAP$PathPointer.class
--rw-r--r--  2.0 unx      199 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/ScoreIsolationTree.class
--rw-r--r--  2.0 unx     1445 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/SharedTreeMojoModel$StringDecisionPathTracker.class
--rw-r--r--  2.0 unx      399 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/CalibrationMojoHelper$MojoModelWithCalibration.class
--rw-r--r--  2.0 unx     3805 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/ContributionsPredictor.class
--rw-r--r--  2.0 unx     2632 b- defN 23-Oct-16 10:26 hex/genmodel/algos/tree/SharedTreeMojoModel$AuxInfo.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/algos/coxph/
--rw-r--r--  2.0 unx     6398 b- defN 23-Oct-16 10:26 hex/genmodel/algos/coxph/CoxPHMojoModel.class
--rw-r--r--  2.0 unx     1311 b- defN 23-Oct-16 10:26 hex/genmodel/algos/coxph/CoxPHMojoModel$InteractionTypes.class
--rw-r--r--  2.0 unx     1144 b- defN 23-Oct-16 10:26 hex/genmodel/algos/coxph/CoxPHMojoModel$Strata.class
--rw-r--r--  2.0 unx     5061 b- defN 23-Oct-16 10:26 hex/genmodel/algos/coxph/CoxPHMojoReader.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/algos/drf/
--rw-r--r--  2.0 unx     1633 b- defN 23-Oct-16 10:26 hex/genmodel/algos/drf/DrfMojoReader.class
--rw-r--r--  2.0 unx      230 b- defN 23-Oct-16 10:26 hex/genmodel/algos/drf/DrfMojoModel$1.class
--rw-r--r--  2.0 unx     3129 b- defN 23-Oct-16 10:26 hex/genmodel/algos/drf/DrfMojoModel$ContributionsPredictorDRF.class
--rw-r--r--  2.0 unx     2700 b- defN 23-Oct-16 10:26 hex/genmodel/algos/drf/DrfMojoModel.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/algos/isoforextended/
--rw-r--r--  2.0 unx     4170 b- defN 23-Oct-16 10:26 hex/genmodel/algos/isoforextended/ExtendedIsolationForestMojoModel.class
--rw-r--r--  2.0 unx     2306 b- defN 23-Oct-16 10:26 hex/genmodel/algos/isoforextended/ExtendedIsolationForestMojoReader.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/algos/pca/
--rw-r--r--  2.0 unx     2645 b- defN 23-Oct-16 10:26 hex/genmodel/algos/pca/PCAMojoModel.class
--rw-r--r--  2.0 unx     2819 b- defN 23-Oct-16 10:26 hex/genmodel/algos/pca/PCAMojoReader.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glm/
--rw-r--r--  2.0 unx     4318 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glm/GlmMojoModel.class
--rw-r--r--  2.0 unx     2466 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glm/GlmMultinomialMojoModel.class
--rw-r--r--  2.0 unx     1747 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glm/GlmMojoModelBase.class
--rw-r--r--  2.0 unx      848 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glm/GlmMojoModel$GLM_inverseInv.class
--rw-r--r--  2.0 unx      851 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glm/GlmMojoModel$GLM_identityInv.class
--rw-r--r--  2.0 unx      230 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glm/GlmMojoModel$1.class
--rw-r--r--  2.0 unx     2647 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glm/GlmOrdinalMojoModel.class
--rw-r--r--  2.0 unx      836 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glm/GlmMojoModel$GLM_logInv.class
--rw-r--r--  2.0 unx      626 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glm/GlmMojoModel$GLM_ologitInv.class
--rw-r--r--  2.0 unx      272 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glm/GlmMojoModel$Function1.class
--rw-r--r--  2.0 unx      724 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glm/GlmMojoModel$GLM_tweedieInv.class
--rw-r--r--  2.0 unx      842 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glm/GlmMojoModel$GLM_logitInv.class
--rw-r--r--  2.0 unx     3584 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glm/GlmMojoReader.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/algos/targetencoder/
--rw-r--r--  2.0 unx      677 b- defN 23-Oct-16 10:26 hex/genmodel/algos/targetencoder/ColumnsMapping.class
--rw-r--r--  2.0 unx     3493 b- defN 23-Oct-16 10:26 hex/genmodel/algos/targetencoder/EncodingMap.class
--rw-r--r--  2.0 unx     9375 b- defN 23-Oct-16 10:26 hex/genmodel/algos/targetencoder/TargetEncoderMojoReader.class
--rw-r--r--  2.0 unx     2436 b- defN 23-Oct-16 10:26 hex/genmodel/algos/targetencoder/EncodingMaps.class
--rw-r--r--  2.0 unx     1417 b- defN 23-Oct-16 10:26 hex/genmodel/algos/targetencoder/ColumnsToSingleMapping.class
--rw-r--r--  2.0 unx     8265 b- defN 23-Oct-16 10:26 hex/genmodel/algos/targetencoder/TargetEncoderMojoModel.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/algos/isotonic/
--rw-r--r--  2.0 unx      888 b- defN 23-Oct-16 10:26 hex/genmodel/algos/isotonic/IsotonicCalibrator.class
--rw-r--r--  2.0 unx      874 b- defN 23-Oct-16 10:26 hex/genmodel/algos/isotonic/IsotonicRegressionMojoModel.class
--rw-r--r--  2.0 unx     1676 b- defN 23-Oct-16 10:26 hex/genmodel/algos/isotonic/IsotonicRegressionMojoReader.class
--rw-r--r--  2.0 unx     1680 b- defN 23-Oct-16 10:26 hex/genmodel/algos/isotonic/IsotonicRegressionUtils.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/algos/deeplearning/
--rw-r--r--  2.0 unx      783 b- defN 23-Oct-16 10:26 hex/genmodel/algos/deeplearning/ActivationUtils$RectifierDropoutOut.class
--rw-r--r--  2.0 unx     5224 b- defN 23-Oct-16 10:26 hex/genmodel/algos/deeplearning/DeeplearningMojoReader.class
--rw-r--r--  2.0 unx     1081 b- defN 23-Oct-16 10:26 hex/genmodel/algos/deeplearning/ActivationUtils$SoftmaxOut.class
--rw-r--r--  2.0 unx      769 b- defN 23-Oct-16 10:26 hex/genmodel/algos/deeplearning/ActivationUtils$MaxoutDropoutOut.class
--rw-r--r--  2.0 unx      709 b- defN 23-Oct-16 10:26 hex/genmodel/algos/deeplearning/ActivationUtils$LinearOut.class
--rw-r--r--  2.0 unx     1096 b- defN 23-Oct-16 10:26 hex/genmodel/algos/deeplearning/DeeplearningMojoModel$1.class
--rw-r--r--  2.0 unx     6719 b- defN 23-Oct-16 10:26 hex/genmodel/algos/deeplearning/NeuralNetwork.class
--rw-r--r--  2.0 unx      934 b- defN 23-Oct-16 10:26 hex/genmodel/algos/deeplearning/ActivationUtils$RectifierOut.class
--rw-r--r--  2.0 unx      323 b- defN 23-Oct-16 10:26 hex/genmodel/algos/deeplearning/ActivationUtils$ActivationFunctions.class
--rw-r--r--  2.0 unx     2132 b- defN 23-Oct-16 10:26 hex/genmodel/algos/deeplearning/ActivationUtils.class
--rw-r--r--  2.0 unx      798 b- defN 23-Oct-16 10:26 hex/genmodel/algos/deeplearning/ActivationUtils$ExpRectifierDropoutOut.class
--rw-r--r--  2.0 unx      663 b- defN 23-Oct-16 10:26 hex/genmodel/algos/deeplearning/DeeplearningMojoModel$StoreWeightsBias.class
--rw-r--r--  2.0 unx     6843 b- defN 23-Oct-16 10:26 hex/genmodel/algos/deeplearning/DeeplearningMojoModel.class
--rw-r--r--  2.0 unx      787 b- defN 23-Oct-16 10:26 hex/genmodel/algos/deeplearning/ActivationUtils$TanhDropoutOut.class
--rw-r--r--  2.0 unx      995 b- defN 23-Oct-16 10:26 hex/genmodel/algos/deeplearning/ActivationUtils$ExpRectifierOut.class
--rw-r--r--  2.0 unx      922 b- defN 23-Oct-16 10:26 hex/genmodel/algos/deeplearning/ActivationUtils$TanhOut.class
--rw-r--r--  2.0 unx     1007 b- defN 23-Oct-16 10:26 hex/genmodel/algos/deeplearning/ActivationUtils$MaxoutOut.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/algos/psvm/
--rw-r--r--  2.0 unx      196 b- defN 23-Oct-16 10:26 hex/genmodel/algos/psvm/SupportVectorScorer.class
--rw-r--r--  2.0 unx      422 b- defN 23-Oct-16 10:26 hex/genmodel/algos/psvm/KernelParameters.class
--rw-r--r--  2.0 unx     1388 b- defN 23-Oct-16 10:26 hex/genmodel/algos/psvm/ScorerFactory.class
--rw-r--r--  2.0 unx     1550 b- defN 23-Oct-16 10:26 hex/genmodel/algos/psvm/GaussianScorer.class
--rw-r--r--  2.0 unx      973 b- defN 23-Oct-16 10:26 hex/genmodel/algos/psvm/KernelType.class
--rw-r--r--  2.0 unx      699 b- defN 23-Oct-16 10:26 hex/genmodel/algos/psvm/ScorerFactory$1.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/algos/ensemble/
--rw-r--r--  2.0 unx     3993 b- defN 23-Oct-16 10:26 hex/genmodel/algos/ensemble/StackedEnsembleMojoReader.class
--rw-r--r--  2.0 unx      974 b- defN 23-Oct-16 10:26 hex/genmodel/algos/ensemble/StackedEnsembleMojoModel$StackedEnsembleMojoSubModel.class
--rw-r--r--  2.0 unx     2165 b- defN 23-Oct-16 10:26 hex/genmodel/algos/ensemble/StackedEnsembleMojoModel.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/algos/isofor/
--rw-r--r--  2.0 unx     1835 b- defN 23-Oct-16 10:26 hex/genmodel/algos/isofor/IsolationForestMojoModel.class
--rw-r--r--  2.0 unx     2021 b- defN 23-Oct-16 10:26 hex/genmodel/algos/isofor/IsolationForestMojoReader.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/algos/gam/
--rw-r--r--  2.0 unx     1572 b- defN 23-Oct-16 10:26 hex/genmodel/algos/gam/GamMojoModel.class
--rw-r--r--  2.0 unx     2046 b- defN 23-Oct-16 10:26 hex/genmodel/algos/gam/ISplines.class
--rw-r--r--  2.0 unx     2045 b- defN 23-Oct-16 10:26 hex/genmodel/algos/gam/NBSplinesTypeII.class
--rw-r--r--  2.0 unx    10726 b- defN 23-Oct-16 10:26 hex/genmodel/algos/gam/GamMojoReader.class
--rw-r--r--  2.0 unx     1717 b- defN 23-Oct-16 10:26 hex/genmodel/algos/gam/NBSplinesTypeI$MSplineBasis.class
--rw-r--r--  2.0 unx      855 b- defN 23-Oct-16 10:26 hex/genmodel/algos/gam/ISplines$ISplineBasis.class
--rw-r--r--  2.0 unx     1902 b- defN 23-Oct-16 10:26 hex/genmodel/algos/gam/NBSplinesTypeII$BSplineBasis.class
--rw-r--r--  2.0 unx     3495 b- defN 23-Oct-16 10:26 hex/genmodel/algos/gam/NBSplinesTypeI.class
--rw-r--r--  2.0 unx     2061 b- defN 23-Oct-16 10:26 hex/genmodel/algos/gam/GamUtilsThinPlateRegression.class
--rw-r--r--  2.0 unx    11583 b- defN 23-Oct-16 10:26 hex/genmodel/algos/gam/GamMojoModelBase.class
--rw-r--r--  2.0 unx     1347 b- defN 23-Oct-16 10:26 hex/genmodel/algos/gam/MSplines.class
--rw-r--r--  2.0 unx     4489 b- defN 23-Oct-16 10:26 hex/genmodel/algos/gam/GamUtilsISplines.class
--rw-r--r--  2.0 unx      896 b- defN 23-Oct-16 10:26 hex/genmodel/algos/gam/GamMojoModelBase$1.class
--rw-r--r--  2.0 unx     2234 b- defN 23-Oct-16 10:26 hex/genmodel/algos/gam/GamMojoMultinomialModel.class
--rw-r--r--  2.0 unx     1977 b- defN 23-Oct-16 10:26 hex/genmodel/algos/gam/GamRowToRawDataConverter.class
--rw-r--r--  2.0 unx     2518 b- defN 23-Oct-16 10:26 hex/genmodel/algos/gam/GamUtilsCubicRegression.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/algos/pipeline/
--rw-r--r--  2.0 unx     1732 b- defN 23-Oct-16 10:26 hex/genmodel/algos/pipeline/MojoPipeline.class
--rw-r--r--  2.0 unx     6799 b- defN 23-Oct-16 10:26 hex/genmodel/algos/pipeline/MojoPipelineReader.class
--rw-r--r--  2.0 unx      635 b- defN 23-Oct-16 10:26 hex/genmodel/algos/pipeline/MojoPipeline$PipelineSubModel.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/algos/kmeans/
--rw-r--r--  2.0 unx     1339 b- defN 23-Oct-16 10:26 hex/genmodel/algos/kmeans/KMeansMojoModel.class
--rw-r--r--  2.0 unx     2248 b- defN 23-Oct-16 10:26 hex/genmodel/algos/kmeans/KMeansMojoReader.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/algos/gbm/
--rw-r--r--  2.0 unx     4006 b- defN 23-Oct-16 10:26 hex/genmodel/algos/gbm/GbmMojoModel.class
--rw-r--r--  2.0 unx     2104 b- defN 23-Oct-16 10:26 hex/genmodel/algos/gbm/GbmMojoReader.class
--rw-r--r--  2.0 unx      981 b- defN 23-Oct-16 10:26 hex/genmodel/algos/gbm/GbmMojoModel$1.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glrm/
--rw-r--r--  2.0 unx     1345 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glrm/GlrmRegularizer$3.class
--rw-r--r--  2.0 unx     4904 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glrm/GlrmMojoReader.class
--rw-r--r--  2.0 unx     1567 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glrm/GlrmLoss$5.class
--rw-r--r--  2.0 unx     2161 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glrm/GlrmLoss$8.class
--rw-r--r--  2.0 unx     1232 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glrm/GlrmRegularizer$2.class
--rw-r--r--  2.0 unx     1980 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glrm/GlrmRegularizer$8.class
--rw-r--r--  2.0 unx      875 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glrm/GlrmRegularizer$1.class
--rw-r--r--  2.0 unx     2578 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glrm/GlrmRegularizer.class
--rw-r--r--  2.0 unx     1219 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glrm/GlrmInitialization.class
--rw-r--r--  2.0 unx     1075 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glrm/GlrmLoss$2.class
--rw-r--r--  2.0 unx     2236 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glrm/GlrmLoss$9.class
--rw-r--r--  2.0 unx     1512 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glrm/GlrmLoss$6.class
--rw-r--r--  2.0 unx     1186 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glrm/GlrmLoss$3.class
--rw-r--r--  2.0 unx     1290 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glrm/GlrmRegularizer$4.class
--rw-r--r--  2.0 unx     1406 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glrm/GlrmRegularizer$7.class
--rw-r--r--  2.0 unx     9537 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glrm/GlrmMojoModel.class
--rw-r--r--  2.0 unx     1280 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glrm/GlrmRegularizer$5.class
--rw-r--r--  2.0 unx      983 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glrm/GlrmLoss$1.class
--rw-r--r--  2.0 unx     1510 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glrm/GlrmLoss$7.class
--rw-r--r--  2.0 unx     1460 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glrm/GlrmRegularizer$6.class
--rw-r--r--  2.0 unx     3178 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glrm/GlrmLoss.class
--rw-r--r--  2.0 unx     1499 b- defN 23-Oct-16 10:26 hex/genmodel/algos/glrm/GlrmLoss$4.class
--rw-r--r--  2.0 unx     1100 b- defN 23-Oct-16 10:26 hex/genmodel/ModelMojoReader$1.class
--rw-r--r--  2.0 unx      855 b- defN 23-Oct-16 10:26 hex/genmodel/MojoReaderBackendFactory$1.class
--rw-r--r--  2.0 unx     1934 b- defN 23-Oct-16 10:26 hex/genmodel/MultiModelMojoReader$NestedMojoReaderBackend.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/
--rw-r--r--  2.0 unx     1045 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/SharedTreeModelAttributes.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/metrics/
--rw-r--r--  2.0 unx      798 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/metrics/MojoModelMetricsOrdinalGLM.class
--rw-r--r--  2.0 unx      420 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/metrics/MojoModelMetricsSupervised.class
--rw-r--r--  2.0 unx      590 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/metrics/MojoModelMetricsRegression.class
--rw-r--r--  2.0 unx      802 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/metrics/MojoModelMetricsBinomialGLM.class
--rw-r--r--  2.0 unx      449 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/metrics/MojoModelMetricsAnomaly.class
--rw-r--r--  2.0 unx      630 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/metrics/MojoModelMetrics.class
--rw-r--r--  2.0 unx      748 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/metrics/MojoModelMetricsOrdinal.class
--rw-r--r--  2.0 unx      860 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/metrics/MojoModelMetricsBinomial.class
--rw-r--r--  2.0 unx      860 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/metrics/MojoModelMetricsMultinomial.class
--rw-r--r--  2.0 unx      810 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/metrics/MojoModelMetricsRegressionGLM.class
--rw-r--r--  2.0 unx      814 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/metrics/MojoModelMetricsMultinomialGLM.class
--rw-r--r--  2.0 unx      517 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/metrics/MojoModelMetricsRegressionCoxPH.class
--rw-r--r--  2.0 unx      993 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/DeepLearningModelAttributes.class
--rw-r--r--  2.0 unx     5653 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/ModelAttributes.class
--rw-r--r--  2.0 unx     1267 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/VariableImportances$1.class
--rw-r--r--  2.0 unx      495 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/SerializedName.class
--rw-r--r--  2.0 unx     2602 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/VariableImportances.class
--rw-r--r--  2.0 unx     1676 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/Table$ColumnType.class
--rw-r--r--  2.0 unx     1155 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/ModelAttributes$1.class
--rw-r--r--  2.0 unx     3376 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/Table.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/parameters/
--rw-r--r--  2.0 unx      874 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/parameters/ColumnSpecifier.class
--rw-r--r--  2.0 unx      249 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/parameters/VariableImportancesHolder.class
--rw-r--r--  2.0 unx      953 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/parameters/KeyValue.class
--rw-r--r--  2.0 unx     1892 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/parameters/ModelParameter.class
--rw-r--r--  2.0 unx     1319 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/parameters/ParameterKey$Type.class
--rw-r--r--  2.0 unx      880 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/parameters/FeatureContribution.class
--rw-r--r--  2.0 unx     1176 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/parameters/ParameterKey.class
--rw-r--r--  2.0 unx     1263 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/parameters/StringPair.class
--rw-r--r--  2.0 unx     1768 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/ModelJsonReader$1.class
--rw-r--r--  2.0 unx     2522 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/ModelJsonReader$TypeHint.class
--rw-r--r--  2.0 unx     1234 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/ModelAttributesGLM.class
--rw-r--r--  2.0 unx    15710 b- defN 23-Oct-16 10:26 hex/genmodel/attributes/ModelJsonReader.class
--rw-r--r--  2.0 unx     1541 b- defN 23-Oct-16 10:26 hex/genmodel/CategoricalEncoding$2.class
--rw-r--r--  2.0 unx     1551 b- defN 23-Oct-16 10:26 hex/genmodel/CategoricalEncoding$4.class
--rw-r--r--  2.0 unx     1127 b- defN 23-Oct-16 10:26 hex/genmodel/MojoPipelineBuilder$MappingSpec.class
--rw-r--r--  2.0 unx     5145 b- defN 23-Oct-16 10:26 hex/genmodel/ModelMojoFactory.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 water/
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 water/util/
--rw-r--r--  2.0 unx     4898 b- defN 23-Oct-16 10:26 water/util/ParseTime.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 water/util/comparison/
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 water/util/comparison/string/
--rw-r--r--  2.0 unx     1597 b- defN 23-Oct-16 10:26 water/util/comparison/string/JaccardIndexComparator.class
--rw-r--r--  2.0 unx      865 b- defN 23-Oct-16 10:26 water/util/comparison/string/LongestCommonSubstring$Formula$3.class
--rw-r--r--  2.0 unx      272 b- defN 23-Oct-16 10:26 water/util/comparison/string/LongestCommonSubstring$1.class
--rw-r--r--  2.0 unx     2471 b- defN 23-Oct-16 10:26 water/util/comparison/string/QGramComparator$Formula.class
--rw-r--r--  2.0 unx     1804 b- defN 23-Oct-16 10:26 water/util/comparison/string/SoundexComparator.class
--rw-r--r--  2.0 unx     1908 b- defN 23-Oct-16 10:26 water/util/comparison/string/StringComparatorFactory.class
--rw-r--r--  2.0 unx      865 b- defN 23-Oct-16 10:26 water/util/comparison/string/LongestCommonSubstring$Formula$2.class
--rw-r--r--  2.0 unx     1101 b- defN 23-Oct-16 10:26 water/util/comparison/string/QGramComparator$Formula$3.class
--rw-r--r--  2.0 unx     2359 b- defN 23-Oct-16 10:26 water/util/comparison/string/LongestCommonSubstring$Formula.class
--rw-r--r--  2.0 unx     2346 b- defN 23-Oct-16 10:26 water/util/comparison/string/QGramComparator$Tokenizer.class
--rw-r--r--  2.0 unx      861 b- defN 23-Oct-16 10:26 water/util/comparison/string/LongestCommonSubstring$Formula$1.class
--rw-r--r--  2.0 unx     2936 b- defN 23-Oct-16 10:26 water/util/comparison/string/QGramComparator.class
--rw-r--r--  2.0 unx     1416 b- defN 23-Oct-16 10:26 water/util/comparison/string/StringUtils.class
--rw-r--r--  2.0 unx     2744 b- defN 23-Oct-16 10:26 water/util/comparison/string/LongestCommonSubstring.class
--rw-r--r--  2.0 unx     1566 b- defN 23-Oct-16 10:26 water/util/comparison/string/QGramComparator$Tokenizer$3.class
--rw-r--r--  2.0 unx     1540 b- defN 23-Oct-16 10:26 water/util/comparison/string/QGramComparator$Tokenizer$2.class
--rw-r--r--  2.0 unx      251 b- defN 23-Oct-16 10:26 water/util/comparison/string/QGramComparator$1.class
--rw-r--r--  2.0 unx      230 b- defN 23-Oct-16 10:26 water/util/comparison/string/StringComparator.class
--rw-r--r--  2.0 unx     1336 b- defN 23-Oct-16 10:26 water/util/comparison/string/QGramComparator$Tokenizer$1.class
--rw-r--r--  2.0 unx     1135 b- defN 23-Oct-16 10:26 water/util/comparison/string/QGramComparator$Formula$1.class
--rw-r--r--  2.0 unx     1637 b- defN 23-Oct-16 10:26 water/util/comparison/string/LevenshteinDistanceComparator.class
--rw-r--r--  2.0 unx     2090 b- defN 23-Oct-16 10:26 water/util/comparison/string/H2OJaroWinklerComparator.class
--rw-r--r--  2.0 unx     1090 b- defN 23-Oct-16 10:26 water/util/comparison/string/QGramComparator$Formula$2.class
--rw-r--r--  2.0 unx      724 b- defN 23-Oct-16 10:26 water/util/comparison/string/ExactComparator.class
--rw-r--r--  2.0 unx    10148 b- defN 23-Oct-16 10:26 water/util/H2OPredictor.class
--rw-r--r--  2.0 unx      606 b- defN 23-Oct-16 10:26 water/util/H2OPredictor$1.class
--rw-r--r--  2.0 unx     2742 b- defN 23-Oct-16 10:26 water/util/JavaVersionUtils.class
--rw-r--r--  2.0 unx      971 b- defN 23-Oct-16 10:26 water/util/ModelUtils.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:26 water/genmodel/
--rw-r--r--  2.0 unx      873 b- defN 23-Oct-16 10:26 water/genmodel/AbstractBuildVersion$1.class
--rw-r--r--  2.0 unx     2965 b- defN 23-Oct-16 10:26 water/genmodel/AbstractBuildVersion.class
--rw-r--r--  2.0 unx      922 b- defN 23-Oct-16 10:26 water/genmodel/BuildVersion.class
--rw-r--r--  2.0 unx      921 b- defN 23-Oct-16 10:26 water/genmodel/IGeneratedModel.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Oct-16 10:27 META-INF/services/
--rw-r--r--  2.0 unx       29 b- defN 23-Oct-16 10:27 META-INF/services/hex.genmodel.tools.MojoPrinter
-391 files, 815480 bytes uncompressed, 399530 bytes compressed:  51.0%
+Zip file size: 466825 bytes, number of entries: 392
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:51 META-INF/
+-rw-r--r--  2.0 unx       25 b- defN 23-Nov-08 09:51 META-INF/MANIFEST.MF
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/
+-rw-r--r--  2.0 unx     1699 b- defN 23-Nov-08 09:50 hex/ModelCategory.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/descriptor/
+-rw-r--r--  2.0 unx      757 b- defN 23-Nov-08 09:50 hex/genmodel/descriptor/ModelDescriptor.class
+-rw-r--r--  2.0 unx     3908 b- defN 23-Nov-08 09:50 hex/genmodel/descriptor/ModelDescriptorBuilder$PojoModelDescriptor.class
+-rw-r--r--  2.0 unx      262 b- defN 23-Nov-08 09:50 hex/genmodel/descriptor/ModelDescriptorBuilder$1.class
+-rw-r--r--  2.0 unx     1415 b- defN 23-Nov-08 09:50 hex/genmodel/descriptor/ModelDescriptorBuilder.class
+-rw-r--r--  2.0 unx     4711 b- defN 23-Nov-08 09:50 hex/genmodel/descriptor/ModelDescriptorBuilder$MojoModelDescriptor.class
+-rw-r--r--  2.0 unx     1088 b- defN 23-Nov-08 09:50 hex/genmodel/ModelMojoReader$RawValue.class
+-rw-r--r--  2.0 unx     5067 b- defN 23-Nov-08 09:50 hex/genmodel/MojoReaderBackendFactory.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/easy/
+-rw-r--r--  2.0 unx     2069 b- defN 23-Nov-08 09:50 hex/genmodel/easy/EnumLimitedEncoderDomainMapConstructor.class
+-rw-r--r--  2.0 unx     1698 b- defN 23-Nov-08 09:50 hex/genmodel/easy/EnumEncoder.class
+-rw-r--r--  2.0 unx     1570 b- defN 23-Nov-08 09:50 hex/genmodel/easy/EigenEncoder.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/easy/prediction/
+-rw-r--r--  2.0 unx      549 b- defN 23-Nov-08 09:50 hex/genmodel/easy/prediction/AutoEncoderModelPrediction.class
+-rw-r--r--  2.0 unx      365 b- defN 23-Nov-08 09:50 hex/genmodel/easy/prediction/AbstractPrediction.class
+-rw-r--r--  2.0 unx     1159 b- defN 23-Nov-08 09:50 hex/genmodel/easy/prediction/AnomalyDetectionPrediction.class
+-rw-r--r--  2.0 unx      476 b- defN 23-Nov-08 09:50 hex/genmodel/easy/prediction/OrdinalModelPrediction.class
+-rw-r--r--  2.0 unx      394 b- defN 23-Nov-08 09:50 hex/genmodel/easy/prediction/CoxPHModelPrediction.class
+-rw-r--r--  2.0 unx      455 b- defN 23-Nov-08 09:50 hex/genmodel/easy/prediction/ClusteringModelPrediction.class
+-rw-r--r--  2.0 unx      683 b- defN 23-Nov-08 09:50 hex/genmodel/easy/prediction/SortedClassProbability.class
+-rw-r--r--  2.0 unx      428 b- defN 23-Nov-08 09:50 hex/genmodel/easy/prediction/UpliftBinomialModelPrediction.class
+-rw-r--r--  2.0 unx      606 b- defN 23-Nov-08 09:50 hex/genmodel/easy/prediction/MultinomialModelPrediction.class
+-rw-r--r--  2.0 unx      479 b- defN 23-Nov-08 09:50 hex/genmodel/easy/prediction/Word2VecPrediction.class
+-rw-r--r--  2.0 unx      665 b- defN 23-Nov-08 09:50 hex/genmodel/easy/prediction/BinomialModelPrediction.class
+-rw-r--r--  2.0 unx      445 b- defN 23-Nov-08 09:50 hex/genmodel/easy/prediction/DimReductionModelPrediction.class
+-rw-r--r--  2.0 unx      561 b- defN 23-Nov-08 09:50 hex/genmodel/easy/prediction/RegressionModelPrediction.class
+-rw-r--r--  2.0 unx      414 b- defN 23-Nov-08 09:50 hex/genmodel/easy/prediction/TargetEncoderPrediction.class
+-rw-r--r--  2.0 unx      430 b- defN 23-Nov-08 09:50 hex/genmodel/easy/prediction/KLimeModelPrediction.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/easy/exception/
+-rw-r--r--  2.0 unx      454 b- defN 23-Nov-08 09:50 hex/genmodel/easy/exception/PredictUnknownTypeException.class
+-rw-r--r--  2.0 unx      683 b- defN 23-Nov-08 09:50 hex/genmodel/easy/exception/PredictException.class
+-rw-r--r--  2.0 unx      457 b- defN 23-Nov-08 09:50 hex/genmodel/easy/exception/PredictNumberFormatException.class
+-rw-r--r--  2.0 unx      475 b- defN 23-Nov-08 09:50 hex/genmodel/easy/exception/PredictWrongModelCategoryException.class
+-rw-r--r--  2.0 unx      831 b- defN 23-Nov-08 09:50 hex/genmodel/easy/exception/PredictUnknownCategoricalLevelException.class
+-rw-r--r--  2.0 unx     1302 b- defN 23-Nov-08 09:50 hex/genmodel/easy/EnumEncoderColumnMapper.class
+-rw-r--r--  2.0 unx     1309 b- defN 23-Nov-08 09:50 hex/genmodel/easy/EigenEncoderColumnMapper.class
+-rw-r--r--  2.0 unx    24456 b- defN 23-Nov-08 09:50 hex/genmodel/easy/EasyPredictModelWrapper.class
+-rw-r--r--  2.0 unx     5805 b- defN 23-Nov-08 09:50 hex/genmodel/easy/EasyPredictModelWrapper$Config.class
+-rw-r--r--  2.0 unx      621 b- defN 23-Nov-08 09:50 hex/genmodel/easy/EnumLimitedEncoderColumnMapper.class
+-rw-r--r--  2.0 unx      241 b- defN 23-Nov-08 09:50 hex/genmodel/easy/CategoricalEncoder.class
+-rw-r--r--  2.0 unx     5444 b- defN 23-Nov-08 09:50 hex/genmodel/easy/RowToRawDataConverter.class
+-rw-r--r--  2.0 unx      363 b- defN 23-Nov-08 09:50 hex/genmodel/easy/RowData.class
+-rw-r--r--  2.0 unx      597 b- defN 23-Nov-08 09:50 hex/genmodel/easy/EasyPredictModelWrapper$ErrorConsumer.class
+-rw-r--r--  2.0 unx     1939 b- defN 23-Nov-08 09:50 hex/genmodel/easy/LabelEncoderDomainMapConstructor.class
+-rw-r--r--  2.0 unx     1591 b- defN 23-Nov-08 09:50 hex/genmodel/easy/BinaryColumnMapper.class
+-rw-r--r--  2.0 unx      872 b- defN 23-Nov-08 09:50 hex/genmodel/easy/DomainMapConstructor.class
+-rw-r--r--  2.0 unx     1941 b- defN 23-Nov-08 09:50 hex/genmodel/easy/BinaryDomainMapConstructor.class
+-rw-r--r--  2.0 unx     1570 b- defN 23-Nov-08 09:50 hex/genmodel/easy/OneHotEncoderColumnMapper.class
+-rw-r--r--  2.0 unx     1962 b- defN 23-Nov-08 09:50 hex/genmodel/easy/OneHotEncoderDomainMapConstructor.class
+-rw-r--r--  2.0 unx     2357 b- defN 23-Nov-08 09:50 hex/genmodel/easy/EnumLimitedEncoder.class
+-rw-r--r--  2.0 unx     2209 b- defN 23-Nov-08 09:50 hex/genmodel/easy/OneHotEncoder.class
+-rw-r--r--  2.0 unx     2290 b- defN 23-Nov-08 09:50 hex/genmodel/easy/BinaryEncoder.class
+-rw-r--r--  2.0 unx     1633 b- defN 23-Nov-08 09:50 hex/genmodel/easy/LabelEncoder.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/easy/error/
+-rw-r--r--  2.0 unx      805 b- defN 23-Nov-08 09:50 hex/genmodel/easy/error/VoidErrorConsumer.class
+-rw-r--r--  2.0 unx      702 b- defN 23-Nov-08 09:50 hex/genmodel/easy/error/CountingErrorConsumer$Config.class
+-rw-r--r--  2.0 unx     5332 b- defN 23-Nov-08 09:50 hex/genmodel/easy/error/CountingErrorConsumer.class
+-rw-r--r--  2.0 unx     1325 b- defN 23-Nov-08 09:50 hex/genmodel/easy/EasyPredictModelWrapper$1.class
+-rw-r--r--  2.0 unx     1876 b- defN 23-Nov-08 09:50 hex/genmodel/easy/EnumEncoderDomainMapConstructor.class
+-rw-r--r--  2.0 unx     2146 b- defN 23-Nov-08 09:50 hex/genmodel/easy/EigenEncoderDomainMapConstructor.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/tools/
+-rw-r--r--  2.0 unx     1287 b- defN 23-Nov-08 09:50 hex/genmodel/tools/PrintMojo$FloatCastingSerializer.class
+-rw-r--r--  2.0 unx     1026 b- defN 23-Nov-08 09:50 hex/genmodel/tools/PredictCsv$1.class
+-rw-r--r--  2.0 unx     5410 b- defN 23-Nov-08 09:50 hex/genmodel/tools/MungeCsv.class
+-rw-r--r--  2.0 unx     1010 b- defN 23-Nov-08 09:50 hex/genmodel/tools/PrintMojo$PrintTreeOptions.class
+-rw-r--r--  2.0 unx    20777 b- defN 23-Nov-08 09:50 hex/genmodel/tools/PredictCsv.class
+-rw-r--r--  2.0 unx    14133 b- defN 23-Nov-08 09:50 hex/genmodel/tools/PrintMojo.class
+-rw-r--r--  2.0 unx     1286 b- defN 23-Nov-08 09:50 hex/genmodel/tools/PredictCsv$PredictCsvCollection.class
+-rw-r--r--  2.0 unx     4591 b- defN 23-Nov-08 09:50 hex/genmodel/tools/PredictCsv$PredictCsvBuilder.class
+-rw-r--r--  2.0 unx      826 b- defN 23-Nov-08 09:50 hex/genmodel/tools/PrintMojo$2.class
+-rw-r--r--  2.0 unx      722 b- defN 23-Nov-08 09:50 hex/genmodel/tools/PrintMojo$1.class
+-rw-r--r--  2.0 unx     7956 b- defN 23-Nov-08 09:50 hex/genmodel/tools/BuildPipeline.class
+-rw-r--r--  2.0 unx     1294 b- defN 23-Nov-08 09:50 hex/genmodel/tools/PredictCsv$PredictCsvCallable.class
+-rw-r--r--  2.0 unx     1202 b- defN 23-Nov-08 09:50 hex/genmodel/tools/MojoPrinter$Format.class
+-rw-r--r--  2.0 unx      388 b- defN 23-Nov-08 09:50 hex/genmodel/tools/MojoPrinter.class
+-rw-r--r--  2.0 unx      895 b- defN 23-Nov-08 09:50 hex/genmodel/ConverterFactoryProvidingModel.class
+-rw-r--r--  2.0 unx     1538 b- defN 23-Nov-08 09:50 hex/genmodel/CategoricalEncoding$6.class
+-rw-r--r--  2.0 unx     2779 b- defN 23-Nov-08 09:50 hex/genmodel/MultiModelMojoReader.class
+-rw-r--r--  2.0 unx     1583 b- defN 23-Nov-08 09:50 hex/genmodel/GenMunger$Step.class
+-rw-r--r--  2.0 unx     1277 b- defN 23-Nov-08 09:50 hex/genmodel/GenModel$1.class
+-rw-r--r--  2.0 unx     1403 b- defN 23-Nov-08 09:50 hex/genmodel/TmpMojoReaderBackend.class
+-rw-r--r--  2.0 unx      215 b- defN 23-Nov-08 09:50 hex/genmodel/IClusteringModel.class
+-rw-r--r--  2.0 unx     2445 b- defN 23-Nov-08 09:50 hex/genmodel/CategoricalEncoding.class
+-rw-r--r--  2.0 unx     6310 b- defN 23-Nov-08 09:50 hex/genmodel/MojoPipelineBuilder.class
+-rw-r--r--  2.0 unx     2276 b- defN 23-Nov-08 09:50 hex/genmodel/InMemoryMojoReaderBackend.class
+-rw-r--r--  2.0 unx     5604 b- defN 23-Nov-08 09:50 hex/genmodel/MojoPipelineWriter.class
+-rw-r--r--  2.0 unx     1729 b- defN 23-Nov-08 09:50 hex/genmodel/FolderMojoReaderBackend.class
+-rw-r--r--  2.0 unx     1489 b- defN 23-Nov-08 09:50 hex/genmodel/CategoricalEncoding$1.class
+-rw-r--r--  2.0 unx      225 b- defN 23-Nov-08 09:50 hex/genmodel/PredictContributionsFactory.class
+-rw-r--r--  2.0 unx      334 b- defN 23-Nov-08 09:50 hex/genmodel/PredictContributions.class
+-rw-r--r--  2.0 unx     4391 b- defN 23-Nov-08 09:50 hex/genmodel/MojoPipelineWriter$MojoPipelineDescriptor.class
+-rw-r--r--  2.0 unx      234 b- defN 23-Nov-08 09:50 hex/genmodel/MultiModelMojoReader$1.class
+-rw-r--r--  2.0 unx     9766 b- defN 23-Nov-08 09:50 hex/genmodel/AbstractMojoWriter.class
+-rw-r--r--  2.0 unx     3008 b- defN 23-Nov-08 09:50 hex/genmodel/MojoModel.class
+-rw-r--r--  2.0 unx      228 b- defN 23-Nov-08 09:50 hex/genmodel/MojoPipelineWriter$1.class
+-rw-r--r--  2.0 unx      345 b- defN 23-Nov-08 09:50 hex/genmodel/MojoReaderBackend.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/utils/
+-rw-r--r--  2.0 unx     1366 b- defN 23-Nov-08 09:50 hex/genmodel/utils/StringEscapeUtils.class
+-rw-r--r--  2.0 unx      770 b- defN 23-Nov-08 09:50 hex/genmodel/utils/IOUtils.class
+-rw-r--r--  2.0 unx     7386 b- defN 23-Nov-08 09:50 hex/genmodel/utils/ArrayUtils.class
+-rw-r--r--  2.0 unx     3399 b- defN 23-Nov-08 09:50 hex/genmodel/utils/ParseUtils.class
+-rw-r--r--  2.0 unx     1869 b- defN 23-Nov-08 09:50 hex/genmodel/utils/ByteBufferWrapper.class
+-rw-r--r--  2.0 unx     1329 b- defN 23-Nov-08 09:50 hex/genmodel/utils/MathUtils.class
+-rw-r--r--  2.0 unx      988 b- defN 23-Nov-08 09:50 hex/genmodel/utils/ArrayUtils$1.class
+-rw-r--r--  2.0 unx     1361 b- defN 23-Nov-08 09:50 hex/genmodel/utils/LinkFunctionType.class
+-rw-r--r--  2.0 unx     1862 b- defN 23-Nov-08 09:50 hex/genmodel/utils/DistributionFamily.class
+-rw-r--r--  2.0 unx     3320 b- defN 23-Nov-08 09:50 hex/genmodel/utils/GenmodelBitSet.class
+-rw-r--r--  2.0 unx     1206 b- defN 23-Nov-08 09:50 hex/genmodel/utils/ArrayUtils$2.class
+-rw-r--r--  2.0 unx     1234 b- defN 23-Nov-08 09:50 hex/genmodel/MojoReaderBackendFactory$CachingStrategy.class
+-rw-r--r--  2.0 unx     8569 b- defN 23-Nov-08 09:50 hex/genmodel/GenMunger.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/annotations/
+-rw-r--r--  2.0 unx      521 b- defN 23-Nov-08 09:50 hex/genmodel/annotations/ModelPojo.class
+-rw-r--r--  2.0 unx     1527 b- defN 23-Nov-08 09:50 hex/genmodel/CategoricalEncoding$3.class
+-rw-r--r--  2.0 unx      398 b- defN 23-Nov-08 09:50 hex/genmodel/IGenModel.class
+-rw-r--r--  2.0 unx     1539 b- defN 23-Nov-08 09:50 hex/genmodel/CategoricalEncoding$5.class
+-rw-r--r--  2.0 unx     1268 b- defN 23-Nov-08 09:50 hex/genmodel/NestedMojoReaderBackend.class
+-rw-r--r--  2.0 unx    15640 b- defN 23-Nov-08 09:50 hex/genmodel/ModelMojoReader.class
+-rw-r--r--  2.0 unx     2041 b- defN 23-Nov-08 09:50 hex/genmodel/ZipfileMojoReaderBackend.class
+-rw-r--r--  2.0 unx    19329 b- defN 23-Nov-08 09:50 hex/genmodel/GenModel.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/algos/
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/algos/svm/
+-rw-r--r--  2.0 unx     1887 b- defN 23-Nov-08 09:50 hex/genmodel/algos/svm/SvmMojoReader.class
+-rw-r--r--  2.0 unx     1340 b- defN 23-Nov-08 09:50 hex/genmodel/algos/svm/SvmMojoModel.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/algos/upliftdrf/
+-rw-r--r--  2.0 unx     1699 b- defN 23-Nov-08 09:50 hex/genmodel/algos/upliftdrf/UpliftDrfMojoModel.class
+-rw-r--r--  2.0 unx     2172 b- defN 23-Nov-08 09:50 hex/genmodel/algos/upliftdrf/UpliftDrfMojoReader.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/algos/klime/
+-rw-r--r--  2.0 unx     2319 b- defN 23-Nov-08 09:50 hex/genmodel/algos/klime/KLimeMojoModel.class
+-rw-r--r--  2.0 unx     2687 b- defN 23-Nov-08 09:50 hex/genmodel/algos/klime/KLimeMojoReader.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/algos/word2vec/
+-rw-r--r--  2.0 unx     1490 b- defN 23-Nov-08 09:50 hex/genmodel/algos/word2vec/Word2VecMojoModel.class
+-rw-r--r--  2.0 unx     3174 b- defN 23-Nov-08 09:50 hex/genmodel/algos/word2vec/Word2VecMojoReader.class
+-rw-r--r--  2.0 unx      220 b- defN 23-Nov-08 09:50 hex/genmodel/algos/word2vec/WordEmbeddingModel.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/algos/rulefit/
+-rw-r--r--  2.0 unx      863 b- defN 23-Nov-08 09:50 hex/genmodel/algos/rulefit/MojoRule.class
+-rw-r--r--  2.0 unx     1620 b- defN 23-Nov-08 09:50 hex/genmodel/algos/rulefit/MojoCondition.class
+-rw-r--r--  2.0 unx     2502 b- defN 23-Nov-08 09:50 hex/genmodel/algos/rulefit/RuleFitMojoModel.class
+-rw-r--r--  2.0 unx     7385 b- defN 23-Nov-08 09:50 hex/genmodel/algos/rulefit/RuleFitMojoReader.class
+-rw-r--r--  2.0 unx     3386 b- defN 23-Nov-08 09:50 hex/genmodel/algos/rulefit/MojoRuleEnsemble.class
+-rw-r--r--  2.0 unx     1177 b- defN 23-Nov-08 09:50 hex/genmodel/algos/rulefit/MojoCondition$Type.class
+-rw-r--r--  2.0 unx     1286 b- defN 23-Nov-08 09:50 hex/genmodel/algos/rulefit/RuleFitMojoModel$ModelType.class
+-rw-r--r--  2.0 unx     1256 b- defN 23-Nov-08 09:50 hex/genmodel/algos/rulefit/MojoCondition$Operator.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/
+-rw-r--r--  2.0 unx      263 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/TreeSHAPPredictor$Workspace.class
+-rw-r--r--  2.0 unx     3299 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/SharedTreeMojoModel$AuxInfoLightReader.class
+-rw-r--r--  2.0 unx      880 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/TreeSHAP$PathElement.class
+-rw-r--r--  2.0 unx     4714 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/SharedTreeMojoReader.class
+-rw-r--r--  2.0 unx      353 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/SharedTreeGraphConverter.class
+-rw-r--r--  2.0 unx      657 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/ScoreTree0.class
+-rw-r--r--  2.0 unx      202 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/ScoreTree.class
+-rw-r--r--  2.0 unx      220 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/TreeSHAP$1.class
+-rw-r--r--  2.0 unx      635 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/ScoreTree2.class
+-rw-r--r--  2.0 unx     1101 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/ConvertTreeOptions.class
+-rw-r--r--  2.0 unx     8018 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/SharedTreeSubgraph.class
+-rw-r--r--  2.0 unx     3434 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/TreeSHAPEnsemble.class
+-rw-r--r--  2.0 unx    11309 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/TreeSHAP.class
+-rw-r--r--  2.0 unx      253 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/SharedTreeMojoModel$1.class
+-rw-r--r--  2.0 unx      535 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/SharedTreeMojoModel$LeafNodeAssignments.class
+-rw-r--r--  2.0 unx      438 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/SharedTreeMojoModel$DecisionPathTracker.class
+-rw-r--r--  2.0 unx     2835 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/SharedTreeMojoModelWithContributions.class
+-rw-r--r--  2.0 unx      657 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/ScoreTree1.class
+-rw-r--r--  2.0 unx      833 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/TreeSHAPPredictor.class
+-rw-r--r--  2.0 unx    16477 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/SharedTreeNode.class
+-rw-r--r--  2.0 unx     1175 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/CalibrationMojoHelper.class
+-rw-r--r--  2.0 unx     2634 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/ContributionComposer.class
+-rw-r--r--  2.0 unx      602 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/ScoreIsolationTree0.class
+-rw-r--r--  2.0 unx     1395 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/NaSplitDir.class
+-rw-r--r--  2.0 unx     3003 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/SharedTreeMojoModel$LeafDecisionPathTracker.class
+-rw-r--r--  2.0 unx      611 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/TreeBackedMojoModel.class
+-rw-r--r--  2.0 unx     3699 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/SharedTreeGraph.class
+-rw-r--r--  2.0 unx    25057 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/SharedTreeMojoModel.class
+-rw-r--r--  2.0 unx     1518 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/SharedTreeMojoModelWithContributions$SharedTreeContributionsPredictor.class
+-rw-r--r--  2.0 unx     1707 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/TreeSHAP$PathPointer.class
+-rw-r--r--  2.0 unx      199 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/ScoreIsolationTree.class
+-rw-r--r--  2.0 unx     1445 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/SharedTreeMojoModel$StringDecisionPathTracker.class
+-rw-r--r--  2.0 unx      399 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/CalibrationMojoHelper$MojoModelWithCalibration.class
+-rw-r--r--  2.0 unx     3805 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/ContributionsPredictor.class
+-rw-r--r--  2.0 unx     2632 b- defN 23-Nov-08 09:50 hex/genmodel/algos/tree/SharedTreeMojoModel$AuxInfo.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/algos/coxph/
+-rw-r--r--  2.0 unx     6398 b- defN 23-Nov-08 09:50 hex/genmodel/algos/coxph/CoxPHMojoModel.class
+-rw-r--r--  2.0 unx     1311 b- defN 23-Nov-08 09:50 hex/genmodel/algos/coxph/CoxPHMojoModel$InteractionTypes.class
+-rw-r--r--  2.0 unx     1144 b- defN 23-Nov-08 09:50 hex/genmodel/algos/coxph/CoxPHMojoModel$Strata.class
+-rw-r--r--  2.0 unx     5061 b- defN 23-Nov-08 09:50 hex/genmodel/algos/coxph/CoxPHMojoReader.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/algos/drf/
+-rw-r--r--  2.0 unx     1633 b- defN 23-Nov-08 09:50 hex/genmodel/algos/drf/DrfMojoReader.class
+-rw-r--r--  2.0 unx      230 b- defN 23-Nov-08 09:50 hex/genmodel/algos/drf/DrfMojoModel$1.class
+-rw-r--r--  2.0 unx     3129 b- defN 23-Nov-08 09:50 hex/genmodel/algos/drf/DrfMojoModel$ContributionsPredictorDRF.class
+-rw-r--r--  2.0 unx     2700 b- defN 23-Nov-08 09:50 hex/genmodel/algos/drf/DrfMojoModel.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/algos/isoforextended/
+-rw-r--r--  2.0 unx     4170 b- defN 23-Nov-08 09:50 hex/genmodel/algos/isoforextended/ExtendedIsolationForestMojoModel.class
+-rw-r--r--  2.0 unx     2306 b- defN 23-Nov-08 09:50 hex/genmodel/algos/isoforextended/ExtendedIsolationForestMojoReader.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/algos/pca/
+-rw-r--r--  2.0 unx     2645 b- defN 23-Nov-08 09:50 hex/genmodel/algos/pca/PCAMojoModel.class
+-rw-r--r--  2.0 unx     2819 b- defN 23-Nov-08 09:50 hex/genmodel/algos/pca/PCAMojoReader.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glm/
+-rw-r--r--  2.0 unx     4318 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glm/GlmMojoModel.class
+-rw-r--r--  2.0 unx     2466 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glm/GlmMultinomialMojoModel.class
+-rw-r--r--  2.0 unx     1747 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glm/GlmMojoModelBase.class
+-rw-r--r--  2.0 unx      848 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glm/GlmMojoModel$GLM_inverseInv.class
+-rw-r--r--  2.0 unx      851 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glm/GlmMojoModel$GLM_identityInv.class
+-rw-r--r--  2.0 unx      230 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glm/GlmMojoModel$1.class
+-rw-r--r--  2.0 unx     2647 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glm/GlmOrdinalMojoModel.class
+-rw-r--r--  2.0 unx      836 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glm/GlmMojoModel$GLM_logInv.class
+-rw-r--r--  2.0 unx      626 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glm/GlmMojoModel$GLM_ologitInv.class
+-rw-r--r--  2.0 unx      272 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glm/GlmMojoModel$Function1.class
+-rw-r--r--  2.0 unx      724 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glm/GlmMojoModel$GLM_tweedieInv.class
+-rw-r--r--  2.0 unx      842 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glm/GlmMojoModel$GLM_logitInv.class
+-rw-r--r--  2.0 unx     3584 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glm/GlmMojoReader.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/algos/targetencoder/
+-rw-r--r--  2.0 unx      677 b- defN 23-Nov-08 09:50 hex/genmodel/algos/targetencoder/ColumnsMapping.class
+-rw-r--r--  2.0 unx     3493 b- defN 23-Nov-08 09:50 hex/genmodel/algos/targetencoder/EncodingMap.class
+-rw-r--r--  2.0 unx     9375 b- defN 23-Nov-08 09:50 hex/genmodel/algos/targetencoder/TargetEncoderMojoReader.class
+-rw-r--r--  2.0 unx     2436 b- defN 23-Nov-08 09:50 hex/genmodel/algos/targetencoder/EncodingMaps.class
+-rw-r--r--  2.0 unx     1417 b- defN 23-Nov-08 09:50 hex/genmodel/algos/targetencoder/ColumnsToSingleMapping.class
+-rw-r--r--  2.0 unx     8265 b- defN 23-Nov-08 09:50 hex/genmodel/algos/targetencoder/TargetEncoderMojoModel.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/algos/isotonic/
+-rw-r--r--  2.0 unx      888 b- defN 23-Nov-08 09:50 hex/genmodel/algos/isotonic/IsotonicCalibrator.class
+-rw-r--r--  2.0 unx      874 b- defN 23-Nov-08 09:50 hex/genmodel/algos/isotonic/IsotonicRegressionMojoModel.class
+-rw-r--r--  2.0 unx     1676 b- defN 23-Nov-08 09:50 hex/genmodel/algos/isotonic/IsotonicRegressionMojoReader.class
+-rw-r--r--  2.0 unx     1680 b- defN 23-Nov-08 09:50 hex/genmodel/algos/isotonic/IsotonicRegressionUtils.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/algos/deeplearning/
+-rw-r--r--  2.0 unx      783 b- defN 23-Nov-08 09:50 hex/genmodel/algos/deeplearning/ActivationUtils$RectifierDropoutOut.class
+-rw-r--r--  2.0 unx     5224 b- defN 23-Nov-08 09:50 hex/genmodel/algos/deeplearning/DeeplearningMojoReader.class
+-rw-r--r--  2.0 unx     1081 b- defN 23-Nov-08 09:50 hex/genmodel/algos/deeplearning/ActivationUtils$SoftmaxOut.class
+-rw-r--r--  2.0 unx      769 b- defN 23-Nov-08 09:50 hex/genmodel/algos/deeplearning/ActivationUtils$MaxoutDropoutOut.class
+-rw-r--r--  2.0 unx      709 b- defN 23-Nov-08 09:50 hex/genmodel/algos/deeplearning/ActivationUtils$LinearOut.class
+-rw-r--r--  2.0 unx     1096 b- defN 23-Nov-08 09:50 hex/genmodel/algos/deeplearning/DeeplearningMojoModel$1.class
+-rw-r--r--  2.0 unx     6719 b- defN 23-Nov-08 09:50 hex/genmodel/algos/deeplearning/NeuralNetwork.class
+-rw-r--r--  2.0 unx      934 b- defN 23-Nov-08 09:50 hex/genmodel/algos/deeplearning/ActivationUtils$RectifierOut.class
+-rw-r--r--  2.0 unx      323 b- defN 23-Nov-08 09:50 hex/genmodel/algos/deeplearning/ActivationUtils$ActivationFunctions.class
+-rw-r--r--  2.0 unx     2132 b- defN 23-Nov-08 09:50 hex/genmodel/algos/deeplearning/ActivationUtils.class
+-rw-r--r--  2.0 unx      798 b- defN 23-Nov-08 09:50 hex/genmodel/algos/deeplearning/ActivationUtils$ExpRectifierDropoutOut.class
+-rw-r--r--  2.0 unx      663 b- defN 23-Nov-08 09:50 hex/genmodel/algos/deeplearning/DeeplearningMojoModel$StoreWeightsBias.class
+-rw-r--r--  2.0 unx     6843 b- defN 23-Nov-08 09:50 hex/genmodel/algos/deeplearning/DeeplearningMojoModel.class
+-rw-r--r--  2.0 unx      787 b- defN 23-Nov-08 09:50 hex/genmodel/algos/deeplearning/ActivationUtils$TanhDropoutOut.class
+-rw-r--r--  2.0 unx      995 b- defN 23-Nov-08 09:50 hex/genmodel/algos/deeplearning/ActivationUtils$ExpRectifierOut.class
+-rw-r--r--  2.0 unx      922 b- defN 23-Nov-08 09:50 hex/genmodel/algos/deeplearning/ActivationUtils$TanhOut.class
+-rw-r--r--  2.0 unx     1007 b- defN 23-Nov-08 09:50 hex/genmodel/algos/deeplearning/ActivationUtils$MaxoutOut.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/algos/psvm/
+-rw-r--r--  2.0 unx      196 b- defN 23-Nov-08 09:50 hex/genmodel/algos/psvm/SupportVectorScorer.class
+-rw-r--r--  2.0 unx      422 b- defN 23-Nov-08 09:50 hex/genmodel/algos/psvm/KernelParameters.class
+-rw-r--r--  2.0 unx     1388 b- defN 23-Nov-08 09:50 hex/genmodel/algos/psvm/ScorerFactory.class
+-rw-r--r--  2.0 unx     1550 b- defN 23-Nov-08 09:50 hex/genmodel/algos/psvm/GaussianScorer.class
+-rw-r--r--  2.0 unx      973 b- defN 23-Nov-08 09:50 hex/genmodel/algos/psvm/KernelType.class
+-rw-r--r--  2.0 unx      699 b- defN 23-Nov-08 09:50 hex/genmodel/algos/psvm/ScorerFactory$1.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/algos/ensemble/
+-rw-r--r--  2.0 unx     3993 b- defN 23-Nov-08 09:50 hex/genmodel/algos/ensemble/StackedEnsembleMojoReader.class
+-rw-r--r--  2.0 unx      974 b- defN 23-Nov-08 09:50 hex/genmodel/algos/ensemble/StackedEnsembleMojoModel$StackedEnsembleMojoSubModel.class
+-rw-r--r--  2.0 unx     2165 b- defN 23-Nov-08 09:50 hex/genmodel/algos/ensemble/StackedEnsembleMojoModel.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/algos/isofor/
+-rw-r--r--  2.0 unx     1835 b- defN 23-Nov-08 09:50 hex/genmodel/algos/isofor/IsolationForestMojoModel.class
+-rw-r--r--  2.0 unx     2021 b- defN 23-Nov-08 09:50 hex/genmodel/algos/isofor/IsolationForestMojoReader.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/algos/gam/
+-rw-r--r--  2.0 unx     1572 b- defN 23-Nov-08 09:50 hex/genmodel/algos/gam/GamMojoModel.class
+-rw-r--r--  2.0 unx     2046 b- defN 23-Nov-08 09:50 hex/genmodel/algos/gam/ISplines.class
+-rw-r--r--  2.0 unx     2045 b- defN 23-Nov-08 09:50 hex/genmodel/algos/gam/NBSplinesTypeII.class
+-rw-r--r--  2.0 unx    10726 b- defN 23-Nov-08 09:50 hex/genmodel/algos/gam/GamMojoReader.class
+-rw-r--r--  2.0 unx     1717 b- defN 23-Nov-08 09:50 hex/genmodel/algos/gam/NBSplinesTypeI$MSplineBasis.class
+-rw-r--r--  2.0 unx      855 b- defN 23-Nov-08 09:50 hex/genmodel/algos/gam/ISplines$ISplineBasis.class
+-rw-r--r--  2.0 unx     1902 b- defN 23-Nov-08 09:50 hex/genmodel/algos/gam/NBSplinesTypeII$BSplineBasis.class
+-rw-r--r--  2.0 unx     3495 b- defN 23-Nov-08 09:50 hex/genmodel/algos/gam/NBSplinesTypeI.class
+-rw-r--r--  2.0 unx     2061 b- defN 23-Nov-08 09:50 hex/genmodel/algos/gam/GamUtilsThinPlateRegression.class
+-rw-r--r--  2.0 unx    11583 b- defN 23-Nov-08 09:50 hex/genmodel/algos/gam/GamMojoModelBase.class
+-rw-r--r--  2.0 unx     1347 b- defN 23-Nov-08 09:50 hex/genmodel/algos/gam/MSplines.class
+-rw-r--r--  2.0 unx     4489 b- defN 23-Nov-08 09:50 hex/genmodel/algos/gam/GamUtilsISplines.class
+-rw-r--r--  2.0 unx      896 b- defN 23-Nov-08 09:50 hex/genmodel/algos/gam/GamMojoModelBase$1.class
+-rw-r--r--  2.0 unx     2234 b- defN 23-Nov-08 09:50 hex/genmodel/algos/gam/GamMojoMultinomialModel.class
+-rw-r--r--  2.0 unx     1977 b- defN 23-Nov-08 09:50 hex/genmodel/algos/gam/GamRowToRawDataConverter.class
+-rw-r--r--  2.0 unx     2518 b- defN 23-Nov-08 09:50 hex/genmodel/algos/gam/GamUtilsCubicRegression.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/algos/pipeline/
+-rw-r--r--  2.0 unx     1732 b- defN 23-Nov-08 09:50 hex/genmodel/algos/pipeline/MojoPipeline.class
+-rw-r--r--  2.0 unx     6799 b- defN 23-Nov-08 09:50 hex/genmodel/algos/pipeline/MojoPipelineReader.class
+-rw-r--r--  2.0 unx      635 b- defN 23-Nov-08 09:50 hex/genmodel/algos/pipeline/MojoPipeline$PipelineSubModel.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/algos/kmeans/
+-rw-r--r--  2.0 unx     1339 b- defN 23-Nov-08 09:50 hex/genmodel/algos/kmeans/KMeansMojoModel.class
+-rw-r--r--  2.0 unx     2248 b- defN 23-Nov-08 09:50 hex/genmodel/algos/kmeans/KMeansMojoReader.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/algos/gbm/
+-rw-r--r--  2.0 unx     4006 b- defN 23-Nov-08 09:50 hex/genmodel/algos/gbm/GbmMojoModel.class
+-rw-r--r--  2.0 unx     2104 b- defN 23-Nov-08 09:50 hex/genmodel/algos/gbm/GbmMojoReader.class
+-rw-r--r--  2.0 unx      981 b- defN 23-Nov-08 09:50 hex/genmodel/algos/gbm/GbmMojoModel$1.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glrm/
+-rw-r--r--  2.0 unx     1345 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glrm/GlrmRegularizer$3.class
+-rw-r--r--  2.0 unx     4904 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glrm/GlrmMojoReader.class
+-rw-r--r--  2.0 unx     1567 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glrm/GlrmLoss$5.class
+-rw-r--r--  2.0 unx     2161 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glrm/GlrmLoss$8.class
+-rw-r--r--  2.0 unx     1232 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glrm/GlrmRegularizer$2.class
+-rw-r--r--  2.0 unx     1980 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glrm/GlrmRegularizer$8.class
+-rw-r--r--  2.0 unx      875 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glrm/GlrmRegularizer$1.class
+-rw-r--r--  2.0 unx     2578 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glrm/GlrmRegularizer.class
+-rw-r--r--  2.0 unx     1219 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glrm/GlrmInitialization.class
+-rw-r--r--  2.0 unx     1075 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glrm/GlrmLoss$2.class
+-rw-r--r--  2.0 unx     2236 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glrm/GlrmLoss$9.class
+-rw-r--r--  2.0 unx     1512 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glrm/GlrmLoss$6.class
+-rw-r--r--  2.0 unx     1186 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glrm/GlrmLoss$3.class
+-rw-r--r--  2.0 unx     1290 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glrm/GlrmRegularizer$4.class
+-rw-r--r--  2.0 unx     1406 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glrm/GlrmRegularizer$7.class
+-rw-r--r--  2.0 unx     9537 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glrm/GlrmMojoModel.class
+-rw-r--r--  2.0 unx     1280 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glrm/GlrmRegularizer$5.class
+-rw-r--r--  2.0 unx      983 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glrm/GlrmLoss$1.class
+-rw-r--r--  2.0 unx     1510 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glrm/GlrmLoss$7.class
+-rw-r--r--  2.0 unx     1460 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glrm/GlrmRegularizer$6.class
+-rw-r--r--  2.0 unx     3178 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glrm/GlrmLoss.class
+-rw-r--r--  2.0 unx     1499 b- defN 23-Nov-08 09:50 hex/genmodel/algos/glrm/GlrmLoss$4.class
+-rw-r--r--  2.0 unx     1100 b- defN 23-Nov-08 09:50 hex/genmodel/ModelMojoReader$1.class
+-rw-r--r--  2.0 unx      855 b- defN 23-Nov-08 09:50 hex/genmodel/MojoReaderBackendFactory$1.class
+-rw-r--r--  2.0 unx     1934 b- defN 23-Nov-08 09:50 hex/genmodel/MultiModelMojoReader$NestedMojoReaderBackend.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/
+-rw-r--r--  2.0 unx     1045 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/SharedTreeModelAttributes.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/metrics/
+-rw-r--r--  2.0 unx      798 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/metrics/MojoModelMetricsOrdinalGLM.class
+-rw-r--r--  2.0 unx      420 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/metrics/MojoModelMetricsSupervised.class
+-rw-r--r--  2.0 unx      590 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/metrics/MojoModelMetricsRegression.class
+-rw-r--r--  2.0 unx      774 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/metrics/MojoModelMetricsBinomialUplift.class
+-rw-r--r--  2.0 unx      802 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/metrics/MojoModelMetricsBinomialGLM.class
+-rw-r--r--  2.0 unx      449 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/metrics/MojoModelMetricsAnomaly.class
+-rw-r--r--  2.0 unx      630 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/metrics/MojoModelMetrics.class
+-rw-r--r--  2.0 unx      748 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/metrics/MojoModelMetricsOrdinal.class
+-rw-r--r--  2.0 unx      860 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/metrics/MojoModelMetricsBinomial.class
+-rw-r--r--  2.0 unx      860 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/metrics/MojoModelMetricsMultinomial.class
+-rw-r--r--  2.0 unx      810 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/metrics/MojoModelMetricsRegressionGLM.class
+-rw-r--r--  2.0 unx      814 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/metrics/MojoModelMetricsMultinomialGLM.class
+-rw-r--r--  2.0 unx      517 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/metrics/MojoModelMetricsRegressionCoxPH.class
+-rw-r--r--  2.0 unx      993 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/DeepLearningModelAttributes.class
+-rw-r--r--  2.0 unx     5743 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/ModelAttributes.class
+-rw-r--r--  2.0 unx     1267 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/VariableImportances$1.class
+-rw-r--r--  2.0 unx      495 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/SerializedName.class
+-rw-r--r--  2.0 unx     2602 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/VariableImportances.class
+-rw-r--r--  2.0 unx     1676 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/Table$ColumnType.class
+-rw-r--r--  2.0 unx     1211 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/ModelAttributes$1.class
+-rw-r--r--  2.0 unx     3376 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/Table.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/parameters/
+-rw-r--r--  2.0 unx      874 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/parameters/ColumnSpecifier.class
+-rw-r--r--  2.0 unx      249 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/parameters/VariableImportancesHolder.class
+-rw-r--r--  2.0 unx      953 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/parameters/KeyValue.class
+-rw-r--r--  2.0 unx     1892 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/parameters/ModelParameter.class
+-rw-r--r--  2.0 unx     1319 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/parameters/ParameterKey$Type.class
+-rw-r--r--  2.0 unx      880 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/parameters/FeatureContribution.class
+-rw-r--r--  2.0 unx     1176 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/parameters/ParameterKey.class
+-rw-r--r--  2.0 unx     1263 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/parameters/StringPair.class
+-rw-r--r--  2.0 unx     1768 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/ModelJsonReader$1.class
+-rw-r--r--  2.0 unx     2522 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/ModelJsonReader$TypeHint.class
+-rw-r--r--  2.0 unx     1234 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/ModelAttributesGLM.class
+-rw-r--r--  2.0 unx    15710 b- defN 23-Nov-08 09:50 hex/genmodel/attributes/ModelJsonReader.class
+-rw-r--r--  2.0 unx     1541 b- defN 23-Nov-08 09:50 hex/genmodel/CategoricalEncoding$2.class
+-rw-r--r--  2.0 unx     1551 b- defN 23-Nov-08 09:50 hex/genmodel/CategoricalEncoding$4.class
+-rw-r--r--  2.0 unx     1127 b- defN 23-Nov-08 09:50 hex/genmodel/MojoPipelineBuilder$MappingSpec.class
+-rw-r--r--  2.0 unx     5145 b- defN 23-Nov-08 09:50 hex/genmodel/ModelMojoFactory.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 water/
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 water/util/
+-rw-r--r--  2.0 unx     4898 b- defN 23-Nov-08 09:50 water/util/ParseTime.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 water/util/comparison/
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 water/util/comparison/string/
+-rw-r--r--  2.0 unx     1597 b- defN 23-Nov-08 09:50 water/util/comparison/string/JaccardIndexComparator.class
+-rw-r--r--  2.0 unx      865 b- defN 23-Nov-08 09:50 water/util/comparison/string/LongestCommonSubstring$Formula$3.class
+-rw-r--r--  2.0 unx      272 b- defN 23-Nov-08 09:50 water/util/comparison/string/LongestCommonSubstring$1.class
+-rw-r--r--  2.0 unx     2471 b- defN 23-Nov-08 09:50 water/util/comparison/string/QGramComparator$Formula.class
+-rw-r--r--  2.0 unx     1804 b- defN 23-Nov-08 09:50 water/util/comparison/string/SoundexComparator.class
+-rw-r--r--  2.0 unx     1908 b- defN 23-Nov-08 09:50 water/util/comparison/string/StringComparatorFactory.class
+-rw-r--r--  2.0 unx      865 b- defN 23-Nov-08 09:50 water/util/comparison/string/LongestCommonSubstring$Formula$2.class
+-rw-r--r--  2.0 unx     1101 b- defN 23-Nov-08 09:50 water/util/comparison/string/QGramComparator$Formula$3.class
+-rw-r--r--  2.0 unx     2359 b- defN 23-Nov-08 09:50 water/util/comparison/string/LongestCommonSubstring$Formula.class
+-rw-r--r--  2.0 unx     2346 b- defN 23-Nov-08 09:50 water/util/comparison/string/QGramComparator$Tokenizer.class
+-rw-r--r--  2.0 unx      861 b- defN 23-Nov-08 09:50 water/util/comparison/string/LongestCommonSubstring$Formula$1.class
+-rw-r--r--  2.0 unx     2936 b- defN 23-Nov-08 09:50 water/util/comparison/string/QGramComparator.class
+-rw-r--r--  2.0 unx     1416 b- defN 23-Nov-08 09:50 water/util/comparison/string/StringUtils.class
+-rw-r--r--  2.0 unx     2744 b- defN 23-Nov-08 09:50 water/util/comparison/string/LongestCommonSubstring.class
+-rw-r--r--  2.0 unx     1566 b- defN 23-Nov-08 09:50 water/util/comparison/string/QGramComparator$Tokenizer$3.class
+-rw-r--r--  2.0 unx     1540 b- defN 23-Nov-08 09:50 water/util/comparison/string/QGramComparator$Tokenizer$2.class
+-rw-r--r--  2.0 unx      251 b- defN 23-Nov-08 09:50 water/util/comparison/string/QGramComparator$1.class
+-rw-r--r--  2.0 unx      230 b- defN 23-Nov-08 09:50 water/util/comparison/string/StringComparator.class
+-rw-r--r--  2.0 unx     1336 b- defN 23-Nov-08 09:50 water/util/comparison/string/QGramComparator$Tokenizer$1.class
+-rw-r--r--  2.0 unx     1135 b- defN 23-Nov-08 09:50 water/util/comparison/string/QGramComparator$Formula$1.class
+-rw-r--r--  2.0 unx     1637 b- defN 23-Nov-08 09:50 water/util/comparison/string/LevenshteinDistanceComparator.class
+-rw-r--r--  2.0 unx     2090 b- defN 23-Nov-08 09:50 water/util/comparison/string/H2OJaroWinklerComparator.class
+-rw-r--r--  2.0 unx     1090 b- defN 23-Nov-08 09:50 water/util/comparison/string/QGramComparator$Formula$2.class
+-rw-r--r--  2.0 unx      724 b- defN 23-Nov-08 09:50 water/util/comparison/string/ExactComparator.class
+-rw-r--r--  2.0 unx    10148 b- defN 23-Nov-08 09:50 water/util/H2OPredictor.class
+-rw-r--r--  2.0 unx      606 b- defN 23-Nov-08 09:50 water/util/H2OPredictor$1.class
+-rw-r--r--  2.0 unx     2742 b- defN 23-Nov-08 09:50 water/util/JavaVersionUtils.class
+-rw-r--r--  2.0 unx      971 b- defN 23-Nov-08 09:50 water/util/ModelUtils.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:50 water/genmodel/
+-rw-r--r--  2.0 unx      873 b- defN 23-Nov-08 09:50 water/genmodel/AbstractBuildVersion$1.class
+-rw-r--r--  2.0 unx     2965 b- defN 23-Nov-08 09:50 water/genmodel/AbstractBuildVersion.class
+-rw-r--r--  2.0 unx      919 b- defN 23-Nov-08 09:50 water/genmodel/BuildVersion.class
+-rw-r--r--  2.0 unx      921 b- defN 23-Nov-08 09:50 water/genmodel/IGeneratedModel.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-08 09:51 META-INF/services/
+-rw-r--r--  2.0 unx       29 b- defN 23-Nov-08 09:51 META-INF/services/hex.genmodel.tools.MojoPrinter
+392 files, 816755 bytes uncompressed, 400079 bytes compressed:  51.0%
```

#### zipnote «TEMP»/diffoscope_wqp9k9w__/tmpqwsmwgyi_.zip

```diff
@@ -945,14 +945,17 @@
 
 Filename: hex/genmodel/attributes/metrics/MojoModelMetricsSupervised.class
 Comment: 
 
 Filename: hex/genmodel/attributes/metrics/MojoModelMetricsRegression.class
 Comment: 
 
+Filename: hex/genmodel/attributes/metrics/MojoModelMetricsBinomialUplift.class
+Comment: 
+
 Filename: hex/genmodel/attributes/metrics/MojoModelMetricsBinomialGLM.class
 Comment: 
 
 Filename: hex/genmodel/attributes/metrics/MojoModelMetricsAnomaly.class
 Comment: 
 
 Filename: hex/genmodel/attributes/metrics/MojoModelMetrics.class
```

#### hex/genmodel/descriptor/ModelDescriptor.class

##### procyon -ec {}

```diff
@@ -15,14 +15,16 @@
     
     String offsetColumn();
     
     String weightsColumn();
     
     String foldColumn();
     
+    String treatmentColumn();
+    
     ModelCategory getModelCategory();
     
     boolean isSupervised();
     
     int nfeatures();
     
     String[] features();
```

#### hex/genmodel/descriptor/ModelDescriptorBuilder$PojoModelDescriptor.class

##### procyon -ec {}

```diff
@@ -59,14 +59,18 @@
         return null;
     }
     
     public String foldColumn() {
         return null;
     }
     
+    public String treatmentColumn() {
+        return null;
+    }
+    
     public ModelCategory getModelCategory() {
         return this._category;
     }
     
     public boolean isSupervised() {
         return this._supervised;
     }
```

#### hex/genmodel/descriptor/ModelDescriptorBuilder$MojoModelDescriptor.class

##### procyon -ec {}

```diff
@@ -18,14 +18,15 @@
     private final int _nclasses;
     private final boolean _balanceClasses;
     private final double _defaultThreshold;
     private final double[] _priorClassDistrib;
     private final double[] _modelClassDistrib;
     private final String _offsetColumn;
     private final String _weightsColumn;
+    private final String _treatmentColumn;
     private final String[][] _domains;
     private final String[][] _origDomains;
     private final String[] _names;
     private final String[] _origNames;
     private final String _algoName;
     private final String _fullAlgoName;
     
@@ -50,14 +51,20 @@
         if (modelAttributes != null) {
             final ColumnSpecifier weightsColSpec = (ColumnSpecifier)modelAttributes.getParameterValueByName("weights_column");
             this._weightsColumn = ((weightsColSpec != null) ? weightsColSpec.getColumnName() : null);
         }
         else {
             this._weightsColumn = null;
         }
+        if (modelAttributes != null) {
+            this._treatmentColumn = (String)modelAttributes.getParameterValueByName("treatment_column");
+        }
+        else {
+            this._treatmentColumn = null;
+        }
     }
     
     public String[][] scoringDomains() {
         return this._domains;
     }
     
     public String projectVersion() {
@@ -80,14 +87,18 @@
         return this._weightsColumn;
     }
     
     public String foldColumn() {
         return null;
     }
     
+    public String treatmentColumn() {
+        return this._treatmentColumn;
+    }
+    
     public ModelCategory getModelCategory() {
         return this._category;
     }
     
     public boolean isSupervised() {
         return this._supervised;
     }
```

#### hex/genmodel/MojoPipelineWriter$MojoPipelineDescriptor.class

##### procyon -ec {}

```diff
@@ -51,14 +51,18 @@
         return null;
     }
     
     public String foldColumn() {
         return null;
     }
     
+    public String treatmentColumn() {
+        return null;
+    }
+    
     public ModelCategory getModelCategory() {
         return this._finalModel._category;
     }
     
     public boolean isSupervised() {
         return this._finalModel.isSupervised();
     }
```

#### hex/genmodel/attributes/ModelAttributes.class

##### procyon -ec {}

```diff
@@ -1,10 +1,11 @@
 
 package hex.genmodel.attributes;
 
+import hex.genmodel.attributes.metrics.MojoModelMetricsBinomialUplift;
 import hex.genmodel.attributes.metrics.MojoModelMetricsRegressionCoxPH;
 import hex.genmodel.attributes.metrics.MojoModelMetricsOrdinal;
 import hex.genmodel.attributes.metrics.MojoModelMetricsOrdinalGLM;
 import hex.genmodel.algos.glm.GlmOrdinalMojoModel;
 import hex.genmodel.attributes.metrics.MojoModelMetricsAnomaly;
 import hex.genmodel.attributes.metrics.MojoModelMetricsRegression;
 import hex.genmodel.attributes.metrics.MojoModelMetricsRegressionGLM;
@@ -104,14 +105,17 @@
                     return (MojoModelMetrics)new MojoModelMetricsOrdinalGLM();
                 }
                 return (MojoModelMetrics)new MojoModelMetricsOrdinal();
             }
             case 6: {
                 return (MojoModelMetrics)new MojoModelMetricsRegressionCoxPH();
             }
+            case 7: {
+                return (MojoModelMetrics)new MojoModelMetricsBinomialUplift();
+            }
             default: {
                 return new MojoModelMetrics();
             }
         }
     }
     
     public Table getModelSummary() {
```

#### hex/genmodel/attributes/ModelAttributes$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,84 +1,87 @@
-  SHA-256 checksum d4ae475217c13def59bdae1d24b0808df5f349927bb5d08030c29c1ec7aea2cd
+  SHA-256 checksum f23e2c1f5c81ba18d4b3eba01da7b6a60784bca49013491c934ccece05648015
   Compiled from "ModelAttributes.java"
 class hex.genmodel.attributes.ModelAttributes$1
   minor version: 0
   major version: 51
   flags: (0x1020) ACC_SUPER, ACC_SYNTHETIC
-  this_class: #16                         // hex/genmodel/attributes/ModelAttributes$1
-  super_class: #17                        // java/lang/Object
+  this_class: #17                         // hex/genmodel/attributes/ModelAttributes$1
+  super_class: #18                        // java/lang/Object
   interfaces: 0, fields: 1, methods: 1, attributes: 3
 Constant pool:
-   #1 = Methodref          #31.#32        // hex/ModelCategory.values:()[Lhex/ModelCategory;
-   #2 = Fieldref           #16.#33        // hex/genmodel/attributes/ModelAttributes$1.$SwitchMap$hex$ModelCategory:[I
-   #3 = Fieldref           #31.#34        // hex/ModelCategory.Binomial:Lhex/ModelCategory;
-   #4 = Methodref          #31.#35        // hex/ModelCategory.ordinal:()I
-   #5 = Class              #36            // java/lang/NoSuchFieldError
-   #6 = Fieldref           #31.#37        // hex/ModelCategory.Multinomial:Lhex/ModelCategory;
-   #7 = Fieldref           #31.#38        // hex/ModelCategory.Regression:Lhex/ModelCategory;
-   #8 = Fieldref           #31.#39        // hex/ModelCategory.AnomalyDetection:Lhex/ModelCategory;
-   #9 = Fieldref           #31.#40        // hex/ModelCategory.Ordinal:Lhex/ModelCategory;
-  #10 = Fieldref           #31.#41        // hex/ModelCategory.CoxPH:Lhex/ModelCategory;
-  #11 = Fieldref           #31.#42        // hex/ModelCategory.Unknown:Lhex/ModelCategory;
-  #12 = Fieldref           #31.#43        // hex/ModelCategory.Clustering:Lhex/ModelCategory;
-  #13 = Fieldref           #31.#44        // hex/ModelCategory.AutoEncoder:Lhex/ModelCategory;
-  #14 = Fieldref           #31.#45        // hex/ModelCategory.DimReduction:Lhex/ModelCategory;
-  #15 = Fieldref           #31.#46        // hex/ModelCategory.WordEmbedding:Lhex/ModelCategory;
-  #16 = Class              #47            // hex/genmodel/attributes/ModelAttributes$1
-  #17 = Class              #49            // java/lang/Object
-  #18 = Utf8               $SwitchMap$hex$ModelCategory
-  #19 = Utf8               [I
-  #20 = Utf8               <clinit>
-  #21 = Utf8               ()V
-  #22 = Utf8               Code
-  #23 = Utf8               LineNumberTable
-  #24 = Utf8               LocalVariableTable
-  #25 = Utf8               StackMapTable
-  #26 = Class              #36            // java/lang/NoSuchFieldError
-  #27 = Utf8               SourceFile
-  #28 = Utf8               ModelAttributes.java
-  #29 = Utf8               EnclosingMethod
-  #30 = Class              #50            // hex/genmodel/attributes/ModelAttributes
-  #31 = Class              #51            // hex/ModelCategory
-  #32 = NameAndType        #52:#53        // values:()[Lhex/ModelCategory;
-  #33 = NameAndType        #18:#19        // $SwitchMap$hex$ModelCategory:[I
-  #34 = NameAndType        #54:#55        // Binomial:Lhex/ModelCategory;
-  #35 = NameAndType        #56:#57        // ordinal:()I
-  #36 = Utf8               java/lang/NoSuchFieldError
-  #37 = NameAndType        #58:#55        // Multinomial:Lhex/ModelCategory;
-  #38 = NameAndType        #59:#55        // Regression:Lhex/ModelCategory;
-  #39 = NameAndType        #60:#55        // AnomalyDetection:Lhex/ModelCategory;
-  #40 = NameAndType        #61:#55        // Ordinal:Lhex/ModelCategory;
-  #41 = NameAndType        #62:#55        // CoxPH:Lhex/ModelCategory;
-  #42 = NameAndType        #63:#55        // Unknown:Lhex/ModelCategory;
-  #43 = NameAndType        #64:#55        // Clustering:Lhex/ModelCategory;
-  #44 = NameAndType        #65:#55        // AutoEncoder:Lhex/ModelCategory;
-  #45 = NameAndType        #66:#55        // DimReduction:Lhex/ModelCategory;
-  #46 = NameAndType        #67:#55        // WordEmbedding:Lhex/ModelCategory;
-  #47 = Utf8               hex/genmodel/attributes/ModelAttributes$1
-  #48 = Utf8               InnerClasses
-  #49 = Utf8               java/lang/Object
-  #50 = Utf8               hex/genmodel/attributes/ModelAttributes
-  #51 = Utf8               hex/ModelCategory
-  #52 = Utf8               values
-  #53 = Utf8               ()[Lhex/ModelCategory;
-  #54 = Utf8               Binomial
-  #55 = Utf8               Lhex/ModelCategory;
-  #56 = Utf8               ordinal
-  #57 = Utf8               ()I
-  #58 = Utf8               Multinomial
-  #59 = Utf8               Regression
-  #60 = Utf8               AnomalyDetection
-  #61 = Utf8               Ordinal
-  #62 = Utf8               CoxPH
-  #63 = Utf8               Unknown
-  #64 = Utf8               Clustering
-  #65 = Utf8               AutoEncoder
-  #66 = Utf8               DimReduction
-  #67 = Utf8               WordEmbedding
+   #1 = Methodref          #32.#33        // hex/ModelCategory.values:()[Lhex/ModelCategory;
+   #2 = Fieldref           #17.#34        // hex/genmodel/attributes/ModelAttributes$1.$SwitchMap$hex$ModelCategory:[I
+   #3 = Fieldref           #32.#35        // hex/ModelCategory.Binomial:Lhex/ModelCategory;
+   #4 = Methodref          #32.#36        // hex/ModelCategory.ordinal:()I
+   #5 = Class              #37            // java/lang/NoSuchFieldError
+   #6 = Fieldref           #32.#38        // hex/ModelCategory.Multinomial:Lhex/ModelCategory;
+   #7 = Fieldref           #32.#39        // hex/ModelCategory.Regression:Lhex/ModelCategory;
+   #8 = Fieldref           #32.#40        // hex/ModelCategory.AnomalyDetection:Lhex/ModelCategory;
+   #9 = Fieldref           #32.#41        // hex/ModelCategory.Ordinal:Lhex/ModelCategory;
+  #10 = Fieldref           #32.#42        // hex/ModelCategory.CoxPH:Lhex/ModelCategory;
+  #11 = Fieldref           #32.#43        // hex/ModelCategory.BinomialUplift:Lhex/ModelCategory;
+  #12 = Fieldref           #32.#44        // hex/ModelCategory.Unknown:Lhex/ModelCategory;
+  #13 = Fieldref           #32.#45        // hex/ModelCategory.Clustering:Lhex/ModelCategory;
+  #14 = Fieldref           #32.#46        // hex/ModelCategory.AutoEncoder:Lhex/ModelCategory;
+  #15 = Fieldref           #32.#47        // hex/ModelCategory.DimReduction:Lhex/ModelCategory;
+  #16 = Fieldref           #32.#48        // hex/ModelCategory.WordEmbedding:Lhex/ModelCategory;
+  #17 = Class              #49            // hex/genmodel/attributes/ModelAttributes$1
+  #18 = Class              #51            // java/lang/Object
+  #19 = Utf8               $SwitchMap$hex$ModelCategory
+  #20 = Utf8               [I
+  #21 = Utf8               <clinit>
+  #22 = Utf8               ()V
+  #23 = Utf8               Code
+  #24 = Utf8               LineNumberTable
+  #25 = Utf8               LocalVariableTable
+  #26 = Utf8               StackMapTable
+  #27 = Class              #37            // java/lang/NoSuchFieldError
+  #28 = Utf8               SourceFile
+  #29 = Utf8               ModelAttributes.java
+  #30 = Utf8               EnclosingMethod
+  #31 = Class              #52            // hex/genmodel/attributes/ModelAttributes
+  #32 = Class              #53            // hex/ModelCategory
+  #33 = NameAndType        #54:#55        // values:()[Lhex/ModelCategory;
+  #34 = NameAndType        #19:#20        // $SwitchMap$hex$ModelCategory:[I
+  #35 = NameAndType        #56:#57        // Binomial:Lhex/ModelCategory;
+  #36 = NameAndType        #58:#59        // ordinal:()I
+  #37 = Utf8               java/lang/NoSuchFieldError
+  #38 = NameAndType        #60:#57        // Multinomial:Lhex/ModelCategory;
+  #39 = NameAndType        #61:#57        // Regression:Lhex/ModelCategory;
+  #40 = NameAndType        #62:#57        // AnomalyDetection:Lhex/ModelCategory;
+  #41 = NameAndType        #63:#57        // Ordinal:Lhex/ModelCategory;
+  #42 = NameAndType        #64:#57        // CoxPH:Lhex/ModelCategory;
+  #43 = NameAndType        #65:#57        // BinomialUplift:Lhex/ModelCategory;
+  #44 = NameAndType        #66:#57        // Unknown:Lhex/ModelCategory;
+  #45 = NameAndType        #67:#57        // Clustering:Lhex/ModelCategory;
+  #46 = NameAndType        #68:#57        // AutoEncoder:Lhex/ModelCategory;
+  #47 = NameAndType        #69:#57        // DimReduction:Lhex/ModelCategory;
+  #48 = NameAndType        #70:#57        // WordEmbedding:Lhex/ModelCategory;
+  #49 = Utf8               hex/genmodel/attributes/ModelAttributes$1
+  #50 = Utf8               InnerClasses
+  #51 = Utf8               java/lang/Object
+  #52 = Utf8               hex/genmodel/attributes/ModelAttributes
+  #53 = Utf8               hex/ModelCategory
+  #54 = Utf8               values
+  #55 = Utf8               ()[Lhex/ModelCategory;
+  #56 = Utf8               Binomial
+  #57 = Utf8               Lhex/ModelCategory;
+  #58 = Utf8               ordinal
+  #59 = Utf8               ()I
+  #60 = Utf8               Multinomial
+  #61 = Utf8               Regression
+  #62 = Utf8               AnomalyDetection
+  #63 = Utf8               Ordinal
+  #64 = Utf8               CoxPH
+  #65 = Utf8               BinomialUplift
+  #66 = Utf8               Unknown
+  #67 = Utf8               Clustering
+  #68 = Utf8               AutoEncoder
+  #69 = Utf8               DimReduction
+  #70 = Utf8               WordEmbedding
 {
   static final int[] $SwitchMap$hex$ModelCategory;
     descriptor: [I
     flags: (0x1018) ACC_STATIC, ACC_FINAL, ACC_SYNTHETIC
 
   static {};
     descriptor: ()V
@@ -128,67 +131,75 @@
         87: getstatic     #10                 // Field hex/ModelCategory.CoxPH:Lhex/ModelCategory;
         90: invokevirtual #4                  // Method hex/ModelCategory.ordinal:()I
         93: bipush        6
         95: iastore
         96: goto          100
         99: astore_0
        100: getstatic     #2                  // Field $SwitchMap$hex$ModelCategory:[I
-       103: getstatic     #11                 // Field hex/ModelCategory.Unknown:Lhex/ModelCategory;
+       103: getstatic     #11                 // Field hex/ModelCategory.BinomialUplift:Lhex/ModelCategory;
        106: invokevirtual #4                  // Method hex/ModelCategory.ordinal:()I
        109: bipush        7
        111: iastore
        112: goto          116
        115: astore_0
        116: getstatic     #2                  // Field $SwitchMap$hex$ModelCategory:[I
-       119: getstatic     #12                 // Field hex/ModelCategory.Clustering:Lhex/ModelCategory;
+       119: getstatic     #12                 // Field hex/ModelCategory.Unknown:Lhex/ModelCategory;
        122: invokevirtual #4                  // Method hex/ModelCategory.ordinal:()I
        125: bipush        8
        127: iastore
        128: goto          132
        131: astore_0
        132: getstatic     #2                  // Field $SwitchMap$hex$ModelCategory:[I
-       135: getstatic     #13                 // Field hex/ModelCategory.AutoEncoder:Lhex/ModelCategory;
+       135: getstatic     #13                 // Field hex/ModelCategory.Clustering:Lhex/ModelCategory;
        138: invokevirtual #4                  // Method hex/ModelCategory.ordinal:()I
        141: bipush        9
        143: iastore
        144: goto          148
        147: astore_0
        148: getstatic     #2                  // Field $SwitchMap$hex$ModelCategory:[I
-       151: getstatic     #14                 // Field hex/ModelCategory.DimReduction:Lhex/ModelCategory;
+       151: getstatic     #14                 // Field hex/ModelCategory.AutoEncoder:Lhex/ModelCategory;
        154: invokevirtual #4                  // Method hex/ModelCategory.ordinal:()I
        157: bipush        10
        159: iastore
        160: goto          164
        163: astore_0
        164: getstatic     #2                  // Field $SwitchMap$hex$ModelCategory:[I
-       167: getstatic     #15                 // Field hex/ModelCategory.WordEmbedding:Lhex/ModelCategory;
+       167: getstatic     #15                 // Field hex/ModelCategory.DimReduction:Lhex/ModelCategory;
        170: invokevirtual #4                  // Method hex/ModelCategory.ordinal:()I
        173: bipush        11
        175: iastore
        176: goto          180
        179: astore_0
-       180: return
+       180: getstatic     #2                  // Field $SwitchMap$hex$ModelCategory:[I
+       183: getstatic     #16                 // Field hex/ModelCategory.WordEmbedding:Lhex/ModelCategory;
+       186: invokevirtual #4                  // Method hex/ModelCategory.ordinal:()I
+       189: bipush        12
+       191: iastore
+       192: goto          196
+       195: astore_0
+       196: return
       Exception table:
          from    to  target type
              9    20    23   Class java/lang/NoSuchFieldError
             24    35    38   Class java/lang/NoSuchFieldError
             39    50    53   Class java/lang/NoSuchFieldError
             54    65    68   Class java/lang/NoSuchFieldError
             69    80    83   Class java/lang/NoSuchFieldError
             84    96    99   Class java/lang/NoSuchFieldError
            100   112   115   Class java/lang/NoSuchFieldError
            116   128   131   Class java/lang/NoSuchFieldError
            132   144   147   Class java/lang/NoSuchFieldError
            148   160   163   Class java/lang/NoSuchFieldError
            164   176   179   Class java/lang/NoSuchFieldError
+           180   192   195   Class java/lang/NoSuchFieldError
       LineNumberTable:
         line 73: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
-      StackMapTable: number_of_entries = 22
+      StackMapTable: number_of_entries = 24
         frame_type = 87 /* same_locals_1_stack_item */
           stack = [ class java/lang/NoSuchFieldError ]
         frame_type = 0 /* same */
         frame_type = 77 /* same_locals_1_stack_item */
           stack = [ class java/lang/NoSuchFieldError ]
         frame_type = 0 /* same */
         frame_type = 77 /* same_locals_1_stack_item */
@@ -214,12 +225,15 @@
         frame_type = 0 /* same */
         frame_type = 78 /* same_locals_1_stack_item */
           stack = [ class java/lang/NoSuchFieldError ]
         frame_type = 0 /* same */
         frame_type = 78 /* same_locals_1_stack_item */
           stack = [ class java/lang/NoSuchFieldError ]
         frame_type = 0 /* same */
+        frame_type = 78 /* same_locals_1_stack_item */
+          stack = [ class java/lang/NoSuchFieldError ]
+        frame_type = 0 /* same */
 }
 SourceFile: "ModelAttributes.java"
-EnclosingMethod: #30.#0                 // hex.genmodel.attributes.ModelAttributes
+EnclosingMethod: #31.#0                 // hex.genmodel.attributes.ModelAttributes
 InnerClasses:
-  static #16;                             // class hex/genmodel/attributes/ModelAttributes$1
+  static #17;                             // class hex/genmodel/attributes/ModelAttributes$1
```

#### water/genmodel/BuildVersion.class

##### procyon -ec {}

```diff
@@ -4,26 +4,26 @@
 public class BuildVersion extends AbstractBuildVersion
 {
     public String branchName() {
         return "rel-3.44.0";
     }
     
     public String lastCommitHash() {
-        return "0a9196d7fe134320fe1c956fe0d7c80fbfa30936";
+        return "55978fe6a06c55ce67cbfa653a783e3787a2bb5e";
     }
     
     public String describe() {
-        return "jenkins-master-6342-18-g0a9196d";
+        return "jenkins-3.44.0.1-22-g55978fe";
     }
     
     public String projectVersion() {
-        return "3.44.0.1";
+        return "3.44.0.2";
     }
     
     public String compiledOn() {
-        return "2023-10-16 10:26:34";
+        return "2023-11-08 09:50:42";
     }
     
     public String compiledBy() {
         return "jenkins";
     }
 }
```

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/classpath.txt` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/classpath.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 sklearn2pmml-1.0-SNAPSHOT.jar
 gson-2.10.1.jar
 guava-32.1.1-jre.jar
-h2o-genmodel-3.44.0.1.jar
-h2o-logger-3.44.0.1.jar
+h2o-genmodel-3.44.0.2.jar
+h2o-logger-3.44.0.2.jar
 h2o-tree-api-0.3.17.jar
 istack-commons-runtime-4.0.1.jar
 jackson-annotations-2.13.3.jar
 jakarta.activation-2.0.1.jar
 jakarta.xml.bind-api-3.0.1.jar
 jaxb-core-3.0.2.jar
 jaxb-runtime-3.0.2.jar
 jcommander-1.72.jar
-pickle-1.4.jar
+pickle-1.5.jar
 pmml-converter-1.5.5.jar
 pmml-h2o-1.2.9.jar
 pmml-lightgbm-1.4.6.jar
 pmml-model-1.6.4.jar
 pmml-model-metro-1.6.4.jar
-pmml-python-1.1.17.jar
-pmml-sklearn-1.7.41.jar
-pmml-sklearn-extension-1.7.41.jar
-pmml-sklearn-h2o-1.7.41.jar
-pmml-sklearn-lightgbm-1.7.41.jar
-pmml-sklearn-statsmodels-1.7.41.jar
-pmml-sklearn-xgboost-1.7.41.jar
+pmml-python-1.1.18.jar
+pmml-sklearn-1.7.42.jar
+pmml-sklearn-extension-1.7.42.jar
+pmml-sklearn-h2o-1.7.42.jar
+pmml-sklearn-lightgbm-1.7.42.jar
+pmml-sklearn-statsmodels-1.7.42.jar
+pmml-sklearn-xgboost-1.7.42.jar
 pmml-statsmodels-1.0.5.jar
 pmml-xgboost-1.7.4.jar
 serpent-1.40.jar
 slf4j-api-1.7.36.jar
 slf4j-jdk14-1.7.36.jar
 ubjson-0.1.8.jar
 ubjson-gson-0.1.8.jar
```

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.41.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.42.jar`

 * *Files 13% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 8467 bytes, number of entries: 15
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Oct-23 22:44 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 xgboost/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 xgboost/sklearn/
--rw-rw-r--  2.0 unx      364 b- defN 23-Oct-23 22:44 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx      168 b- defN 23-Oct-23 22:44 xgboost/sklearn/HasBooster.class
--rw-rw-r--  2.0 unx     2440 b- defN 23-Oct-23 22:44 xgboost/sklearn/XGBClassifier.class
--rw-rw-r--  2.0 unx     2210 b- defN 23-Oct-23 22:44 xgboost/sklearn/Booster.class
--rw-rw-r--  2.0 unx     3023 b- defN 23-Oct-23 22:44 xgboost/sklearn/XGBRegressor.class
--rw-rw-r--  2.0 unx     4855 b- defN 23-Oct-23 22:44 xgboost/sklearn/BoosterUtil.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Oct-23 22:44 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Oct-23 22:44 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Oct-23 22:44 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/
--rw-rw-r--  2.0 unx     1453 b- defN 23-Oct-23 22:44 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml
--rw-rw-r--  2.0 unx      116 b- defN 23-Oct-23 22:44 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.properties
-15 files, 14759 bytes uncompressed, 6411 bytes compressed:  56.6%
+Zip file size: 8465 bytes, number of entries: 15
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Dec-04 22:17 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 xgboost/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 xgboost/sklearn/
+-rw-rw-r--  2.0 unx      364 b- defN 23-Dec-04 22:17 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx      168 b- defN 23-Dec-04 22:17 xgboost/sklearn/HasBooster.class
+-rw-rw-r--  2.0 unx     2440 b- defN 23-Dec-04 22:17 xgboost/sklearn/XGBClassifier.class
+-rw-rw-r--  2.0 unx     2210 b- defN 23-Dec-04 22:17 xgboost/sklearn/Booster.class
+-rw-rw-r--  2.0 unx     3023 b- defN 23-Dec-04 22:17 xgboost/sklearn/XGBRegressor.class
+-rw-rw-r--  2.0 unx     4855 b- defN 23-Dec-04 22:17 xgboost/sklearn/BoosterUtil.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Dec-04 22:17 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Dec-04 22:17 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Dec-04 22:17 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/
+-rw-rw-r--  2.0 unx     1453 b- defN 23-Dec-04 22:16 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml
+-rw-rw-r--  2.0 unx      115 b- defN 23-Dec-04 22:17 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.properties
+15 files, 14758 bytes uncompressed, 6409 bytes compressed:  56.6%
```

#### META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.41</version>
+    <version>1.7.42</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-xgboost</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn XGBoost converter</name>
   <description>JPMML Scikit-Learn XGBoost to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Mon Oct 23 22:44:50 EEST 2023
-version=1.7.41
+#Mon Dec 04 22:17:24 EET 2023
+version=1.7.42
 groupId=org.jpmml
 artifactId=pmml-sklearn-xgboost
```

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar`

 * *Files 16% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 4885 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-23 22:52 META-INF/
--rw-r--r--  2.0 unx      158 b- defN 23-Oct-23 22:52 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:52 com/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:52 com/sklearn2pmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-23 22:52 META-INF/maven/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-23 22:52 META-INF/maven/com.sklearn2pmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-23 22:52 META-INF/maven/com.sklearn2pmml/sklearn2pmml/
--rw-rw-r--  2.0 unx     3376 b- defN 23-Oct-23 22:52 com/sklearn2pmml/Main.class
--rw-rw-r--  2.0 unx     8216 b- defN 23-Oct-23 22:52 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.xml
--rw-rw-r--  2.0 unx       70 b- defN 23-Oct-23 22:52 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.properties
-10 files, 11820 bytes uncompressed, 3543 bytes compressed:  70.0%
+Zip file size: 4886 bytes, number of entries: 10
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-04 22:28 META-INF/
+-rw-r--r--  2.0 unx      158 b- defN 23-Dec-04 22:28 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:28 com/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:28 com/sklearn2pmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-04 22:28 META-INF/maven/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-04 22:28 META-INF/maven/com.sklearn2pmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-04 22:28 META-INF/maven/com.sklearn2pmml/sklearn2pmml/
+-rw-rw-r--  2.0 unx     3376 b- defN 23-Dec-04 22:28 com/sklearn2pmml/Main.class
+-rw-rw-r--  2.0 unx     8216 b- defN 23-Dec-04 22:27 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.xml
+-rw-rw-r--  2.0 unx       70 b- defN 23-Dec-04 22:28 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.properties
+10 files, 11820 bytes uncompressed, 3544 bytes compressed:  70.0%
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,6 @@
 Manifest-Version: 1.0
 Implementation-Title: SkLearn2PMML package
-Implementation-Version: 0.99.1
+Implementation-Version: 0.99.3
 Build-Jdk-Spec: 1.8
 Created-By: Maven JAR Plugin 3.3.0
```

#### META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.xml

##### META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.xml

```diff
@@ -24,15 +24,15 @@
     <tag>HEAD</tag>
   </scm>
   <issueManagement>
     <system>GitHub</system>
     <url>https://github.com/jpmml/sklearn2pmml/issues</url>
   </issueManagement>
   <properties>
-    <jpmml-sklearn.version>1.7.41</jpmml-sklearn.version>
+    <jpmml-sklearn.version>1.7.42</jpmml-sklearn.version>
   </properties>
   <dependencies>
     <dependency>
       <groupId>org.jpmml</groupId>
       <artifactId>pmml-sklearn</artifactId>
       <version>${jpmml-sklearn.version}</version>
       <exclusions>
```

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/pmml-python-1.1.17.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/pmml-python-1.1.18.jar`

 * *Files 18% similar despite different names*

#### zipinfo {}

```diff
@@ -1,184 +1,184 @@
-Zip file size: 209112 bytes, number of entries: 182
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 10:47 META-INF/
--rw-r--r--  2.0 unx      158 b- defN 23-Jul-21 10:47 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-21 10:47 patsy/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-21 10:47 functools/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-21 10:47 types/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-21 10:47 treelib/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-21 10:47 pandas/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-21 10:47 pandas/core/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-21 10:47 dill/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-21 10:47 numpy/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-21 10:47 numpy/random/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-21 10:47 numpy/core/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-21 10:47 collections/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-21 10:47 org/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-21 10:47 org/jpmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-21 10:47 org/jpmml/python/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-21 10:47 joblib/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-21 10:47 scipy/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-21 10:47 scipy/stats/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-21 10:47 scipy/interpolate/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-21 10:47 scipy/sparse/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-21 10:47 builtins/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 10:47 META-INF/maven/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 10:47 META-INF/maven/org.jpmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 10:47 META-INF/maven/org.jpmml/pmml-python/
--rw-rw-r--  2.0 unx     2108 b- defN 23-Jul-21 10:47 patsy/PatsyOperation.class
--rw-rw-r--  2.0 unx     2272 b- defN 23-Jul-21 10:47 patsy/PatsyOperator.class
--rw-rw-r--  2.0 unx     3106 b- defN 23-Jul-21 10:47 patsy/PatsyToken.class
--rw-rw-r--  2.0 unx      933 b- defN 23-Jul-21 10:47 patsy/PatsyFactor.class
--rw-rw-r--  2.0 unx      747 b- defN 23-Jul-21 10:47 patsy/PatsyTerm.class
--rw-rw-r--  2.0 unx     8491 b- defN 23-Jul-21 10:47 patsy/FormulaParser.class
--rw-rw-r--  2.0 unx     3432 b- defN 23-Jul-21 10:47 META-INF/python2pmml.properties
--rw-rw-r--  2.0 unx     3301 b- defN 23-Jul-21 10:47 functools/Partial.class
--rw-rw-r--  2.0 unx     1431 b- defN 23-Jul-21 10:47 types/MethodTypeConstructor.class
--rw-rw-r--  2.0 unx      495 b- defN 23-Jul-21 10:47 types/MethodType.class
--rw-rw-r--  2.0 unx     1046 b- defN 23-Jul-21 10:47 types/FunctionType.class
--rw-rw-r--  2.0 unx     2675 b- defN 23-Jul-21 10:47 treelib/Node.class
--rw-rw-r--  2.0 unx     2537 b- defN 23-Jul-21 10:47 treelib/Tree.class
--rw-rw-r--  2.0 unx     1800 b- defN 23-Jul-21 10:47 pandas/NDArrayBackedConstructor.class
--rw-rw-r--  2.0 unx     2430 b- defN 23-Jul-21 10:47 pandas/NDArrayBacked.class
--rw-rw-r--  2.0 unx     1117 b- defN 23-Jul-21 10:47 pandas/core/Index$NDArrayData.class
--rw-rw-r--  2.0 unx     3088 b- defN 23-Jul-21 10:47 pandas/core/Index.class
--rw-rw-r--  2.0 unx     4337 b- defN 23-Jul-21 10:47 pandas/core/BlockManager.class
--rw-rw-r--  2.0 unx     1602 b- defN 23-Jul-21 10:47 pandas/core/SingleBlockManager.class
--rw-rw-r--  2.0 unx      724 b- defN 23-Jul-21 10:47 pandas/core/DataFrame.class
--rw-rw-r--  2.0 unx     2419 b- defN 23-Jul-21 10:47 pandas/core/MaskedArray.class
--rw-rw-r--  2.0 unx      565 b- defN 23-Jul-21 10:47 pandas/core/StringDtype.class
--rw-rw-r--  2.0 unx     3212 b- defN 23-Jul-21 10:47 pandas/core/SeriesUtil.class
--rw-rw-r--  2.0 unx     2092 b- defN 23-Jul-21 10:47 pandas/core/Series.class
--rw-rw-r--  2.0 unx     1382 b- defN 23-Jul-21 10:47 pandas/core/Index$RangeData.class
--rw-rw-r--  2.0 unx     1397 b- defN 23-Jul-21 10:47 pandas/core/CategoricalDtype.class
--rw-rw-r--  2.0 unx      385 b- defN 23-Jul-21 10:47 pandas/core/StringArray.class
--rw-rw-r--  2.0 unx      569 b- defN 23-Jul-21 10:47 pandas/core/IntegerDtype.class
--rw-rw-r--  2.0 unx      703 b- defN 23-Jul-21 10:47 pandas/core/Index$Data.class
--rw-rw-r--  2.0 unx      569 b- defN 23-Jul-21 10:47 pandas/core/BooleanDtype.class
--rw-rw-r--  2.0 unx      713 b- defN 23-Jul-21 10:47 pandas/core/Categorical.class
--rw-rw-r--  2.0 unx      994 b- defN 23-Jul-21 10:47 pandas/core/SeriesUtil$1.class
--rw-rw-r--  2.0 unx     1122 b- defN 23-Jul-21 10:47 pandas/core/MaskedArray$1.class
--rw-rw-r--  2.0 unx      453 b- defN 23-Jul-21 10:47 pandas/core/ExtensionDtype.class
--rw-rw-r--  2.0 unx     1390 b- defN 23-Jul-21 10:47 pandas/core/Block.class
--rw-rw-r--  2.0 unx     3066 b- defN 23-Jul-21 10:47 dill/CreateCodeConstructor.class
--rw-rw-r--  2.0 unx     1021 b- defN 23-Jul-21 10:47 dill/CreateTypeConstructor.class
--rw-rw-r--  2.0 unx     2269 b- defN 23-Jul-21 10:47 dill/LoadTypeConstructor.class
--rw-rw-r--  2.0 unx     1530 b- defN 23-Jul-21 10:47 dill/CreateArrayConstructor.class
--rw-rw-r--  2.0 unx     1260 b- defN 23-Jul-21 10:47 dill/CreateFunctionConstructor.class
--rw-rw-r--  2.0 unx     1172 b- defN 23-Jul-21 10:47 numpy/DTypeUtil.class
--rw-rw-r--  2.0 unx     1404 b- defN 23-Jul-21 10:47 numpy/random/BitGeneratorUtil.class
--rw-rw-r--  2.0 unx     1064 b- defN 23-Jul-21 10:47 numpy/random/Generator.class
--rw-rw-r--  2.0 unx      889 b- defN 23-Jul-21 10:47 numpy/random/BitGenerator.class
--rw-rw-r--  2.0 unx      953 b- defN 23-Jul-21 10:47 numpy/random/RandomState.class
--rw-rw-r--  2.0 unx     1077 b- defN 23-Jul-21 10:47 numpy/random/LegacyRandomState.class
--rw-rw-r--  2.0 unx     4593 b- defN 23-Jul-21 10:47 numpy/DType.class
--rw-rw-r--  2.0 unx     2147 b- defN 23-Jul-21 10:47 numpy/core/TypeDescriptor$Kind.class
--rw-rw-r--  2.0 unx     2138 b- defN 23-Jul-21 10:47 numpy/core/MaskedArray.class
--rw-rw-r--  2.0 unx     1136 b- defN 23-Jul-21 10:47 numpy/core/UFunc.class
--rw-rw-r--  2.0 unx    12387 b- defN 23-Jul-21 10:47 numpy/core/NDArrayUtil.class
--rw-rw-r--  2.0 unx      641 b- defN 23-Jul-21 10:47 numpy/core/Function.class
--rw-rw-r--  2.0 unx     2386 b- defN 23-Jul-21 10:47 numpy/core/FromBufferConstructor.class
--rw-rw-r--  2.0 unx     1065 b- defN 23-Jul-21 10:47 numpy/core/TypeDescriptor$1.class
--rw-rw-r--  2.0 unx     4249 b- defN 23-Jul-21 10:47 numpy/core/NDArray.class
--rw-rw-r--  2.0 unx     5262 b- defN 23-Jul-21 10:47 numpy/core/TypeDescriptor.class
--rw-rw-r--  2.0 unx     3674 b- defN 23-Jul-21 10:47 numpy/core/Scalar.class
--rw-rw-r--  2.0 unx      586 b- defN 23-Jul-21 10:47 numpy/core/ScalarUtil.class
--rw-rw-r--  2.0 unx      109 b- defN 23-Jul-21 10:47 collections/Callable.class
--rw-rw-r--  2.0 unx      895 b- defN 23-Jul-21 10:47 collections/DefaultDict.class
--rw-rw-r--  2.0 unx     1467 b- defN 23-Jul-21 10:47 org/jpmml/python/PythonObject$5.class
--rw-rw-r--  2.0 unx     1256 b- defN 23-Jul-21 10:47 org/jpmml/python/Token.class
--rw-rw-r--  2.0 unx     2927 b- defN 23-Jul-21 10:47 org/jpmml/python/TokenMgrException.class
--rw-rw-r--  2.0 unx     2230 b- defN 23-Jul-21 10:47 org/jpmml/python/TupleUtil.class
--rw-rw-r--  2.0 unx     2779 b- defN 23-Jul-21 10:47 org/jpmml/python/PythonParserConstants.class
--rw-rw-r--  2.0 unx      472 b- defN 23-Jul-21 10:47 org/jpmml/python/Storage.class
--rw-rw-r--  2.0 unx     1689 b- defN 23-Jul-21 10:47 org/jpmml/python/CustomUnpickler.class
--rw-rw-r--  2.0 unx      497 b- defN 23-Jul-21 10:47 org/jpmml/python/FunctionDefParser$JJCalls.class
--rw-rw-r--  2.0 unx      914 b- defN 23-Jul-21 10:47 org/jpmml/python/CompressedInputStreamStorage$Type$2.class
--rw-rw-r--  2.0 unx     1381 b- defN 23-Jul-21 10:47 org/jpmml/python/CompressedInputStreamStorage$1.class
--rw-rw-r--  2.0 unx      242 b- defN 23-Jul-21 10:47 org/jpmml/python/ExpressionTranslator$1.class
--rw-rw-r--  2.0 unx     4157 b- defN 23-Jul-21 10:47 org/jpmml/python/ParseException.class
--rw-rw-r--  2.0 unx      282 b- defN 23-Jul-21 10:47 org/jpmml/python/HasArray.class
--rw-rw-r--  2.0 unx     3481 b- defN 23-Jul-21 10:47 org/jpmml/python/PythonParserUtil.class
--rw-rw-r--  2.0 unx     2631 b- defN 23-Jul-21 10:47 org/jpmml/python/FunctionDefScope.class
--rw-rw-r--  2.0 unx      784 b- defN 23-Jul-21 10:47 org/jpmml/python/ExpressionTranslator$LookaheadSuccess.class
--rw-rw-r--  2.0 unx     2861 b- defN 23-Jul-21 10:47 org/jpmml/python/CompressedInputStreamStorage.class
--rw-rw-r--  2.0 unx      777 b- defN 23-Jul-21 10:47 org/jpmml/python/PredicateTranslator$LookaheadSuccess.class
--rw-rw-r--  2.0 unx     1016 b- defN 23-Jul-21 10:47 org/jpmml/python/CastUtil.class
--rw-rw-r--  2.0 unx      164 b- defN 23-Jul-21 10:47 org/jpmml/python/TypeInfo.class
--rw-rw-r--  2.0 unx     6636 b- defN 23-Jul-21 10:47 org/jpmml/python/ClassDictUtil.class
--rw-rw-r--  2.0 unx    39867 b- defN 23-Jul-21 10:47 org/jpmml/python/ExpressionTranslator.class
--rw-rw-r--  2.0 unx     1294 b- defN 23-Jul-21 10:47 org/jpmml/python/StreamProvider.class
--rw-rw-r--  2.0 unx     1340 b- defN 23-Jul-21 10:47 org/jpmml/python/PickleUtil$1.class
--rw-rw-r--  2.0 unx     6658 b- defN 23-Jul-21 10:47 org/jpmml/python/SimpleCharStream.class
--rw-rw-r--  2.0 unx     9499 b- defN 23-Jul-21 10:47 org/jpmml/python/FunctionDefParser.class
--rw-rw-r--  2.0 unx     1139 b- defN 23-Jul-21 10:47 org/jpmml/python/InputStreamStorage.class
--rw-rw-r--  2.0 unx      986 b- defN 23-Jul-21 10:47 org/jpmml/python/ExpressionTranslator$Block.class
--rw-rw-r--  2.0 unx      914 b- defN 23-Jul-21 10:47 org/jpmml/python/CompressedInputStreamStorage$Type$1.class
--rw-rw-r--  2.0 unx     4624 b- defN 23-Jul-21 10:47 org/jpmml/python/PythonParser.class
--rw-rw-r--  2.0 unx      441 b- defN 23-Jul-21 10:47 org/jpmml/python/NamedTuple.class
--rw-rw-r--  2.0 unx     1303 b- defN 23-Jul-21 10:47 org/jpmml/python/ClassDictUtil$1.class
--rw-rw-r--  2.0 unx      805 b- defN 23-Jul-21 10:47 org/jpmml/python/NullConstructor.class
--rw-rw-r--  2.0 unx     1120 b- defN 23-Jul-21 10:47 org/jpmml/python/PythonTypeUtil.class
--rw-rw-r--  2.0 unx     1145 b- defN 23-Jul-21 10:47 org/jpmml/python/FileStorage.class
--rw-rw-r--  2.0 unx     1117 b- defN 23-Jul-21 10:47 org/jpmml/python/StringProvider.class
--rw-rw-r--  2.0 unx     1299 b- defN 23-Jul-21 10:47 org/jpmml/python/PushbackPythonParserTokenManager.class
--rw-rw-r--  2.0 unx     9731 b- defN 23-Jul-21 10:47 org/jpmml/python/AbstractTranslator.class
--rw-rw-r--  2.0 unx     8911 b- defN 23-Jul-21 10:47 org/jpmml/python/PickleUtil.class
--rw-rw-r--  2.0 unx     2017 b- defN 23-Jul-21 10:47 org/jpmml/python/PythonEnumConstructor.class
--rw-rw-r--  2.0 unx     4475 b- defN 23-Jul-21 10:47 org/jpmml/python/PythonObjectConstructor.class
--rw-rw-r--  2.0 unx      800 b- defN 23-Jul-21 10:47 org/jpmml/python/FunctionDef$Parameter.class
--rw-rw-r--  2.0 unx      183 b- defN 23-Jul-21 10:47 org/jpmml/python/Identifiable.class
--rw-rw-r--  2.0 unx     2647 b- defN 23-Jul-21 10:47 org/jpmml/python/ClassDictConstructorUtil.class
--rw-rw-r--  2.0 unx    10443 b- defN 23-Jul-21 10:47 org/jpmml/python/PythonObject.class
--rw-rw-r--  2.0 unx     1442 b- defN 23-Jul-21 10:47 org/jpmml/python/PythonObject$1.class
--rw-rw-r--  2.0 unx    11022 b- defN 23-Jul-21 10:47 org/jpmml/python/FunctionUtil.class
--rw-rw-r--  2.0 unx     1456 b- defN 23-Jul-21 10:47 org/jpmml/python/PythonObject$3.class
--rw-rw-r--  2.0 unx      239 b- defN 23-Jul-21 10:47 org/jpmml/python/PredicateTranslator$1.class
--rw-rw-r--  2.0 unx      434 b- defN 23-Jul-21 10:47 org/jpmml/python/IConstantConstructor.class
--rw-rw-r--  2.0 unx     1338 b- defN 23-Jul-21 10:47 org/jpmml/python/FunctionDef.class
--rw-rw-r--  2.0 unx      270 b- defN 23-Jul-21 10:47 org/jpmml/python/HasContent.class
--rw-rw-r--  2.0 unx      763 b- defN 23-Jul-21 10:47 org/jpmml/python/FunctionDefParser$LookaheadSuccess.class
--rw-rw-r--  2.0 unx     1545 b- defN 23-Jul-21 10:47 org/jpmml/python/CustomPythonObjectConstructor.class
--rw-rw-r--  2.0 unx     1784 b- defN 23-Jul-21 10:47 org/jpmml/python/CompressedInputStreamStorage$Type.class
--rw-rw-r--  2.0 unx      233 b- defN 23-Jul-21 10:47 org/jpmml/python/FunctionDefParser$1.class
--rw-rw-r--  2.0 unx      534 b- defN 23-Jul-21 10:47 org/jpmml/python/NullProvider.class
--rw-rw-r--  2.0 unx      219 b- defN 23-Jul-21 10:47 org/jpmml/python/Provider.class
--rw-rw-r--  2.0 unx      566 b- defN 23-Jul-21 10:47 org/jpmml/python/PythonEnum.class
--rw-rw-r--  2.0 unx      505 b- defN 23-Jul-21 10:47 org/jpmml/python/PredicateTranslator$JJCalls.class
--rw-rw-r--  2.0 unx     1201 b- defN 23-Jul-21 10:47 org/jpmml/python/CalendarUtil.class
--rw-rw-r--  2.0 unx     1793 b- defN 23-Jul-21 10:47 org/jpmml/python/PythonObject$2.class
--rw-rw-r--  2.0 unx     2786 b- defN 23-Jul-21 10:47 org/jpmml/python/SliceUtil.class
--rw-rw-r--  2.0 unx      234 b- defN 23-Jul-21 10:47 org/jpmml/python/Castable.class
--rw-rw-r--  2.0 unx     1107 b- defN 23-Jul-21 10:47 org/jpmml/python/TupleUtil$1.class
--rw-rw-r--  2.0 unx     1512 b- defN 23-Jul-21 10:47 org/jpmml/python/AbstractTranslator$1.class
--rw-rw-r--  2.0 unx     1795 b- defN 23-Jul-21 10:47 org/jpmml/python/CastFunction.class
--rw-rw-r--  2.0 unx     1106 b- defN 23-Jul-21 10:47 org/jpmml/python/TupleUtil$3.class
--rw-rw-r--  2.0 unx     1873 b- defN 23-Jul-21 10:47 org/jpmml/python/NamedTupleConstructor.class
--rw-rw-r--  2.0 unx      509 b- defN 23-Jul-21 10:47 org/jpmml/python/ExpressionTranslator$JJCalls.class
--rw-rw-r--  2.0 unx      875 b- defN 23-Jul-21 10:47 org/jpmml/python/SliceUtil$1.class
--rw-rw-r--  2.0 unx     2825 b- defN 23-Jul-21 10:47 org/jpmml/python/BlockScope.class
--rw-rw-r--  2.0 unx     4439 b- defN 23-Jul-21 10:47 org/jpmml/python/DataFrameScope.class
--rw-rw-r--  2.0 unx      643 b- defN 23-Jul-21 10:47 org/jpmml/python/PythonEncoder.class
--rw-rw-r--  2.0 unx     1454 b- defN 23-Jul-21 10:47 org/jpmml/python/PythonObject$4.class
--rw-rw-r--  2.0 unx     1729 b- defN 23-Jul-21 10:47 org/jpmml/python/Scope.class
--rw-rw-r--  2.0 unx      911 b- defN 23-Jul-21 10:47 org/jpmml/python/TupleUtil$2.class
--rw-rw-r--  2.0 unx    15487 b- defN 23-Jul-21 10:47 org/jpmml/python/PythonParserTokenManager.class
--rw-rw-r--  2.0 unx     2223 b- defN 23-Jul-21 10:47 org/jpmml/python/CustomPythonObject.class
--rw-rw-r--  2.0 unx    23138 b- defN 23-Jul-21 10:47 org/jpmml/python/PredicateTranslator.class
--rw-rw-r--  2.0 unx     1629 b- defN 23-Jul-21 10:47 org/jpmml/python/StorageUtil.class
--rw-rw-r--  2.0 unx     1128 b- defN 23-Jul-21 10:47 joblib/NDArrayWrapperConstructor$1.class
--rw-rw-r--  2.0 unx     1371 b- defN 23-Jul-21 10:47 joblib/NDArrayWrapperConstructor.class
--rw-rw-r--  2.0 unx     2667 b- defN 23-Jul-21 10:47 joblib/NumpyArrayWrapper.class
--rw-rw-r--  2.0 unx     2493 b- defN 23-Jul-21 10:47 joblib/NDArrayWrapper.class
--rw-rw-r--  2.0 unx      388 b- defN 23-Jul-21 10:47 scipy/stats/RVGeneric.class
--rw-rw-r--  2.0 unx      559 b- defN 23-Jul-21 10:47 scipy/stats/RVContinuous.class
--rw-rw-r--  2.0 unx     1056 b- defN 23-Jul-21 10:47 scipy/interpolate/BSpline.class
--rw-rw-r--  2.0 unx     1541 b- defN 23-Jul-21 10:47 scipy/sparse/CSRMatrix.class
--rw-rw-r--  2.0 unx     2618 b- defN 23-Jul-21 10:47 scipy/sparse/CSRMatrixUtil.class
--rw-rw-r--  2.0 unx     2086 b- defN 23-Jul-21 10:47 builtins/Type.class
--rw-rw-r--  2.0 unx     1190 b- defN 23-Jul-21 10:47 builtins/GetAttr.class
--rw-rw-r--  2.0 unx      536 b- defN 23-Jul-21 10:47 builtins/TypeConstructor.class
--rw-rw-r--  2.0 unx      637 b- defN 23-Jul-21 10:47 builtins/Function.class
--rw-rw-r--  2.0 unx      891 b- defN 23-Jul-21 10:47 builtins/Slice.class
--rw-rw-r--  2.0 unx     5158 b- defN 23-Jul-21 10:47 META-INF/maven/org.jpmml/pmml-python/pom.xml
--rw-rw-r--  2.0 unx       56 b- defN 23-Jul-21 10:47 META-INF/maven/org.jpmml/pmml-python/pom.properties
-182 files, 390163 bytes uncompressed, 183810 bytes compressed:  52.9%
+Zip file size: 210028 bytes, number of entries: 182
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-03 15:42 META-INF/
+-rw-r--r--  2.0 unx      158 b- defN 23-Dec-03 15:42 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-03 15:42 patsy/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-03 15:42 functools/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-03 15:42 types/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-03 15:42 treelib/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-03 15:42 pandas/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-03 15:42 pandas/core/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-03 15:42 dill/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-03 15:42 numpy/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-03 15:42 numpy/random/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-03 15:42 numpy/core/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-03 15:42 collections/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-03 15:42 org/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-03 15:42 org/jpmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-03 15:42 org/jpmml/python/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-03 15:42 joblib/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-03 15:42 scipy/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-03 15:42 scipy/stats/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-03 15:42 scipy/interpolate/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-03 15:42 scipy/sparse/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-03 15:42 builtins/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-03 15:42 META-INF/maven/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-03 15:42 META-INF/maven/org.jpmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-03 15:42 META-INF/maven/org.jpmml/pmml-python/
+-rw-rw-r--  2.0 unx     2108 b- defN 23-Dec-03 15:42 patsy/PatsyOperation.class
+-rw-rw-r--  2.0 unx     2272 b- defN 23-Dec-03 15:42 patsy/PatsyOperator.class
+-rw-rw-r--  2.0 unx     3106 b- defN 23-Dec-03 15:42 patsy/PatsyToken.class
+-rw-rw-r--  2.0 unx      933 b- defN 23-Dec-03 15:42 patsy/PatsyFactor.class
+-rw-rw-r--  2.0 unx      747 b- defN 23-Dec-03 15:42 patsy/PatsyTerm.class
+-rw-rw-r--  2.0 unx     8491 b- defN 23-Dec-03 15:42 patsy/FormulaParser.class
+-rw-rw-r--  2.0 unx     3432 b- defN 23-Dec-03 15:42 META-INF/python2pmml.properties
+-rw-rw-r--  2.0 unx     3301 b- defN 23-Dec-03 15:42 functools/Partial.class
+-rw-rw-r--  2.0 unx     1431 b- defN 23-Dec-03 15:42 types/MethodTypeConstructor.class
+-rw-rw-r--  2.0 unx      495 b- defN 23-Dec-03 15:42 types/MethodType.class
+-rw-rw-r--  2.0 unx     1046 b- defN 23-Dec-03 15:42 types/FunctionType.class
+-rw-rw-r--  2.0 unx     2675 b- defN 23-Dec-03 15:42 treelib/Node.class
+-rw-rw-r--  2.0 unx     2537 b- defN 23-Dec-03 15:42 treelib/Tree.class
+-rw-rw-r--  2.0 unx     1800 b- defN 23-Dec-03 15:42 pandas/NDArrayBackedConstructor.class
+-rw-rw-r--  2.0 unx     2430 b- defN 23-Dec-03 15:42 pandas/NDArrayBacked.class
+-rw-rw-r--  2.0 unx     1117 b- defN 23-Dec-03 15:42 pandas/core/Index$NDArrayData.class
+-rw-rw-r--  2.0 unx     3088 b- defN 23-Dec-03 15:42 pandas/core/Index.class
+-rw-rw-r--  2.0 unx     4337 b- defN 23-Dec-03 15:42 pandas/core/BlockManager.class
+-rw-rw-r--  2.0 unx     1602 b- defN 23-Dec-03 15:42 pandas/core/SingleBlockManager.class
+-rw-rw-r--  2.0 unx      724 b- defN 23-Dec-03 15:42 pandas/core/DataFrame.class
+-rw-rw-r--  2.0 unx     2419 b- defN 23-Dec-03 15:42 pandas/core/MaskedArray.class
+-rw-rw-r--  2.0 unx      565 b- defN 23-Dec-03 15:42 pandas/core/StringDtype.class
+-rw-rw-r--  2.0 unx     3212 b- defN 23-Dec-03 15:42 pandas/core/SeriesUtil.class
+-rw-rw-r--  2.0 unx     2092 b- defN 23-Dec-03 15:42 pandas/core/Series.class
+-rw-rw-r--  2.0 unx     1382 b- defN 23-Dec-03 15:42 pandas/core/Index$RangeData.class
+-rw-rw-r--  2.0 unx     1397 b- defN 23-Dec-03 15:42 pandas/core/CategoricalDtype.class
+-rw-rw-r--  2.0 unx      385 b- defN 23-Dec-03 15:42 pandas/core/StringArray.class
+-rw-rw-r--  2.0 unx      569 b- defN 23-Dec-03 15:42 pandas/core/IntegerDtype.class
+-rw-rw-r--  2.0 unx      703 b- defN 23-Dec-03 15:42 pandas/core/Index$Data.class
+-rw-rw-r--  2.0 unx      569 b- defN 23-Dec-03 15:42 pandas/core/BooleanDtype.class
+-rw-rw-r--  2.0 unx      713 b- defN 23-Dec-03 15:42 pandas/core/Categorical.class
+-rw-rw-r--  2.0 unx      994 b- defN 23-Dec-03 15:42 pandas/core/SeriesUtil$1.class
+-rw-rw-r--  2.0 unx     1122 b- defN 23-Dec-03 15:42 pandas/core/MaskedArray$1.class
+-rw-rw-r--  2.0 unx      453 b- defN 23-Dec-03 15:42 pandas/core/ExtensionDtype.class
+-rw-rw-r--  2.0 unx     1390 b- defN 23-Dec-03 15:42 pandas/core/Block.class
+-rw-rw-r--  2.0 unx     3066 b- defN 23-Dec-03 15:42 dill/CreateCodeConstructor.class
+-rw-rw-r--  2.0 unx     1021 b- defN 23-Dec-03 15:42 dill/CreateTypeConstructor.class
+-rw-rw-r--  2.0 unx     2269 b- defN 23-Dec-03 15:42 dill/LoadTypeConstructor.class
+-rw-rw-r--  2.0 unx     1530 b- defN 23-Dec-03 15:42 dill/CreateArrayConstructor.class
+-rw-rw-r--  2.0 unx     1260 b- defN 23-Dec-03 15:42 dill/CreateFunctionConstructor.class
+-rw-rw-r--  2.0 unx     1172 b- defN 23-Dec-03 15:42 numpy/DTypeUtil.class
+-rw-rw-r--  2.0 unx     1404 b- defN 23-Dec-03 15:42 numpy/random/BitGeneratorUtil.class
+-rw-rw-r--  2.0 unx     1064 b- defN 23-Dec-03 15:42 numpy/random/Generator.class
+-rw-rw-r--  2.0 unx      889 b- defN 23-Dec-03 15:42 numpy/random/BitGenerator.class
+-rw-rw-r--  2.0 unx      953 b- defN 23-Dec-03 15:42 numpy/random/RandomState.class
+-rw-rw-r--  2.0 unx     1077 b- defN 23-Dec-03 15:42 numpy/random/LegacyRandomState.class
+-rw-rw-r--  2.0 unx     4593 b- defN 23-Dec-03 15:42 numpy/DType.class
+-rw-rw-r--  2.0 unx     2147 b- defN 23-Dec-03 15:42 numpy/core/TypeDescriptor$Kind.class
+-rw-rw-r--  2.0 unx     2138 b- defN 23-Dec-03 15:42 numpy/core/MaskedArray.class
+-rw-rw-r--  2.0 unx     1136 b- defN 23-Dec-03 15:42 numpy/core/UFunc.class
+-rw-rw-r--  2.0 unx    12387 b- defN 23-Dec-03 15:42 numpy/core/NDArrayUtil.class
+-rw-rw-r--  2.0 unx      641 b- defN 23-Dec-03 15:42 numpy/core/Function.class
+-rw-rw-r--  2.0 unx     2386 b- defN 23-Dec-03 15:42 numpy/core/FromBufferConstructor.class
+-rw-rw-r--  2.0 unx     1065 b- defN 23-Dec-03 15:42 numpy/core/TypeDescriptor$1.class
+-rw-rw-r--  2.0 unx     4249 b- defN 23-Dec-03 15:42 numpy/core/NDArray.class
+-rw-rw-r--  2.0 unx     5262 b- defN 23-Dec-03 15:42 numpy/core/TypeDescriptor.class
+-rw-rw-r--  2.0 unx     3674 b- defN 23-Dec-03 15:42 numpy/core/Scalar.class
+-rw-rw-r--  2.0 unx      586 b- defN 23-Dec-03 15:42 numpy/core/ScalarUtil.class
+-rw-rw-r--  2.0 unx      109 b- defN 23-Dec-03 15:42 collections/Callable.class
+-rw-rw-r--  2.0 unx      895 b- defN 23-Dec-03 15:42 collections/DefaultDict.class
+-rw-rw-r--  2.0 unx     1467 b- defN 23-Dec-03 15:42 org/jpmml/python/PythonObject$5.class
+-rw-rw-r--  2.0 unx     1256 b- defN 23-Dec-03 15:42 org/jpmml/python/Token.class
+-rw-rw-r--  2.0 unx     2928 b- defN 23-Dec-03 15:42 org/jpmml/python/TokenMgrException.class
+-rw-rw-r--  2.0 unx     2230 b- defN 23-Dec-03 15:42 org/jpmml/python/TupleUtil.class
+-rw-rw-r--  2.0 unx     2779 b- defN 23-Dec-03 15:42 org/jpmml/python/PythonParserConstants.class
+-rw-rw-r--  2.0 unx      472 b- defN 23-Dec-03 15:42 org/jpmml/python/Storage.class
+-rw-rw-r--  2.0 unx     1689 b- defN 23-Dec-03 15:42 org/jpmml/python/CustomUnpickler.class
+-rw-rw-r--  2.0 unx      497 b- defN 23-Dec-03 15:42 org/jpmml/python/FunctionDefParser$JJCalls.class
+-rw-rw-r--  2.0 unx      914 b- defN 23-Dec-03 15:42 org/jpmml/python/CompressedInputStreamStorage$Type$2.class
+-rw-rw-r--  2.0 unx     1381 b- defN 23-Dec-03 15:42 org/jpmml/python/CompressedInputStreamStorage$1.class
+-rw-rw-r--  2.0 unx      242 b- defN 23-Dec-03 15:42 org/jpmml/python/ExpressionTranslator$1.class
+-rw-rw-r--  2.0 unx     4157 b- defN 23-Dec-03 15:42 org/jpmml/python/ParseException.class
+-rw-rw-r--  2.0 unx      282 b- defN 23-Dec-03 15:42 org/jpmml/python/HasArray.class
+-rw-rw-r--  2.0 unx     3481 b- defN 23-Dec-03 15:42 org/jpmml/python/PythonParserUtil.class
+-rw-rw-r--  2.0 unx     2631 b- defN 23-Dec-03 15:42 org/jpmml/python/FunctionDefScope.class
+-rw-rw-r--  2.0 unx      784 b- defN 23-Dec-03 15:42 org/jpmml/python/ExpressionTranslator$LookaheadSuccess.class
+-rw-rw-r--  2.0 unx     2861 b- defN 23-Dec-03 15:42 org/jpmml/python/CompressedInputStreamStorage.class
+-rw-rw-r--  2.0 unx      777 b- defN 23-Dec-03 15:42 org/jpmml/python/PredicateTranslator$LookaheadSuccess.class
+-rw-rw-r--  2.0 unx     1016 b- defN 23-Dec-03 15:42 org/jpmml/python/CastUtil.class
+-rw-rw-r--  2.0 unx      164 b- defN 23-Dec-03 15:42 org/jpmml/python/TypeInfo.class
+-rw-rw-r--  2.0 unx     6636 b- defN 23-Dec-03 15:42 org/jpmml/python/ClassDictUtil.class
+-rw-rw-r--  2.0 unx    41024 b- defN 23-Dec-03 15:42 org/jpmml/python/ExpressionTranslator.class
+-rw-rw-r--  2.0 unx     1294 b- defN 23-Dec-03 15:42 org/jpmml/python/StreamProvider.class
+-rw-rw-r--  2.0 unx     1340 b- defN 23-Dec-03 15:42 org/jpmml/python/PickleUtil$1.class
+-rw-rw-r--  2.0 unx     6658 b- defN 23-Dec-03 15:42 org/jpmml/python/SimpleCharStream.class
+-rw-rw-r--  2.0 unx     9499 b- defN 23-Dec-03 15:42 org/jpmml/python/FunctionDefParser.class
+-rw-rw-r--  2.0 unx     1139 b- defN 23-Dec-03 15:42 org/jpmml/python/InputStreamStorage.class
+-rw-rw-r--  2.0 unx      986 b- defN 23-Dec-03 15:42 org/jpmml/python/ExpressionTranslator$Block.class
+-rw-rw-r--  2.0 unx      914 b- defN 23-Dec-03 15:42 org/jpmml/python/CompressedInputStreamStorage$Type$1.class
+-rw-rw-r--  2.0 unx     4624 b- defN 23-Dec-03 15:42 org/jpmml/python/PythonParser.class
+-rw-rw-r--  2.0 unx      441 b- defN 23-Dec-03 15:42 org/jpmml/python/NamedTuple.class
+-rw-rw-r--  2.0 unx     1303 b- defN 23-Dec-03 15:42 org/jpmml/python/ClassDictUtil$1.class
+-rw-rw-r--  2.0 unx      805 b- defN 23-Dec-03 15:42 org/jpmml/python/NullConstructor.class
+-rw-rw-r--  2.0 unx     1120 b- defN 23-Dec-03 15:42 org/jpmml/python/PythonTypeUtil.class
+-rw-rw-r--  2.0 unx     1145 b- defN 23-Dec-03 15:42 org/jpmml/python/FileStorage.class
+-rw-rw-r--  2.0 unx     1117 b- defN 23-Dec-03 15:42 org/jpmml/python/StringProvider.class
+-rw-rw-r--  2.0 unx     1299 b- defN 23-Dec-03 15:42 org/jpmml/python/PushbackPythonParserTokenManager.class
+-rw-rw-r--  2.0 unx     9731 b- defN 23-Dec-03 15:42 org/jpmml/python/AbstractTranslator.class
+-rw-rw-r--  2.0 unx     8911 b- defN 23-Dec-03 15:42 org/jpmml/python/PickleUtil.class
+-rw-rw-r--  2.0 unx     2017 b- defN 23-Dec-03 15:42 org/jpmml/python/PythonEnumConstructor.class
+-rw-rw-r--  2.0 unx     4475 b- defN 23-Dec-03 15:42 org/jpmml/python/PythonObjectConstructor.class
+-rw-rw-r--  2.0 unx      800 b- defN 23-Dec-03 15:42 org/jpmml/python/FunctionDef$Parameter.class
+-rw-rw-r--  2.0 unx      183 b- defN 23-Dec-03 15:42 org/jpmml/python/Identifiable.class
+-rw-rw-r--  2.0 unx     2647 b- defN 23-Dec-03 15:42 org/jpmml/python/ClassDictConstructorUtil.class
+-rw-rw-r--  2.0 unx    10443 b- defN 23-Dec-03 15:42 org/jpmml/python/PythonObject.class
+-rw-rw-r--  2.0 unx     1442 b- defN 23-Dec-03 15:42 org/jpmml/python/PythonObject$1.class
+-rw-rw-r--  2.0 unx    11022 b- defN 23-Dec-03 15:42 org/jpmml/python/FunctionUtil.class
+-rw-rw-r--  2.0 unx     1456 b- defN 23-Dec-03 15:42 org/jpmml/python/PythonObject$3.class
+-rw-rw-r--  2.0 unx      239 b- defN 23-Dec-03 15:42 org/jpmml/python/PredicateTranslator$1.class
+-rw-rw-r--  2.0 unx      434 b- defN 23-Dec-03 15:42 org/jpmml/python/IConstantConstructor.class
+-rw-rw-r--  2.0 unx     1338 b- defN 23-Dec-03 15:42 org/jpmml/python/FunctionDef.class
+-rw-rw-r--  2.0 unx      270 b- defN 23-Dec-03 15:42 org/jpmml/python/HasContent.class
+-rw-rw-r--  2.0 unx      763 b- defN 23-Dec-03 15:42 org/jpmml/python/FunctionDefParser$LookaheadSuccess.class
+-rw-rw-r--  2.0 unx     1545 b- defN 23-Dec-03 15:42 org/jpmml/python/CustomPythonObjectConstructor.class
+-rw-rw-r--  2.0 unx     1784 b- defN 23-Dec-03 15:42 org/jpmml/python/CompressedInputStreamStorage$Type.class
+-rw-rw-r--  2.0 unx      233 b- defN 23-Dec-03 15:42 org/jpmml/python/FunctionDefParser$1.class
+-rw-rw-r--  2.0 unx      534 b- defN 23-Dec-03 15:42 org/jpmml/python/NullProvider.class
+-rw-rw-r--  2.0 unx      219 b- defN 23-Dec-03 15:42 org/jpmml/python/Provider.class
+-rw-rw-r--  2.0 unx      566 b- defN 23-Dec-03 15:42 org/jpmml/python/PythonEnum.class
+-rw-rw-r--  2.0 unx      505 b- defN 23-Dec-03 15:42 org/jpmml/python/PredicateTranslator$JJCalls.class
+-rw-rw-r--  2.0 unx     1201 b- defN 23-Dec-03 15:42 org/jpmml/python/CalendarUtil.class
+-rw-rw-r--  2.0 unx     1793 b- defN 23-Dec-03 15:42 org/jpmml/python/PythonObject$2.class
+-rw-rw-r--  2.0 unx     2786 b- defN 23-Dec-03 15:42 org/jpmml/python/SliceUtil.class
+-rw-rw-r--  2.0 unx      234 b- defN 23-Dec-03 15:42 org/jpmml/python/Castable.class
+-rw-rw-r--  2.0 unx     1107 b- defN 23-Dec-03 15:42 org/jpmml/python/TupleUtil$1.class
+-rw-rw-r--  2.0 unx     1512 b- defN 23-Dec-03 15:42 org/jpmml/python/AbstractTranslator$1.class
+-rw-rw-r--  2.0 unx     1795 b- defN 23-Dec-03 15:42 org/jpmml/python/CastFunction.class
+-rw-rw-r--  2.0 unx     1106 b- defN 23-Dec-03 15:42 org/jpmml/python/TupleUtil$3.class
+-rw-rw-r--  2.0 unx     1873 b- defN 23-Dec-03 15:42 org/jpmml/python/NamedTupleConstructor.class
+-rw-rw-r--  2.0 unx      509 b- defN 23-Dec-03 15:42 org/jpmml/python/ExpressionTranslator$JJCalls.class
+-rw-rw-r--  2.0 unx      875 b- defN 23-Dec-03 15:42 org/jpmml/python/SliceUtil$1.class
+-rw-rw-r--  2.0 unx     2825 b- defN 23-Dec-03 15:42 org/jpmml/python/BlockScope.class
+-rw-rw-r--  2.0 unx     4439 b- defN 23-Dec-03 15:42 org/jpmml/python/DataFrameScope.class
+-rw-rw-r--  2.0 unx      643 b- defN 23-Dec-03 15:42 org/jpmml/python/PythonEncoder.class
+-rw-rw-r--  2.0 unx     1454 b- defN 23-Dec-03 15:42 org/jpmml/python/PythonObject$4.class
+-rw-rw-r--  2.0 unx     1729 b- defN 23-Dec-03 15:42 org/jpmml/python/Scope.class
+-rw-rw-r--  2.0 unx      911 b- defN 23-Dec-03 15:42 org/jpmml/python/TupleUtil$2.class
+-rw-rw-r--  2.0 unx    15487 b- defN 23-Dec-03 15:42 org/jpmml/python/PythonParserTokenManager.class
+-rw-rw-r--  2.0 unx     2223 b- defN 23-Dec-03 15:42 org/jpmml/python/CustomPythonObject.class
+-rw-rw-r--  2.0 unx    24709 b- defN 23-Dec-03 15:42 org/jpmml/python/PredicateTranslator.class
+-rw-rw-r--  2.0 unx     1629 b- defN 23-Dec-03 15:42 org/jpmml/python/StorageUtil.class
+-rw-rw-r--  2.0 unx     1128 b- defN 23-Dec-03 15:42 joblib/NDArrayWrapperConstructor$1.class
+-rw-rw-r--  2.0 unx     1371 b- defN 23-Dec-03 15:42 joblib/NDArrayWrapperConstructor.class
+-rw-rw-r--  2.0 unx     2667 b- defN 23-Dec-03 15:42 joblib/NumpyArrayWrapper.class
+-rw-rw-r--  2.0 unx     2493 b- defN 23-Dec-03 15:42 joblib/NDArrayWrapper.class
+-rw-rw-r--  2.0 unx      388 b- defN 23-Dec-03 15:42 scipy/stats/RVGeneric.class
+-rw-rw-r--  2.0 unx      559 b- defN 23-Dec-03 15:42 scipy/stats/RVContinuous.class
+-rw-rw-r--  2.0 unx     1056 b- defN 23-Dec-03 15:42 scipy/interpolate/BSpline.class
+-rw-rw-r--  2.0 unx     1541 b- defN 23-Dec-03 15:42 scipy/sparse/CSRMatrix.class
+-rw-rw-r--  2.0 unx     2618 b- defN 23-Dec-03 15:42 scipy/sparse/CSRMatrixUtil.class
+-rw-rw-r--  2.0 unx     2086 b- defN 23-Dec-03 15:42 builtins/Type.class
+-rw-rw-r--  2.0 unx     1190 b- defN 23-Dec-03 15:42 builtins/GetAttr.class
+-rw-rw-r--  2.0 unx      536 b- defN 23-Dec-03 15:42 builtins/TypeConstructor.class
+-rw-rw-r--  2.0 unx      637 b- defN 23-Dec-03 15:42 builtins/Function.class
+-rw-rw-r--  2.0 unx      891 b- defN 23-Dec-03 15:42 builtins/Slice.class
+-rw-rw-r--  2.0 unx     5158 b- defN 23-Dec-03 15:41 META-INF/maven/org.jpmml/pmml-python/pom.xml
+-rw-rw-r--  2.0 unx       56 b- defN 23-Dec-03 15:42 META-INF/maven/org.jpmml/pmml-python/pom.properties
+182 files, 392892 bytes uncompressed, 184726 bytes compressed:  53.0%
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,6 @@
 Manifest-Version: 1.0
 Implementation-Title: JPMML-Python library
-Implementation-Version: 1.1.17
+Implementation-Version: 1.1.18
 Build-Jdk-Spec: 1.8
 Created-By: Maven JAR Plugin 3.3.0
```

#### org/jpmml/python/TokenMgrException.class

##### procyon -ec {}

```diff
@@ -58,15 +58,15 @@
                 }
             }
         }
         return retval.toString();
     }
     
     protected static String LexicalErr(final boolean EOFSeen, final int lexState, final int errorLine, final int errorColumn, final String errorAfter, final int curChar) {
-        return "Lexical error at line " + errorLine + ", column " + errorColumn + ".  Encountered: " + (EOFSeen ? "<EOF>" : ("'" + addEscapes(String.valueOf(curChar)) + "' (" + curChar + "),")) + ((errorAfter == null || errorAfter.length() == 0) ? "" : (" after prefix \"" + addEscapes(errorAfter) + "\"")) + ((lexState == 0) ? "" : (" (in lexical state " + lexState + ")"));
+        return "Lexical error at line " + errorLine + ", column " + errorColumn + ".  Encountered: " + (EOFSeen ? "<EOF>" : ("'" + addEscapes(String.valueOf((char)curChar)) + "' (" + curChar + "),")) + ((errorAfter == null || errorAfter.length() == 0) ? "" : (" after prefix \"" + addEscapes(errorAfter) + "\"")) + ((lexState == 0) ? "" : (" (in lexical state " + lexState + ")"));
     }
     
     @Override
     public String getMessage() {
         return super.getMessage();
     }
```

#### org/jpmml/python/ExpressionTranslator$LookaheadSuccess.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum f83a0f4f2f71739346c5297a85b942fa501dff712c3ef8bcfd967fa9ef46edb1
+  SHA-256 checksum f4ea90faac9365b3a51e2a2f0582ab8cce547eb8bb52e5e118376a8f5095ba5a
   Compiled from "ExpressionTranslator.java"
 final class org.jpmml.python.ExpressionTranslator$LookaheadSuccess extends java.lang.RuntimeException
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #3                          // org/jpmml/python/ExpressionTranslator$LookaheadSuccess
   super_class: #4                         // java/lang/RuntimeException
@@ -41,42 +41,42 @@
     flags: (0x0002) ACC_PRIVATE
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #2                  // Method java/lang/RuntimeException."<init>":()V
          4: return
       LineNumberTable:
-        line 1873: 0
+        line 1930: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lorg/jpmml/python/ExpressionTranslator$LookaheadSuccess;
 
   public java.lang.Throwable fillInStackTrace();
     descriptor: ()Ljava/lang/Throwable;
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: areturn
       LineNumberTable:
-        line 1876: 0
+        line 1933: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       2     0  this   Lorg/jpmml/python/ExpressionTranslator$LookaheadSuccess;
 
   org.jpmml.python.ExpressionTranslator$LookaheadSuccess(org.jpmml.python.ExpressionTranslator$1);
     descriptor: (Lorg/jpmml/python/ExpressionTranslator$1;)V
     flags: (0x1000) ACC_SYNTHETIC
     Code:
       stack=1, locals=2, args_size=2
          0: aload_0
          1: invokespecial #1                  // Method "<init>":()V
          4: return
       LineNumberTable:
-        line 1873: 0
+        line 1930: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lorg/jpmml/python/ExpressionTranslator$LookaheadSuccess;
             0       5     1    x0   Lorg/jpmml/python/ExpressionTranslator$1;
 }
 SourceFile: "ExpressionTranslator.java"
 InnerClasses:
```

#### org/jpmml/python/PredicateTranslator$LookaheadSuccess.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 4ad719d60887b3f40566bff117b3da783949b3c6bf92db18f62c7b0de54081ee
+  SHA-256 checksum 07ecd88deee2e00f88e8aa8f0793988e8668f63267c7920dcc8df523419ff250
   Compiled from "PredicateTranslator.java"
 final class org.jpmml.python.PredicateTranslator$LookaheadSuccess extends java.lang.RuntimeException
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #3                          // org/jpmml/python/PredicateTranslator$LookaheadSuccess
   super_class: #4                         // java/lang/RuntimeException
@@ -41,42 +41,42 @@
     flags: (0x0002) ACC_PRIVATE
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #2                  // Method java/lang/RuntimeException."<init>":()V
          4: return
       LineNumberTable:
-        line 833: 0
+        line 925: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lorg/jpmml/python/PredicateTranslator$LookaheadSuccess;
 
   public java.lang.Throwable fillInStackTrace();
     descriptor: ()Ljava/lang/Throwable;
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: areturn
       LineNumberTable:
-        line 836: 0
+        line 928: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       2     0  this   Lorg/jpmml/python/PredicateTranslator$LookaheadSuccess;
 
   org.jpmml.python.PredicateTranslator$LookaheadSuccess(org.jpmml.python.PredicateTranslator$1);
     descriptor: (Lorg/jpmml/python/PredicateTranslator$1;)V
     flags: (0x1000) ACC_SYNTHETIC
     Code:
       stack=1, locals=2, args_size=2
          0: aload_0
          1: invokespecial #1                  // Method "<init>":()V
          4: return
       LineNumberTable:
-        line 833: 0
+        line 925: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lorg/jpmml/python/PredicateTranslator$LookaheadSuccess;
             0       5     1    x0   Lorg/jpmml/python/PredicateTranslator$1;
 }
 SourceFile: "PredicateTranslator.java"
 InnerClasses:
```

#### org/jpmml/python/ExpressionTranslator.class

##### procyon -ec {}

```diff
@@ -479,14 +479,80 @@
                 this.jj_consume_token(-1);
                 throw new ParseException();
             }
         }
         return token;
     }
     
+    private final int ColumnIndex() throws ParseException {
+        Token sign = null;
+        switch ((this.jj_ntk == -1) ? this.jj_ntk_f() : this.jj_ntk) {
+            case 16:
+            case 17: {
+                sign = this.Sign();
+                break;
+            }
+            default: {
+                this.jj_la1[2] = this.jj_gen;
+                break;
+            }
+        }
+        final Token column = this.jj_consume_token(41);
+        return PythonParserUtil.parseInt(sign, column);
+    }
+    
+    private final int ArrayColumnIndex() throws ParseException {
+        int columnIndex = 0;
+        Label_0222: {
+            switch ((this.jj_ntk == -1) ? this.jj_ntk_f() : this.jj_ntk) {
+                case 27: {
+                    this.jj_consume_token(27);
+                    this.jj_consume_token(25);
+                    switch ((this.jj_ntk == -1) ? this.jj_ntk_f() : this.jj_ntk) {
+                        case 23: {
+                            this.jj_consume_token(23);
+                            columnIndex = this.ColumnIndex();
+                            this.jj_consume_token(24);
+                            break Label_0222;
+                        }
+                        case 16:
+                        case 17:
+                        case 41: {
+                            columnIndex = this.ColumnIndex();
+                            break Label_0222;
+                        }
+                        default: {
+                            this.jj_la1[3] = this.jj_gen;
+                            this.jj_consume_token(-1);
+                            throw new ParseException();
+                        }
+                    }
+                    break;
+                }
+                case 16:
+                case 17:
+                case 41: {
+                    columnIndex = this.ColumnIndex();
+                    break;
+                }
+                default: {
+                    this.jj_la1[4] = this.jj_gen;
+                    this.jj_consume_token(-1);
+                    throw new ParseException();
+                }
+            }
+        }
+        return columnIndex;
+    }
+    
+    private final String ColumnName() throws ParseException {
+        final Token column = this.String();
+        return PythonParserUtil.parseString(column);
+    }
+    
     private final String DottedName() throws ParseException {
         final StringBuilder sb = new StringBuilder();
         Token name = this.jj_consume_token(43);
         sb.append(name.image);
         while (this.jj_2_1(Integer.MAX_VALUE)) {
             this.jj_consume_token(26);
             name = this.jj_consume_token(43);
@@ -505,15 +571,15 @@
         while (true) {
             switch ((this.jj_ntk == -1) ? this.jj_ntk_f() : this.jj_ntk) {
                 case 3: {
                     this.jj_consume_token(3);
                     continue;
                 }
                 default: {
-                    this.jj_la1[2] = this.jj_gen;
+                    this.jj_la1[5] = this.jj_gen;
                     this.jj_consume_token(0);
                     return derivedField;
                 }
             }
         }
     }
     
@@ -522,15 +588,15 @@
         while (true) {
             switch ((this.jj_ntk == -1) ? this.jj_ntk_f() : this.jj_ntk) {
                 case 3: {
                     this.jj_consume_token(3);
                     continue;
                 }
                 default: {
-                    this.jj_la1[3] = this.jj_gen;
+                    this.jj_la1[6] = this.jj_gen;
                     this.jj_consume_token(0);
                     return expression;
                 }
             }
         }
     }
     
@@ -549,15 +615,15 @@
         final ExpressionTranslator.Block block = this.Block();
         this.variableMap.clear();
         return this.createDerivedField(name.image, getOnlyStatement((List<Expression>)block));
     }
     
     private final List<Token> Parameters() throws ParseException {
         final List<Token> names = new ArrayList<Token>();
-        Label_0202: {
+        Label_0204: {
             if (this.jj_2_2(Integer.MAX_VALUE)) {
                 this.jj_consume_token(4);
                 this.jj_consume_token(5);
             }
             else {
                 switch ((this.jj_ntk == -1) ? this.jj_ntk_f() : this.jj_ntk) {
                     case 4: {
@@ -569,24 +635,24 @@
                                 case 25: {
                                     this.jj_consume_token(25);
                                     name = this.jj_consume_token(43);
                                     names.add(name);
                                     continue;
                                 }
                                 default: {
-                                    this.jj_la1[4] = this.jj_gen;
+                                    this.jj_la1[7] = this.jj_gen;
                                     this.jj_consume_token(5);
-                                    break Label_0202;
+                                    break Label_0204;
                                 }
                             }
                         }
                         break;
                     }
                     default: {
-                        this.jj_la1[5] = this.jj_gen;
+                        this.jj_la1[8] = this.jj_gen;
                         this.jj_consume_token(-1);
                         throw new ParseException();
                     }
                 }
             }
         }
         return names;
@@ -600,15 +666,15 @@
                     while (true) {
                         this.jj_consume_token(3);
                         switch ((this.jj_ntk == -1) ? this.jj_ntk_f() : this.jj_ntk) {
                             case 3: {
                                 continue;
                             }
                             default: {
-                                this.jj_la1[6] = this.jj_gen;
+                                this.jj_la1[9] = this.jj_gen;
                                 this.Indent();
                                 statements = this.Statements();
                                 this.Dedent();
                                 break Label_0338;
                             }
                         }
                     }
@@ -628,15 +694,15 @@
                 case 43:
                 case 44:
                 case 51: {
                     statements = this.SimpleStatements();
                     break;
                 }
                 default: {
-                    this.jj_la1[7] = this.jj_gen;
+                    this.jj_la1[10] = this.jj_gen;
                     this.jj_consume_token(-1);
                     throw new ParseException();
                 }
             }
         }
         return new ExpressionTranslator.Block((List)statements, (ExpressionTranslator.ExpressionTranslator$1)null);
     }
@@ -680,15 +746,15 @@
                 case 44:
                 case 51: {
                     final Expression statement = this.Statement();
                     statements.add(statement);
                     break;
                 }
                 default: {
-                    this.jj_la1[8] = this.jj_gen;
+                    this.jj_la1[11] = this.jj_gen;
                     this.jj_consume_token(-1);
                     throw new ParseException();
                 }
             }
             switch ((this.jj_ntk == -1) ? this.jj_ntk_f() : this.jj_ntk) {
                 case 3:
                 case 4:
@@ -705,15 +771,15 @@
                 case 42:
                 case 43:
                 case 44:
                 case 51: {
                     continue;
                 }
                 default: {
-                    this.jj_la1[9] = this.jj_gen;
+                    this.jj_la1[12] = this.jj_gen;
                     return statements;
                 }
             }
         }
     }
     
     private final Expression Statement() throws ParseException {
@@ -740,15 +806,15 @@
             case 44:
             case 51: {
                 final List<Expression> statements = this.SimpleStatements();
                 statement = getOnlyStatement(statements);
                 break;
             }
             default: {
-                this.jj_la1[10] = this.jj_gen;
+                this.jj_la1[13] = this.jj_gen;
                 this.jj_consume_token(-1);
                 throw new ParseException();
             }
         }
         return statement;
     }
     
@@ -766,15 +832,15 @@
                 case 28: {
                     this.jj_consume_token(28);
                     statement = this.SimpleStatement();
                     statements.add(statement);
                     continue;
                 }
                 default: {
-                    this.jj_la1[11] = this.jj_gen;
+                    this.jj_la1[14] = this.jj_gen;
                     this.jj_consume_token(3);
                     return statements;
                 }
             }
         }
     }
     
@@ -801,15 +867,15 @@
                 break;
             }
             case 37: {
                 expression = this.ImportStatement();
                 break;
             }
             default: {
-                this.jj_la1[12] = this.jj_gen;
+                this.jj_la1[15] = this.jj_gen;
                 this.jj_consume_token(-1);
                 throw new ParseException();
             }
         }
         return expression;
     }
     
@@ -825,23 +891,23 @@
                 case 34: {
                     final Apply elif_statement = this.ElIfStatement();
                     tail.addExpressions(new Expression[] { (Expression)elif_statement });
                     tail = elif_statement;
                     continue;
                 }
                 default: {
-                    this.jj_la1[13] = this.jj_gen;
+                    this.jj_la1[16] = this.jj_gen;
                     switch ((this.jj_ntk == -1) ? this.jj_ntk_f() : this.jj_ntk) {
                         case 35: {
                             block = this.ElseBlock();
                             tail.addExpressions(new Expression[] { getOnlyStatement((List<Expression>)block) });
                             break;
                         }
                         default: {
-                            this.jj_la1[14] = this.jj_gen;
+                            this.jj_la1[17] = this.jj_gen;
                             break;
                         }
                     }
                     return if_statement;
                 }
             }
         }
@@ -896,15 +962,15 @@
             switch ((this.jj_ntk == -1) ? this.jj_ntk_f() : this.jj_ntk) {
                 case 25: {
                     this.jj_consume_token(25);
                     this.DottedAsName();
                     continue;
                 }
                 default: {
-                    this.jj_la1[15] = this.jj_gen;
+                    this.jj_la1[18] = this.jj_gen;
                     return null;
                 }
             }
         }
     }
     
     private final void DottedAsName() throws ParseException {
@@ -913,15 +979,15 @@
         switch ((this.jj_ntk == -1) ? this.jj_ntk_f() : this.jj_ntk) {
             case 32: {
                 this.jj_consume_token(32);
                 name = this.jj_consume_token(43);
                 break;
             }
             default: {
-                this.jj_la1[16] = this.jj_gen;
+                this.jj_la1[19] = this.jj_gen;
                 break;
             }
         }
         final Map<String, String> moduleImports = this.getModuleImports();
         moduleImports.put((name != null) ? name.image : dottedName, dottedName);
     }
     
@@ -938,15 +1004,15 @@
                 final Expression center = this.Expression();
                 this.jj_consume_token(35);
                 final Expression right = this.Expression();
                 left = (Expression)PMMLUtil.createApply("if", new Expression[] { center, left, right });
                 break;
             }
             default: {
-                this.jj_la1[17] = this.jj_gen;
+                this.jj_la1[20] = this.jj_gen;
                 break;
             }
         }
         return left;
     }
     
     private final Expression LogicalOrExpression() throws ParseException {
@@ -956,15 +1022,15 @@
                 case 6: {
                     this.jj_consume_token(6);
                     final Expression right = this.LogicalAndExpression();
                     left = (Expression)PMMLUtil.createApply("or", new Expression[] { left, right });
                     continue;
                 }
                 default: {
-                    this.jj_la1[18] = this.jj_gen;
+                    this.jj_la1[21] = this.jj_gen;
                     return left;
                 }
             }
         }
     }
     
     private final Expression LogicalAndExpression() throws ParseException {
@@ -974,30 +1040,30 @@
                 case 7: {
                     this.jj_consume_token(7);
                     final Expression right = this.NegationExpression();
                     left = (Expression)PMMLUtil.createApply("and", new Expression[] { left, right });
                     continue;
                 }
                 default: {
-                    this.jj_la1[19] = this.jj_gen;
+                    this.jj_la1[22] = this.jj_gen;
                     return left;
                 }
             }
         }
     }
     
     private final Expression NegationExpression() throws ParseException {
         Token operator = null;
         switch ((this.jj_ntk == -1) ? this.jj_ntk_f() : this.jj_ntk) {
             case 8: {
                 operator = this.jj_consume_token(8);
                 break;
             }
             default: {
-                this.jj_la1[20] = this.jj_gen;
+                this.jj_la1[23] = this.jj_gen;
                 break;
             }
         }
         final Expression expression = this.ComparisonExpression();
         if (operator != null) {
             return (Expression)PMMLUtil.createApply("not", new Expression[] { expression });
         }
@@ -1031,15 +1097,15 @@
                         this.jj_consume_token(8);
                         this.jj_consume_token(38);
                         final Object right = this.ListMakerExpression();
                         left = (Expression)PMMLUtil.createApply("isNotIn", new Expression[] { left }).addExpressions((Expression[])(Expression[])right);
                         break;
                     }
                     default: {
-                        this.jj_la1[23] = this.jj_gen;
+                        this.jj_la1[26] = this.jj_gen;
                         switch ((this.jj_ntk == -1) ? this.jj_ntk_f() : this.jj_ntk) {
                             case 9:
                             case 10:
                             case 11:
                             case 12:
                             case 13:
                             case 14: {
@@ -1066,25 +1132,25 @@
                                         break;
                                     }
                                     case 14: {
                                         operator = this.jj_consume_token(14);
                                         break;
                                     }
                                     default: {
-                                        this.jj_la1[21] = this.jj_gen;
+                                        this.jj_la1[24] = this.jj_gen;
                                         this.jj_consume_token(-1);
                                         throw new ParseException();
                                     }
                                 }
                                 final Object right = this.AdditiveExpression();
                                 left = (Expression)PMMLUtil.createApply(translateRelationalOperator(operator), new Expression[] { left, (Expression)right });
                                 break Label_0475;
                             }
                             default: {
-                                this.jj_la1[22] = this.jj_gen;
+                                this.jj_la1[25] = this.jj_gen;
                                 break Label_0475;
                             }
                         }
                         break;
                     }
                 }
             }
@@ -1105,29 +1171,29 @@
                             break;
                         }
                         case 17: {
                             operator = this.jj_consume_token(17);
                             break;
                         }
                         default: {
-                            this.jj_la1[25] = this.jj_gen;
+                            this.jj_la1[28] = this.jj_gen;
                             this.jj_consume_token(-1);
                             throw new ParseException();
                         }
                     }
                     final Expression right = this.MultiplicativeExpression();
                     if (operator.kind == 16 && TypeUtil.isString(left, (FeatureResolver)this) && TypeUtil.isString(right, (FeatureResolver)this)) {
                         left = (Expression)PMMLUtil.createApply("concat", new Expression[] { left, right });
                         continue;
                     }
                     left = (Expression)PMMLUtil.createApply(translateArithmeticOperator(operator), new Expression[] { left, right });
                     continue;
                 }
                 default: {
-                    this.jj_la1[24] = this.jj_gen;
+                    this.jj_la1[27] = this.jj_gen;
                     return left;
                 }
             }
         }
     }
     
     private final Expression MultiplicativeExpression() throws ParseException {
@@ -1148,25 +1214,25 @@
                             break;
                         }
                         case 20: {
                             operator = this.jj_consume_token(20);
                             break;
                         }
                         default: {
-                            this.jj_la1[27] = this.jj_gen;
+                            this.jj_la1[30] = this.jj_gen;
                             this.jj_consume_token(-1);
                             throw new ParseException();
                         }
                     }
                     final Expression right = this.UnaryExpression();
                     left = (Expression)PMMLUtil.createApply(translateArithmeticOperator(operator), new Expression[] { left, right });
                     continue;
                 }
                 default: {
-                    this.jj_la1[26] = this.jj_gen;
+                    this.jj_la1[29] = this.jj_gen;
                     return left;
                 }
             }
         }
     }
     
     private final Expression UnaryExpression() throws ParseException {
@@ -1188,15 +1254,15 @@
             case 43:
             case 44:
             case 51: {
                 expression = this.PowerExpression();
                 break;
             }
             default: {
-                this.jj_la1[28] = this.jj_gen;
+                this.jj_la1[31] = this.jj_gen;
                 this.jj_consume_token(-1);
                 throw new ParseException();
             }
         }
         if (sign != null && sign.kind == 17) {
             expression = PMMLUtil.toNegative(expression);
         }
@@ -1209,15 +1275,15 @@
             case 22: {
                 this.jj_consume_token(22);
                 final Expression right = this.UnaryExpression();
                 left = (Expression)PMMLUtil.createApply("pow", new Expression[] { left, right });
                 break;
             }
             default: {
-                this.jj_la1[29] = this.jj_gen;
+                this.jj_la1[32] = this.jj_gen;
                 break;
             }
         }
         return left;
     }
     
     private final Expression PrimaryExpression() throws ParseException {
@@ -1238,23 +1304,23 @@
                                             continue;
                                         }
                                         case 23: {
                                             expression = this.StringSlicingExpression(expression);
                                             continue;
                                         }
                                         default: {
-                                            this.jj_la1[31] = this.jj_gen;
+                                            this.jj_la1[34] = this.jj_gen;
                                             this.jj_consume_token(-1);
                                             throw new ParseException();
                                         }
                                     }
                                     break;
                                 }
                                 default: {
-                                    this.jj_la1[30] = this.jj_gen;
+                                    this.jj_la1[33] = this.jj_gen;
                                     break Label_0884;
                                 }
                             }
                         }
                     }
                     else {
                         switch ((this.jj_ntk == -1) ? this.jj_ntk_f() : this.jj_ntk) {
@@ -1270,31 +1336,31 @@
                                                     continue;
                                                 }
                                                 case 23: {
                                                     expression = this.StringSlicingExpression(expression);
                                                     continue;
                                                 }
                                                 default: {
-                                                    this.jj_la1[33] = this.jj_gen;
+                                                    this.jj_la1[36] = this.jj_gen;
                                                     this.jj_consume_token(-1);
                                                     throw new ParseException();
                                                 }
                                             }
                                             break;
                                         }
                                         default: {
-                                            this.jj_la1[32] = this.jj_gen;
+                                            this.jj_la1[35] = this.jj_gen;
                                             break Label_0884;
                                         }
                                     }
                                 }
                                 break;
                             }
                             default: {
-                                this.jj_la1[37] = this.jj_gen;
+                                this.jj_la1[40] = this.jj_gen;
                                 expression = this.NameInvocationExpression(dottedName);
                                 switch ((this.jj_ntk == -1) ? this.jj_ntk_f() : this.jj_ntk) {
                                     case 23: {
                                         expression = this.StringSlicingExpression(expression);
                                         while (true) {
                                             switch ((this.jj_ntk == -1) ? this.jj_ntk_f() : this.jj_ntk) {
                                                 case 23:
@@ -1305,31 +1371,31 @@
                                                             continue;
                                                         }
                                                         case 23: {
                                                             expression = this.StringSlicingExpression(expression);
                                                             continue;
                                                         }
                                                         default: {
-                                                            this.jj_la1[35] = this.jj_gen;
+                                                            this.jj_la1[38] = this.jj_gen;
                                                             this.jj_consume_token(-1);
                                                             throw new ParseException();
                                                         }
                                                     }
                                                     break;
                                                 }
                                                 default: {
-                                                    this.jj_la1[34] = this.jj_gen;
+                                                    this.jj_la1[37] = this.jj_gen;
                                                     break Label_0884;
                                                 }
                                             }
                                         }
                                         break;
                                     }
                                     default: {
-                                        this.jj_la1[36] = this.jj_gen;
+                                        this.jj_la1[39] = this.jj_gen;
                                         break Label_0884;
                                     }
                                 }
                                 break;
                             }
                         }
                     }
@@ -1347,23 +1413,23 @@
                                         continue;
                                     }
                                     case 23: {
                                         expression = this.StringSlicingExpression(expression);
                                         continue;
                                     }
                                     default: {
-                                        this.jj_la1[39] = this.jj_gen;
+                                        this.jj_la1[42] = this.jj_gen;
                                         this.jj_consume_token(-1);
                                         throw new ParseException();
                                     }
                                 }
                                 break;
                             }
                             default: {
-                                this.jj_la1[38] = this.jj_gen;
+                                this.jj_la1[41] = this.jj_gen;
                                 break Label_0884;
                             }
                         }
                     }
                     break;
                 }
                 case 29:
@@ -1373,69 +1439,54 @@
                 case 42:
                 case 44:
                 case 51: {
                     expression = (Expression)this.LiteralExpression();
                     break;
                 }
                 default: {
-                    this.jj_la1[40] = this.jj_gen;
+                    this.jj_la1[43] = this.jj_gen;
                     this.jj_consume_token(-1);
                     throw new ParseException();
                 }
             }
         }
         return expression;
     }
     
     private final FieldRef ArrayIndexingExpression(final String dottedName) throws ParseException {
-        Token sign = null;
+        final Scope scope = this.ensureScope();
         Feature feature = null;
         if (this.jj_2_6(Integer.MAX_VALUE)) {
             this.jj_consume_token(23);
-            switch ((this.jj_ntk == -1) ? this.jj_ntk_f() : this.jj_ntk) {
-                case 16:
-                case 17: {
-                    sign = this.Sign();
-                    break;
-                }
-                default: {
-                    this.jj_la1[41] = this.jj_gen;
-                    break;
-                }
-            }
-            final Token column = this.jj_consume_token(41);
+            final int colIndex = this.ArrayColumnIndex();
             this.jj_consume_token(24);
-            final Scope scope = this.ensureScope();
-            final int colIndex = PythonParserUtil.parseInt(sign, column);
             feature = scope.getFeature(dottedName, colIndex);
         }
         else {
             switch ((this.jj_ntk == -1) ? this.jj_ntk_f() : this.jj_ntk) {
                 case 23: {
                     this.jj_consume_token(23);
-                    final Token column = this.String();
+                    final String colName = this.ColumnName();
                     this.jj_consume_token(24);
-                    final Scope scope = this.ensureScope();
-                    final String colName = PythonParserUtil.parseString(column);
                     feature = scope.getFeature(dottedName, colName);
                     break;
                 }
                 default: {
-                    this.jj_la1[42] = this.jj_gen;
+                    this.jj_la1[44] = this.jj_gen;
                     this.jj_consume_token(-1);
                     throw new ParseException();
                 }
             }
         }
         return feature.ref();
     }
     
     private final Expression FunctionInvocationExpression(final String dottedName) throws ParseException {
-        final List<Expression> arguments = this.Arguments();
         final Scope scope = this.ensureScope();
+        final List<Expression> arguments = this.Arguments();
         final int dot = dottedName.lastIndexOf(46);
         if (dot > -1) {
             final String featureName = dottedName.substring(0, dot);
             final String functionName = dottedName.substring(dot + 1);
             final Feature feature = scope.resolveFeature(featureName);
             if (feature != null) {
                 return (Expression)translateTrailerFunction((Expression)feature.ref(), functionName, arguments);
@@ -1469,108 +1520,76 @@
                                 case 25: {
                                     this.jj_consume_token(25);
                                     expression = this.Expression();
                                     expressions.add(expression);
                                     continue;
                                 }
                                 default: {
-                                    this.jj_la1[43] = this.jj_gen;
+                                    this.jj_la1[45] = this.jj_gen;
                                     this.jj_consume_token(5);
                                     break Label_0198;
                                 }
                             }
                         }
                         break;
                     }
                     default: {
-                        this.jj_la1[44] = this.jj_gen;
+                        this.jj_la1[46] = this.jj_gen;
                         this.jj_consume_token(-1);
                         throw new ParseException();
                     }
                 }
             }
         }
         return expressions;
     }
     
     private final Expression StringSlicingExpression(final Expression expression) throws ParseException {
-        Token startSign = null;
-        Token start = null;
-        Token stopSign = null;
-        Token stop = null;
+        Integer startPos = null;
+        Integer stopPos = null;
         this.jj_consume_token(23);
         switch ((this.jj_ntk == -1) ? this.jj_ntk_f() : this.jj_ntk) {
             case 16:
             case 17:
             case 41: {
-                switch ((this.jj_ntk == -1) ? this.jj_ntk_f() : this.jj_ntk) {
-                    case 16:
-                    case 17: {
-                        startSign = this.Sign();
-                        break;
-                    }
-                    default: {
-                        this.jj_la1[45] = this.jj_gen;
-                        break;
-                    }
-                }
-                start = this.jj_consume_token(41);
+                startPos = Integer.valueOf(this.ColumnIndex());
                 break;
             }
             default: {
-                this.jj_la1[46] = this.jj_gen;
+                this.jj_la1[47] = this.jj_gen;
                 break;
             }
         }
         this.jj_consume_token(27);
         switch ((this.jj_ntk == -1) ? this.jj_ntk_f() : this.jj_ntk) {
             case 16:
             case 17:
             case 41: {
-                switch ((this.jj_ntk == -1) ? this.jj_ntk_f() : this.jj_ntk) {
-                    case 16:
-                    case 17: {
-                        stopSign = this.Sign();
-                        break;
-                    }
-                    default: {
-                        this.jj_la1[47] = this.jj_gen;
-                        break;
-                    }
-                }
-                stop = this.jj_consume_token(41);
+                stopPos = Integer.valueOf(this.ColumnIndex());
                 break;
             }
             default: {
                 this.jj_la1[48] = this.jj_gen;
                 break;
             }
         }
         this.jj_consume_token(24);
-        Integer startPos = null;
-        if (start != null) {
-            startPos = Integer.valueOf(PythonParserUtil.parseInt(startSign, start));
-        }
-        Integer stopPos = null;
-        if (stop != null) {
-            stopPos = Integer.valueOf(PythonParserUtil.parseInt(stopSign, stop));
-        }
         return translateStringSlice(expression, startPos, stopPos);
     }
     
     private final Expression NameInvocationExpression(final String dottedName) throws ParseException {
+        final Scope scope = this.ensureScope();
         final int dot = dottedName.indexOf(46);
         if (dot > -1) {
             return (Expression)this.encodeConstant(dottedName);
         }
         final FieldRef fieldRef = (FieldRef)this.variableMap.get(dottedName);
         if (fieldRef != null) {
             return (Expression)fieldRef;
         }
-        final Scope scope = this.ensureScope();
         final Feature feature = scope.getFeature(dottedName);
         return (Expression)feature.ref();
     }
     
     private final Expression ParenthesizedExpression() throws ParseException {
         this.jj_consume_token(4);
         final Expression expression = this.Expression();
@@ -1755,111 +1774,145 @@
             return true;
         }
         finally {
             this.jj_save(6, xla);
         }
     }
     
-    private boolean jj_3R_String_565_9_26() {
+    private boolean jj_3_5() {
+        return this.jj_3R_ArrayIndexingExpression_1166_9_20();
+    }
+    
+    private boolean jj_3R_ColumnIndex_598_10_31() {
+        return this.jj_3R_Sign_581_9_32();
+    }
+    
+    private boolean jj_3R_ColumnIndex_598_9_29() {
         final Token xsp = this.jj_scanpos;
-        if (this.jj_scan_token(44)) {
+        if (this.jj_3R_ColumnIndex_598_10_31()) {
             this.jj_scanpos = xsp;
-            if (this.jj_scan_token(51)) {
-                return true;
-            }
         }
-        return false;
+        return this.jj_scan_token(41);
+    }
+    
+    private boolean jj_3_1() {
+        return this.jj_scan_token(26) || this.jj_scan_token(43);
     }
     
     private boolean jj_3_2() {
         return this.jj_scan_token(4) || this.jj_scan_token(5);
     }
     
-    private boolean jj_3_1() {
-        return this.jj_scan_token(26) || this.jj_scan_token(43);
+    private boolean jj_3R_ArrayColumnIndex_611_86_28() {
+        return this.jj_3R_ColumnIndex_598_9_29();
+    }
+    
+    private boolean jj_3_3() {
+        return this.jj_scan_token(43) || this.jj_scan_token(15);
+    }
+    
+    private boolean jj_3R_ArrayColumnIndex_611_34_27() {
+        return this.jj_scan_token(23) || this.jj_3R_ColumnIndex_598_9_29() || this.jj_scan_token(24);
     }
     
-    private boolean jj_3R_Sign_581_9_24() {
+    private boolean jj_3_4() {
+        return this.jj_scan_token(39) || this.jj_scan_token(30);
+    }
+    
+    private boolean jj_3_7() {
+        return this.jj_scan_token(4) || this.jj_scan_token(5);
+    }
+    
+    private boolean jj_3R_Sign_581_9_32() {
         final Token xsp = this.jj_scanpos;
         if (this.jj_scan_token(16)) {
             this.jj_scanpos = xsp;
             if (this.jj_scan_token(17)) {
                 return true;
             }
         }
         return false;
     }
     
-    private boolean jj_3_4() {
-        return this.jj_scan_token(39) || this.jj_scan_token(30);
+    private boolean jj_3R_ColumnName_626_9_26() {
+        return this.jj_3R_String_565_9_30();
+    }
+    
+    private boolean jj_3R_ArrayColumnIndex_613_17_25() {
+        return this.jj_3R_ColumnIndex_598_9_29();
+    }
+    
+    private boolean jj_3_6() {
+        return this.jj_scan_token(23) || this.jj_3R_ArrayColumnIndex_610_9_21();
     }
     
-    private boolean jj_3R_ArrayIndexingExpression_1124_17_22() {
-        if (this.jj_scan_token(23)) {
+    private boolean jj_3R_ArrayColumnIndex_611_17_24() {
+        if (this.jj_scan_token(27)) {
+            return true;
+        }
+        if (this.jj_scan_token(25)) {
             return true;
         }
         final Token xsp = this.jj_scanpos;
-        if (this.jj_3R_ArrayIndexingExpression_1125_29_25()) {
+        if (this.jj_3R_ArrayColumnIndex_611_34_27()) {
             this.jj_scanpos = xsp;
+            if (this.jj_3R_ArrayColumnIndex_611_86_28()) {
+                return true;
+            }
         }
-        return this.jj_scan_token(41) || this.jj_scan_token(24);
-    }
-    
-    private boolean jj_3R_null_1124_39_21() {
-        return this.jj_3R_Sign_581_9_24();
-    }
-    
-    private boolean jj_3_3() {
-        return this.jj_scan_token(43) || this.jj_scan_token(15);
+        return false;
     }
     
-    private boolean jj_3_5() {
-        return this.jj_3R_ArrayIndexingExpression_1123_9_20();
+    private boolean jj_3R_ArrayIndexingExpression_1172_17_23() {
+        return this.jj_scan_token(23) || this.jj_3R_ColumnName_626_9_26() || this.jj_scan_token(24);
     }
     
-    private boolean jj_3R_ArrayIndexingExpression_1123_9_20() {
+    private boolean jj_3R_String_565_9_30() {
         final Token xsp = this.jj_scanpos;
-        if (this.jj_3R_ArrayIndexingExpression_1124_17_22()) {
+        if (this.jj_scan_token(44)) {
             this.jj_scanpos = xsp;
-            if (this.jj_3R_ArrayIndexingExpression_1133_17_23()) {
+            if (this.jj_scan_token(51)) {
                 return true;
             }
         }
         return false;
     }
     
-    private boolean jj_3R_ArrayIndexingExpression_1125_29_25() {
-        return this.jj_3R_Sign_581_9_24();
+    private boolean jj_3R_ArrayIndexingExpression_1167_17_22() {
+        return this.jj_scan_token(23) || this.jj_3R_ArrayColumnIndex_610_9_21() || this.jj_scan_token(24);
     }
     
-    private boolean jj_3_6() {
-        if (this.jj_scan_token(23)) {
-            return true;
-        }
+    private boolean jj_3R_ArrayColumnIndex_610_9_21() {
         final Token xsp = this.jj_scanpos;
-        if (this.jj_3R_null_1124_39_21()) {
+        if (this.jj_3R_ArrayColumnIndex_611_17_24()) {
             this.jj_scanpos = xsp;
+            if (this.jj_3R_ArrayColumnIndex_613_17_25()) {
+                return true;
+            }
         }
-        return this.jj_scan_token(41);
-    }
-    
-    private boolean jj_3R_ArrayIndexingExpression_1133_17_23() {
-        return this.jj_scan_token(23) || this.jj_3R_String_565_9_26() || this.jj_scan_token(24);
+        return false;
     }
     
-    private boolean jj_3_7() {
-        return this.jj_scan_token(4) || this.jj_scan_token(5);
+    private boolean jj_3R_ArrayIndexingExpression_1166_9_20() {
+        final Token xsp = this.jj_scanpos;
+        if (this.jj_3R_ArrayIndexingExpression_1167_17_22()) {
+            this.jj_scanpos = xsp;
+            if (this.jj_3R_ArrayIndexingExpression_1172_17_23()) {
+                return true;
+            }
+        }
+        return false;
     }
     
     private static void jj_la1_init_0() {
-        ExpressionTranslator.jj_la1_0 = new int[] { 0, 196608, 8, 8, 33554432, 16, 8, -536674024, -536674024, -536674024, -536674032, 268435456, -536674032, 0, 0, 33554432, 0, 0, 64, 128, 256, 32256, 32256, 256, 196608, 196608, 1835008, 1835008, -536674288, 4194304, 75497472, 75497472, 75497472, 75497472, 75497472, 75497472, 8388608, 16, 75497472, 75497472, -536870896, 196608, 8388608, 33554432, 16, 196608, 196608, 196608, 196608, -536870912, 33554432 };
+        ExpressionTranslator.jj_la1_0 = new int[] { 0, 196608, 196608, 8585216, 134414336, 8, 8, 33554432, 16, 8, -536674024, -536674024, -536674024, -536674032, 268435456, -536674032, 0, 0, 33554432, 0, 0, 64, 128, 256, 32256, 32256, 256, 196608, 196608, 1835008, 1835008, -536674288, 4194304, 75497472, 75497472, 75497472, 75497472, 75497472, 75497472, 8388608, 16, 75497472, 75497472, -536870896, 8388608, 33554432, 16, 196608, 196608, -536870912, 33554432 };
     }
     
     private static void jj_la1_init_1() {
-        ExpressionTranslator.jj_la1_1 = new int[] { 528384, 0, 0, 0, 0, 0, 0, 532256, 532272, 532272, 532272, 0, 532256, 4, 8, 0, 1, 16, 0, 0, 0, 0, 0, 192, 0, 0, 0, 0, 531968, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 531968, 0, 0, 0, 0, 0, 512, 0, 512, 529920, 0 };
+        ExpressionTranslator.jj_la1_1 = new int[] { 528384, 0, 0, 512, 512, 0, 0, 0, 0, 0, 532256, 532272, 532272, 532272, 0, 532256, 4, 8, 0, 1, 16, 0, 0, 0, 0, 0, 192, 0, 0, 0, 0, 531968, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 531968, 0, 0, 0, 512, 512, 529920, 0 };
     }
     
     public ExpressionTranslator(final Provider stream) {
         this.indents = new ArrayDeque<String>();
         this.variableMap = new LinkedHashMap<String, FieldRef>();
         this.jj_la1 = new int[51];
         this.jj_2_rtns = new ExpressionTranslator.JJCalls[7];
```

#### org/jpmml/python/PredicateTranslator$JJCalls.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 8d6fab4e59fdc113d18b81d68bad368a9952149cea537b2901bd0e5b9c4504b7
+  SHA-256 checksum 5f963ac1dcfd0dbd24de3ab9750acf71e09aedf95825db6a93d51772304ab28f
   Compiled from "PredicateTranslator.java"
 final class org.jpmml.python.PredicateTranslator$JJCalls
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #2                          // org/jpmml/python/PredicateTranslator$JJCalls
   super_class: #3                         // java/lang/Object
@@ -55,15 +55,15 @@
     flags: (0x0000)
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #1                  // Method java/lang/Object."<init>":()V
          4: return
       LineNumberTable:
-        line 1020: 0
+        line 1112: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lorg/jpmml/python/PredicateTranslator$JJCalls;
 }
 SourceFile: "PredicateTranslator.java"
 InnerClasses:
   static final #10= #2 of #22;            // JJCalls=class org/jpmml/python/PredicateTranslator$JJCalls of class org/jpmml/python/PredicateTranslator
```

#### org/jpmml/python/ExpressionTranslator$JJCalls.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 9c9019a9c787ec5721be6f905bd40e19493632cf3f66542dfd8b1e53c9cfe469
+  SHA-256 checksum c5088c883d346961d040dbec6e7d6a77f41a696b395c5376a7e373c4acadbc65
   Compiled from "ExpressionTranslator.java"
 final class org.jpmml.python.ExpressionTranslator$JJCalls
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #2                          // org/jpmml/python/ExpressionTranslator$JJCalls
   super_class: #3                         // java/lang/Object
@@ -55,15 +55,15 @@
     flags: (0x0000)
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #1                  // Method java/lang/Object."<init>":()V
          4: return
       LineNumberTable:
-        line 2063: 0
+        line 2120: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lorg/jpmml/python/ExpressionTranslator$JJCalls;
 }
 SourceFile: "ExpressionTranslator.java"
 InnerClasses:
   static final #10= #2 of #22;            // JJCalls=class org/jpmml/python/ExpressionTranslator$JJCalls of class org/jpmml/python/ExpressionTranslator
```

#### org/jpmml/python/PredicateTranslator.class

##### procyon -ec {}

```diff
@@ -246,14 +246,80 @@
                 this.jj_consume_token(-1);
                 throw new ParseException();
             }
         }
         return token;
     }
     
+    private final int ColumnIndex() throws ParseException {
+        Token sign = null;
+        switch ((this.jj_ntk == -1) ? this.jj_ntk_f() : this.jj_ntk) {
+            case 16:
+            case 17: {
+                sign = this.Sign();
+                break;
+            }
+            default: {
+                this.jj_la1[2] = this.jj_gen;
+                break;
+            }
+        }
+        final Token column = this.jj_consume_token(41);
+        return PythonParserUtil.parseInt(sign, column);
+    }
+    
+    private final int ArrayColumnIndex() throws ParseException {
+        int columnIndex = 0;
+        Label_0222: {
+            switch ((this.jj_ntk == -1) ? this.jj_ntk_f() : this.jj_ntk) {
+                case 27: {
+                    this.jj_consume_token(27);
+                    this.jj_consume_token(25);
+                    switch ((this.jj_ntk == -1) ? this.jj_ntk_f() : this.jj_ntk) {
+                        case 23: {
+                            this.jj_consume_token(23);
+                            columnIndex = this.ColumnIndex();
+                            this.jj_consume_token(24);
+                            break Label_0222;
+                        }
+                        case 16:
+                        case 17:
+                        case 41: {
+                            columnIndex = this.ColumnIndex();
+                            break Label_0222;
+                        }
+                        default: {
+                            this.jj_la1[3] = this.jj_gen;
+                            this.jj_consume_token(-1);
+                            throw new ParseException();
+                        }
+                    }
+                    break;
+                }
+                case 16:
+                case 17:
+                case 41: {
+                    columnIndex = this.ColumnIndex();
+                    break;
+                }
+                default: {
+                    this.jj_la1[4] = this.jj_gen;
+                    this.jj_consume_token(-1);
+                    throw new ParseException();
+                }
+            }
+        }
+        return columnIndex;
+    }
+    
+    private final String ColumnName() throws ParseException {
+        final Token column = this.String();
+        return PythonParserUtil.parseString(column);
+    }
+    
     private final String DottedName() throws ParseException {
         final StringBuilder sb = new StringBuilder();
         Token name = this.jj_consume_token(43);
         sb.append(name.image);
         while (this.jj_2_1(Integer.MAX_VALUE)) {
             this.jj_consume_token(26);
             name = this.jj_consume_token(43);
@@ -285,15 +351,15 @@
                 case 6: {
                     this.jj_consume_token(6);
                     final Predicate right = this.LogicalAndExpression();
                     left = (Predicate)createCompoundPredicate(left, CompoundPredicate.BooleanOperator.OR, right);
                     continue;
                 }
                 default: {
-                    this.jj_la1[2] = this.jj_gen;
+                    this.jj_la1[5] = this.jj_gen;
                     return left;
                 }
             }
         }
     }
     
     private final Predicate LogicalAndExpression() throws ParseException {
@@ -303,15 +369,15 @@
                 case 7: {
                     this.jj_consume_token(7);
                     final Predicate right = this.ComparisonExpression();
                     left = (Predicate)createCompoundPredicate(left, CompoundPredicate.BooleanOperator.AND, right);
                     continue;
                 }
                 default: {
-                    this.jj_la1[3] = this.jj_gen;
+                    this.jj_la1[6] = this.jj_gen;
                     return left;
                 }
             }
         }
     }
     
     private final Predicate ComparisonExpression() throws ParseException {
@@ -372,25 +438,25 @@
                             break;
                         }
                         case 14: {
                             operator = this.jj_consume_token(14);
                             break;
                         }
                         default: {
-                            this.jj_la1[4] = this.jj_gen;
+                            this.jj_la1[7] = this.jj_gen;
                             this.jj_consume_token(-1);
                             throw new ParseException();
                         }
                     }
                     final Object right = this.UnaryExpression();
                     left = createSimplePredicate(left, translateRelationalOperator(operator), right);
                     break;
                 }
                 default: {
-                    this.jj_la1[5] = this.jj_gen;
+                    this.jj_la1[8] = this.jj_gen;
                     left = asPredicate(left);
                     break;
                 }
             }
         }
         return (Predicate)left;
     }
@@ -413,15 +479,15 @@
             case 43:
             case 44:
             case 51: {
                 result = this.PrimaryExpression();
                 break;
             }
             default: {
-                this.jj_la1[6] = this.jj_gen;
+                this.jj_la1[9] = this.jj_gen;
                 this.jj_consume_token(-1);
                 throw new ParseException();
             }
         }
         if (sign != null && sign.kind == 17) {
             result = ValueUtil.toNegative(asValue(result));
         }
@@ -440,15 +506,15 @@
                             break Label_0223;
                         }
                         case 4: {
                             result = this.FunctionInvocationExpression(dottedName);
                             break Label_0223;
                         }
                         default: {
-                            this.jj_la1[7] = this.jj_gen;
+                            this.jj_la1[10] = this.jj_gen;
                             result = this.NameInvocationExpression(dottedName);
                             break Label_0223;
                         }
                     }
                     break;
                 }
                 case 4: {
@@ -461,58 +527,43 @@
                 case 42:
                 case 44:
                 case 51: {
                     result = this.LiteralExpression();
                     break;
                 }
                 default: {
-                    this.jj_la1[8] = this.jj_gen;
+                    this.jj_la1[11] = this.jj_gen;
                     this.jj_consume_token(-1);
                     throw new ParseException();
                 }
             }
         }
         return result;
     }
     
     private final Feature ArrayIndexingExpression(final String dottedName) throws ParseException {
-        Token sign = null;
+        final Scope scope = this.ensureScope();
         Feature feature = null;
         if (this.jj_2_3(Integer.MAX_VALUE)) {
             this.jj_consume_token(23);
-            switch ((this.jj_ntk == -1) ? this.jj_ntk_f() : this.jj_ntk) {
-                case 16:
-                case 17: {
-                    sign = this.Sign();
-                    break;
-                }
-                default: {
-                    this.jj_la1[9] = this.jj_gen;
-                    break;
-                }
-            }
-            final Token column = this.jj_consume_token(41);
+            final int colIndex = this.ArrayColumnIndex();
             this.jj_consume_token(24);
-            final Scope scope = this.ensureScope();
-            final int colIndex = PythonParserUtil.parseInt(sign, column);
             feature = scope.getFeature(dottedName, colIndex);
         }
         else {
             switch ((this.jj_ntk == -1) ? this.jj_ntk_f() : this.jj_ntk) {
                 case 23: {
                     this.jj_consume_token(23);
-                    final Token column = this.String();
+                    final String colName = this.ColumnName();
                     this.jj_consume_token(24);
-                    final Scope scope = this.ensureScope();
-                    final String colName = PythonParserUtil.parseString(column);
                     feature = scope.getFeature(dottedName, colName);
                     break;
                 }
                 default: {
-                    this.jj_la1[10] = this.jj_gen;
+                    this.jj_la1[12] = this.jj_gen;
                     this.jj_consume_token(-1);
                     throw new ParseException();
                 }
             }
         }
         return feature;
     }
@@ -540,24 +591,24 @@
                                 case 25: {
                                     this.jj_consume_token(25);
                                     argument = this.PrimaryExpression();
                                     arguments.add(asArgument(argument));
                                     continue;
                                 }
                                 default: {
-                                    this.jj_la1[11] = this.jj_gen;
+                                    this.jj_la1[13] = this.jj_gen;
                                     this.jj_consume_token(5);
                                     break Label_0205;
                                 }
                             }
                         }
                         break;
                     }
                     default: {
-                        this.jj_la1[12] = this.jj_gen;
+                        this.jj_la1[14] = this.jj_gen;
                         this.jj_consume_token(-1);
                         throw new ParseException();
                     }
                 }
             }
         }
         return arguments;
@@ -597,15 +648,15 @@
             }
             case 44:
             case 51: {
                 value = this.String();
                 break;
             }
             default: {
-                this.jj_la1[13] = this.jj_gen;
+                this.jj_la1[15] = this.jj_gen;
                 this.jj_consume_token(-1);
                 throw new ParseException();
             }
         }
         return PythonParserUtil.parseValue(value);
     }
     
@@ -619,15 +670,15 @@
                 case 25: {
                     this.jj_consume_token(25);
                     predicate = this.UnaryExpression();
                     values.add(asValue(predicate));
                     continue;
                 }
                 default: {
-                    this.jj_la1[14] = this.jj_gen;
+                    this.jj_la1[16] = this.jj_gen;
                     this.jj_consume_token(24);
                     return createArray(values);
                 }
             }
         }
     }
     
@@ -691,74 +742,115 @@
             return true;
         }
         finally {
             this.jj_save(3, xla);
         }
     }
     
-    private boolean jj_3_1() {
-        return this.jj_scan_token(26) || this.jj_scan_token(43);
+    private boolean jj_3_4() {
+        return this.jj_scan_token(4) || this.jj_scan_token(5);
     }
     
-    private boolean jj_3_2() {
-        return this.jj_scan_token(39) || this.jj_scan_token(30);
+    private boolean jj_3R_ArrayColumnIndex_467_34_9() {
+        return this.jj_scan_token(23) || this.jj_3R_ColumnIndex_454_9_11() || this.jj_scan_token(24);
     }
     
-    private boolean jj_3R_null_607_39_6() {
-        return this.jj_3R_Sign_437_9_7();
+    private boolean jj_3R_ArrayColumnIndex_466_9_6() {
+        final Token xsp = this.jj_scanpos;
+        if (this.jj_3R_ArrayColumnIndex_467_17_7()) {
+            this.jj_scanpos = xsp;
+            if (this.jj_3R_ArrayColumnIndex_469_17_8()) {
+                return true;
+            }
+        }
+        return false;
     }
     
     private boolean jj_3_3() {
-        if (this.jj_scan_token(23)) {
-            return true;
+        return this.jj_scan_token(23) || this.jj_3R_ArrayColumnIndex_466_9_6();
+    }
+    
+    private boolean jj_3R_Sign_437_9_13() {
+        final Token xsp = this.jj_scanpos;
+        if (this.jj_scan_token(16)) {
+            this.jj_scanpos = xsp;
+            if (this.jj_scan_token(17)) {
+                return true;
+            }
         }
+        return false;
+    }
+    
+    private boolean jj_3_1() {
+        return this.jj_scan_token(26) || this.jj_scan_token(43);
+    }
+    
+    private boolean jj_3R_ColumnIndex_454_10_12() {
+        return this.jj_3R_Sign_437_9_13();
+    }
+    
+    private boolean jj_3R_ColumnIndex_454_9_11() {
         final Token xsp = this.jj_scanpos;
-        if (this.jj_3R_null_607_39_6()) {
+        if (this.jj_3R_ColumnIndex_454_10_12()) {
             this.jj_scanpos = xsp;
         }
         return this.jj_scan_token(41);
     }
     
-    private boolean jj_3R_Sign_437_9_7() {
+    private boolean jj_3R_ArrayColumnIndex_469_17_8() {
+        return this.jj_3R_ColumnIndex_454_9_11();
+    }
+    
+    private boolean jj_3_2() {
+        return this.jj_scan_token(39) || this.jj_scan_token(30);
+    }
+    
+    private boolean jj_3R_ArrayColumnIndex_467_86_10() {
+        return this.jj_3R_ColumnIndex_454_9_11();
+    }
+    
+    private boolean jj_3R_ArrayColumnIndex_467_17_7() {
+        if (this.jj_scan_token(27)) {
+            return true;
+        }
+        if (this.jj_scan_token(25)) {
+            return true;
+        }
         final Token xsp = this.jj_scanpos;
-        if (this.jj_scan_token(16)) {
+        if (this.jj_3R_ArrayColumnIndex_467_34_9()) {
             this.jj_scanpos = xsp;
-            if (this.jj_scan_token(17)) {
+            if (this.jj_3R_ArrayColumnIndex_467_86_10()) {
                 return true;
             }
         }
         return false;
     }
     
-    private boolean jj_3_4() {
-        return this.jj_scan_token(4) || this.jj_scan_token(5);
-    }
-    
     private static void jj_la1_init_0() {
-        PredicateTranslator.jj_la1_0 = new int[] { 0, 196608, 64, 128, 32256, 32512, -1610416112, 8388624, -1610612720, 196608, 8388608, 33554432, 16, -1610612736, 33554432 };
+        PredicateTranslator.jj_la1_0 = new int[] { 0, 196608, 196608, 8585216, 134414336, 64, 128, 32256, 32512, -1610416112, 8388624, -1610612720, 8388608, 33554432, 16, -1610612736, 33554432 };
     }
     
     private static void jj_la1_init_1() {
-        PredicateTranslator.jj_la1_1 = new int[] { 528384, 0, 0, 0, 0, 192, 531968, 0, 531968, 0, 0, 0, 0, 529920, 0 };
+        PredicateTranslator.jj_la1_1 = new int[] { 528384, 0, 0, 512, 512, 0, 0, 0, 192, 531968, 0, 531968, 0, 0, 0, 529920, 0 };
     }
     
     public PredicateTranslator(final Provider stream) {
-        this.jj_la1 = new int[15];
+        this.jj_la1 = new int[17];
         this.jj_2_rtns = new PredicateTranslator.JJCalls[4];
         this.jj_rescan = false;
         this.jj_gc = 0;
         this.jj_expentries = new ArrayList<int[]>();
         this.jj_kind = -1;
         this.jj_lasttokens = new int[100];
         this.jj_input_stream = new SimpleCharStream(stream, 1, 1);
         this.token_source = new PythonParserTokenManager(this.jj_input_stream);
         this.token = new Token();
         this.jj_ntk = -1;
         this.jj_gen = 0;
-        for (int i = 0; i < 15; ++i) {
+        for (int i = 0; i < 17; ++i) {
             this.jj_la1[i] = -1;
         }
         for (int i = 0; i < this.jj_2_rtns.length; ++i) {
             this.jj_2_rtns[i] = new PredicateTranslator.JJCalls();
         }
     }
     
@@ -780,48 +872,48 @@
         if (this.token_source == null) {
             this.token_source = new PythonParserTokenManager(this.jj_input_stream);
         }
         this.token_source.ReInit(this.jj_input_stream);
         this.token = new Token();
         this.jj_ntk = -1;
         this.jj_gen = 0;
-        for (int i = 0; i < 15; ++i) {
+        for (int i = 0; i < 17; ++i) {
             this.jj_la1[i] = -1;
         }
         for (int i = 0; i < this.jj_2_rtns.length; ++i) {
             this.jj_2_rtns[i] = new PredicateTranslator.JJCalls();
         }
     }
     
     public PredicateTranslator(final PythonParserTokenManager tm) {
-        this.jj_la1 = new int[15];
+        this.jj_la1 = new int[17];
         this.jj_2_rtns = new PredicateTranslator.JJCalls[4];
         this.jj_rescan = false;
         this.jj_gc = 0;
         this.jj_expentries = new ArrayList<int[]>();
         this.jj_kind = -1;
         this.jj_lasttokens = new int[100];
         this.token_source = tm;
         this.token = new Token();
         this.jj_ntk = -1;
         this.jj_gen = 0;
-        for (int i = 0; i < 15; ++i) {
+        for (int i = 0; i < 17; ++i) {
             this.jj_la1[i] = -1;
         }
         for (int i = 0; i < this.jj_2_rtns.length; ++i) {
             this.jj_2_rtns[i] = new PredicateTranslator.JJCalls();
         }
     }
     
     public void ReInit(final PythonParserTokenManager tm) {
         this.token_source = tm;
         this.token = new Token();
         this.jj_ntk = -1;
         this.jj_gen = 0;
-        for (int i = 0; i < 15; ++i) {
+        for (int i = 0; i < 17; ++i) {
             this.jj_la1[i] = -1;
         }
         for (int i = 0; i < this.jj_2_rtns.length; ++i) {
             this.jj_2_rtns[i] = new PredicateTranslator.JJCalls();
         }
     }
     
@@ -974,15 +1066,15 @@
     public ParseException generateParseException() {
         this.jj_expentries.clear();
         final boolean[] la1tokens = new boolean[52];
         if (this.jj_kind >= 0) {
             la1tokens[this.jj_kind] = true;
             this.jj_kind = -1;
         }
-        for (int i = 0; i < 15; ++i) {
+        for (int i = 0; i < 17; ++i) {
             if (this.jj_la1[i] == this.jj_gen) {
                 for (int j = 0; j < 32; ++j) {
                     if ((PredicateTranslator.jj_la1_0[i] & 1 << j) != 0x0) {
                         la1tokens[j] = true;
                     }
                     if ((PredicateTranslator.jj_la1_1[i] & 1 << j) != 0x0) {
                         la1tokens[32 + j] = true;
```

#### META-INF/maven/org.jpmml/pmml-python/pom.xml

##### META-INF/maven/org.jpmml/pmml-python/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-python</artifactId>
-    <version>1.1.17</version>
+    <version>1.1.18</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-python</artifactId>
   <packaging>jar</packaging>
   <name>JPMML Python converter</name>
   <description>JPMML Python to PMML converter</description>
   <licenses>
@@ -137,14 +137,14 @@
             </configuration>
           </execution>
         </executions>
         <dependencies>
           <dependency>
             <groupId>net.java.dev.javacc</groupId>
             <artifactId>javacc</artifactId>
-            <version>7.0.12</version>
+            <version>7.0.13</version>
           </dependency>
         </dependencies>
       </plugin>
     </plugins>
   </build>
 </project>
```

#### META-INF/maven/org.jpmml/pmml-python/pom.properties

```diff
@@ -1,3 +1,3 @@
 artifactId=pmml-python
 groupId=org.jpmml
-version=1.1.17
+version=1.1.18
```

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.41.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.42.jar`

 * *Files 26% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 6418 bytes, number of entries: 15
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Oct-23 22:44 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn2pmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 sklearn2pmml/statsmodels/
--rw-rw-r--  2.0 unx      152 b- defN 23-Oct-23 22:44 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx     1190 b- defN 23-Oct-23 22:44 sklearn2pmml/statsmodels/StatsModelsOrdinalClassifier.class
--rw-rw-r--  2.0 unx     1744 b- defN 23-Oct-23 22:44 sklearn2pmml/statsmodels/StatsModelsClassifier.class
--rw-rw-r--  2.0 unx      180 b- defN 23-Oct-23 22:44 sklearn2pmml/statsmodels/HasResults.class
--rw-rw-r--  2.0 unx     2352 b- defN 23-Oct-23 22:44 sklearn2pmml/statsmodels/StatsModelsUtil.class
--rw-rw-r--  2.0 unx     1740 b- defN 23-Oct-23 22:44 sklearn2pmml/statsmodels/StatsModelsRegressor.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Oct-23 22:44 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Oct-23 22:44 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Oct-23 22:44 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/
--rw-rw-r--  2.0 unx     1331 b- defN 23-Oct-23 22:44 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.xml
--rw-rw-r--  2.0 unx      120 b- defN 23-Oct-23 22:44 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.properties
-15 files, 8939 bytes uncompressed, 4138 bytes compressed:  53.7%
+Zip file size: 6416 bytes, number of entries: 15
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Dec-04 22:17 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn2pmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 sklearn2pmml/statsmodels/
+-rw-rw-r--  2.0 unx      152 b- defN 23-Dec-04 22:17 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx     1190 b- defN 23-Dec-04 22:17 sklearn2pmml/statsmodels/StatsModelsOrdinalClassifier.class
+-rw-rw-r--  2.0 unx     1744 b- defN 23-Dec-04 22:17 sklearn2pmml/statsmodels/StatsModelsClassifier.class
+-rw-rw-r--  2.0 unx      180 b- defN 23-Dec-04 22:17 sklearn2pmml/statsmodels/HasResults.class
+-rw-rw-r--  2.0 unx     2352 b- defN 23-Dec-04 22:17 sklearn2pmml/statsmodels/StatsModelsUtil.class
+-rw-rw-r--  2.0 unx     1740 b- defN 23-Dec-04 22:17 sklearn2pmml/statsmodels/StatsModelsRegressor.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Dec-04 22:17 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Dec-04 22:17 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Dec-04 22:17 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/
+-rw-rw-r--  2.0 unx     1331 b- defN 23-Dec-04 22:16 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.xml
+-rw-rw-r--  2.0 unx      119 b- defN 23-Dec-04 22:17 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.properties
+15 files, 8938 bytes uncompressed, 4136 bytes compressed:  53.7%
```

#### META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.41</version>
+    <version>1.7.42</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-statsmodels</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn StatsModels converter</name>
   <description>JPMML Scikit-Learn StatsModels to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Mon Oct 23 22:44:50 EEST 2023
-version=1.7.41
+#Mon Dec 04 22:17:24 EET 2023
+version=1.7.42
 groupId=org.jpmml
 artifactId=pmml-sklearn-statsmodels
```

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/serpent-1.40.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/serpent-1.40.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/jakarta.activation-2.0.1.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/jakarta.activation-2.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/pmml-statsmodels-1.0.5.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/pmml-statsmodels-1.0.5.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/pickle-1.4.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/pickle-1.5.jar`

 * *Files 16% similar despite different names*

#### zipinfo {}

```diff
@@ -1,41 +1,42 @@
-Zip file size: 54294 bytes, number of entries: 39
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 21:16 META-INF/
--rw-r--r--  2.0 unx      129 b- defN 23-May-24 21:16 META-INF/MANIFEST.MF
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 21:16 net/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 21:16 net/razorvine/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 21:16 net/razorvine/pickle/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 21:16 net/razorvine/pickle/objects/
--rw-r--r--  2.0 unx      655 b- defN 23-May-24 21:16 net/razorvine/pickle/InvalidOpcodeException.class
--rw-r--r--  2.0 unx     1837 b- defN 23-May-24 21:16 net/razorvine/pickle/UnpickleStack.class
--rw-r--r--  2.0 unx      512 b- defN 23-May-24 21:16 net/razorvine/pickle/Pickler$Memo.class
--rw-r--r--  2.0 unx    21134 b- defN 23-May-24 21:16 net/razorvine/pickle/Unpickler.class
--rw-r--r--  2.0 unx     1209 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/Tzinfo.class
--rw-r--r--  2.0 unx     3685 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/TimeZoneConstructor.class
--rw-r--r--  2.0 unx     5930 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/DateTimeConstructor.class
--rw-r--r--  2.0 unx     1411 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/OperatorAttrGetterForCalendarTz$AttrGetterForTz.class
--rw-r--r--  2.0 unx     1835 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/ClassDict.class
--rw-r--r--  2.0 unx     1327 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/ClassDictConstructor.class
--rw-r--r--  2.0 unx     1550 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/Reconstructor.class
--rw-r--r--  2.0 unx     1793 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/Time.class
--rw-r--r--  2.0 unx      759 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/SetConstructor.class
--rw-r--r--  2.0 unx     2497 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/ExceptionConstructor.class
--rw-r--r--  2.0 unx     1966 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/ByteArrayConstructor.class
--rw-r--r--  2.0 unx     1285 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/OperatorAttrGetterForCalendarTz.class
--rw-r--r--  2.0 unx     1349 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/OperatorAttrGetterForCalendarTz$CalendarLocalizer.class
--rw-r--r--  2.0 unx     1980 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/AnyClassConstructor.class
--rw-r--r--  2.0 unx     2727 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/ComplexNumber.class
--rw-r--r--  2.0 unx     1966 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/TimeDelta.class
--rw-r--r--  2.0 unx     8673 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/ArrayConstructor.class
--rw-r--r--  2.0 unx      624 b- defN 23-May-24 21:16 net/razorvine/pickle/PickleException.class
--rw-r--r--  2.0 unx     8302 b- defN 23-May-24 21:16 net/razorvine/pickle/PickleUtils.class
--rw-r--r--  2.0 unx      265 b- defN 23-May-24 21:16 net/razorvine/pickle/IObjectConstructor.class
--rw-r--r--  2.0 unx     2262 b- defN 23-May-24 21:16 net/razorvine/pickle/PythonException.class
--rw-r--r--  2.0 unx     2339 b- defN 23-May-24 21:16 net/razorvine/pickle/Opcodes.class
--rw-r--r--  2.0 unx      315 b- defN 23-May-24 21:16 net/razorvine/pickle/IObjectPickler.class
--rw-r--r--  2.0 unx    17356 b- defN 23-May-24 21:16 net/razorvine/pickle/Pickler.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-May-24 21:16 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-May-24 21:16 META-INF/maven/net.razorvine/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-May-24 21:16 META-INF/maven/net.razorvine/pickle/
--rw-r--r--  2.0 unx     2701 b- defN 23-May-24 21:16 META-INF/maven/net.razorvine/pickle/pom.xml
--rw-r--r--  2.0 unx      103 b- defN 23-May-24 21:16 META-INF/maven/net.razorvine/pickle/pom.properties
-39 files, 100476 bytes uncompressed, 48042 bytes compressed:  52.2%
+Zip file size: 54836 bytes, number of entries: 40
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-19 15:16 META-INF/
+-rw-r--r--  2.0 unx      129 b- defN 23-Nov-19 15:16 META-INF/MANIFEST.MF
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-19 15:16 net/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-19 15:16 net/razorvine/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-19 15:16 net/razorvine/pickle/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-19 15:16 net/razorvine/pickle/objects/
+-rw-r--r--  2.0 unx      655 b- defN 23-Nov-19 15:16 net/razorvine/pickle/InvalidOpcodeException.class
+-rw-r--r--  2.0 unx     1837 b- defN 23-Nov-19 15:16 net/razorvine/pickle/UnpickleStack.class
+-rw-r--r--  2.0 unx      512 b- defN 23-Nov-19 15:16 net/razorvine/pickle/Pickler$Memo.class
+-rw-r--r--  2.0 unx    20989 b- defN 23-Nov-19 15:16 net/razorvine/pickle/Unpickler.class
+-rw-r--r--  2.0 unx     1209 b- defN 23-Nov-19 15:16 net/razorvine/pickle/objects/Tzinfo.class
+-rw-r--r--  2.0 unx     3611 b- defN 23-Nov-19 15:16 net/razorvine/pickle/objects/TimeZoneConstructor.class
+-rw-r--r--  2.0 unx     5872 b- defN 23-Nov-19 15:16 net/razorvine/pickle/objects/DateTimeConstructor.class
+-rw-r--r--  2.0 unx     1170 b- defN 23-Nov-19 15:16 net/razorvine/pickle/objects/OperatorAttrGetterForCalendarTz$AttrGetterForTz.class
+-rw-r--r--  2.0 unx     1374 b- defN 23-Nov-19 15:16 net/razorvine/pickle/objects/ClassDict.class
+-rw-r--r--  2.0 unx     1327 b- defN 23-Nov-19 15:16 net/razorvine/pickle/objects/ClassDictConstructor.class
+-rw-r--r--  2.0 unx     1550 b- defN 23-Nov-19 15:16 net/razorvine/pickle/objects/Reconstructor.class
+-rw-r--r--  2.0 unx     1793 b- defN 23-Nov-19 15:16 net/razorvine/pickle/objects/Time.class
+-rw-r--r--  2.0 unx      759 b- defN 23-Nov-19 15:16 net/razorvine/pickle/objects/SetConstructor.class
+-rw-r--r--  2.0 unx     2494 b- defN 23-Nov-19 15:16 net/razorvine/pickle/objects/ExceptionConstructor.class
+-rw-r--r--  2.0 unx     1966 b- defN 23-Nov-19 15:16 net/razorvine/pickle/objects/ByteArrayConstructor.class
+-rw-r--r--  2.0 unx     1211 b- defN 23-Nov-19 15:16 net/razorvine/pickle/objects/OperatorAttrGetterForCalendarTz.class
+-rw-r--r--  2.0 unx     1154 b- defN 23-Nov-19 15:16 net/razorvine/pickle/objects/OperatorAttrGetterForCalendarTz$CalendarLocalizer.class
+-rw-r--r--  2.0 unx     1980 b- defN 23-Nov-19 15:16 net/razorvine/pickle/objects/AnyClassConstructor.class
+-rw-r--r--  2.0 unx     2731 b- defN 23-Nov-19 15:16 net/razorvine/pickle/objects/ComplexNumber.class
+-rw-r--r--  2.0 unx     1966 b- defN 23-Nov-19 15:16 net/razorvine/pickle/objects/TimeDelta.class
+-rw-r--r--  2.0 unx     8673 b- defN 23-Nov-19 15:16 net/razorvine/pickle/objects/ArrayConstructor.class
+-rw-r--r--  2.0 unx      624 b- defN 23-Nov-19 15:16 net/razorvine/pickle/PickleException.class
+-rw-r--r--  2.0 unx      332 b- defN 23-Nov-19 15:16 net/razorvine/pickle/IObjectDeconstructor.class
+-rw-r--r--  2.0 unx     8302 b- defN 23-Nov-19 15:16 net/razorvine/pickle/PickleUtils.class
+-rw-r--r--  2.0 unx      265 b- defN 23-Nov-19 15:16 net/razorvine/pickle/IObjectConstructor.class
+-rw-r--r--  2.0 unx     2262 b- defN 23-Nov-19 15:16 net/razorvine/pickle/PythonException.class
+-rw-r--r--  2.0 unx     2339 b- defN 23-Nov-19 15:16 net/razorvine/pickle/Opcodes.class
+-rw-r--r--  2.0 unx      315 b- defN 23-Nov-19 15:16 net/razorvine/pickle/IObjectPickler.class
+-rw-r--r--  2.0 unx    18982 b- defN 23-Nov-19 15:16 net/razorvine/pickle/Pickler.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Nov-19 15:16 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Nov-19 15:16 META-INF/maven/net.razorvine/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Nov-19 15:16 META-INF/maven/net.razorvine/pickle/
+-rw-r--r--  2.0 unx     2906 b- defN 23-Nov-19 15:16 META-INF/maven/net.razorvine/pickle/pom.xml
+-rw-r--r--  2.0 unx      102 b- defN 23-Nov-19 15:16 META-INF/maven/net.razorvine/pickle/pom.properties
+40 files, 101391 bytes uncompressed, 48414 bytes compressed:  52.3%
```

#### zipnote «TEMP»/diffoscope_wqp9k9w__/tmp3p8pkogl_.zip

```diff
@@ -78,14 +78,17 @@
 
 Filename: net/razorvine/pickle/objects/ArrayConstructor.class
 Comment: 
 
 Filename: net/razorvine/pickle/PickleException.class
 Comment: 
 
+Filename: net/razorvine/pickle/IObjectDeconstructor.class
+Comment: 
+
 Filename: net/razorvine/pickle/PickleUtils.class
 Comment: 
 
 Filename: net/razorvine/pickle/IObjectConstructor.class
 Comment: 
 
 Filename: net/razorvine/pickle/PythonException.class
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,6 @@
 Manifest-Version: 1.0
 Archiver-Version: Plexus Archiver
 Created-By: Apache Maven 3.8.7
 Built-By: irmen
-Build-Jdk: 11.0.19
+Build-Jdk: 11.0.21
```

#### net/razorvine/pickle/UnpickleStack.class

##### procyon -ec {}

```diff
@@ -5,16 +5,16 @@
 import java.util.List;
 import java.util.ArrayList;
 import java.io.Serializable;
 
 public class UnpickleStack implements Serializable
 {
     private static final long serialVersionUID = 5032718425413805422L;
-    private ArrayList<Object> stack;
-    protected Object MARKER;
+    private final ArrayList<Object> stack;
+    protected final Object MARKER;
     
     public UnpickleStack() {
         this.stack = new ArrayList<Object>();
         this.MARKER = new Object();
     }
     
     public void add(final Object o) {
```

#### net/razorvine/pickle/Pickler$Memo.class

##### procyon -ec {}

```diff
@@ -1,13 +1,13 @@
 
 package net.razorvine.pickle;
 
 protected static class Memo
 {
-    public Object obj;
-    public int index;
+    public final Object obj;
+    public final int index;
     
     public Memo(final Object obj, final int index) {
         this.obj = obj;
         this.index = index;
     }
 }
```

#### net/razorvine/pickle/Unpickler.class

##### procyon -ec {}

```diff
@@ -13,14 +13,15 @@
 import net.razorvine.pickle.objects.ComplexNumber;
 import net.razorvine.pickle.objects.ClassDictConstructor;
 import net.razorvine.pickle.objects.ExceptionConstructor;
 import java.util.Collection;
 import java.util.HashSet;
 import java.util.ArrayList;
 import java.util.List;
+import java.nio.charset.StandardCharsets;
 import java.math.BigInteger;
 import java.lang.reflect.Method;
 import java.io.ByteArrayInputStream;
 import java.io.IOException;
 import java.util.HashMap;
 import java.io.InputStream;
 import java.util.Map;
@@ -28,15 +29,15 @@
 public class Unpickler
 {
     protected static final Object NO_RETURN_VALUE;
     protected final int HIGHEST_PROTOCOL = 5;
     protected Map<Integer, Object> memo;
     protected UnpickleStack stack;
     protected InputStream input;
-    protected static Map<String, IObjectConstructor> objectConstructors;
+    protected static final Map<String, IObjectConstructor> objectConstructors;
     
     public Unpickler() {
         this.memo = new HashMap<Integer, Object>();
     }
     
     public static void registerConstructor(final String module, final String classname, final IObjectConstructor constructor) {
         Unpickler.objectConstructors.put(module + "." + classname, constructor);
@@ -511,27 +512,27 @@
         final String str = PickleUtils.decode_unicode_escaped(PickleUtils.readline(this.input));
         this.stack.add((Object)str);
     }
     
     void load_binunicode() throws IOException {
         final int len = PickleUtils.bytes_to_integer(PickleUtils.readbytes(this.input, 4));
         final byte[] data = PickleUtils.readbytes(this.input, len);
-        this.stack.add((Object)new String(data, "UTF-8"));
+        this.stack.add((Object)new String(data, StandardCharsets.UTF_8));
     }
     
     void load_binunicode8() throws IOException {
         final long len = PickleUtils.bytes_to_long(PickleUtils.readbytes(this.input, 8), 0);
         final byte[] data = PickleUtils.readbytes(this.input, len);
-        this.stack.add((Object)new String(data, "UTF-8"));
+        this.stack.add((Object)new String(data, StandardCharsets.UTF_8));
     }
     
     void load_short_binunicode() throws IOException {
         final int len = PickleUtils.readbyte(this.input);
         final byte[] data = PickleUtils.readbytes(this.input, len);
-        this.stack.add((Object)new String(data, "UTF-8"));
+        this.stack.add((Object)new String(data, StandardCharsets.UTF_8));
     }
     
     void load_short_binstring() throws IOException {
         final short len = PickleUtils.readbyte(this.input);
         final byte[] data = PickleUtils.readbytes(this.input, (int)len);
         this.stack.add((Object)PickleUtils.rawStringFromBytes(data));
     }
@@ -593,16 +594,15 @@
             map.put(key, value);
         }
         this.stack.add((Object)map);
     }
     
     void load_frozenset() {
         final List<Object> top = this.stack.pop_all_since_marker();
-        final HashSet<Object> set = new HashSet<Object>();
-        set.addAll(top);
+        final HashSet<Object> set = new HashSet<Object>(top);
         this.stack.add((Object)set);
     }
     
     void load_additems() {
         final List<Object> top = this.stack.pop_all_since_marker();
         final HashSet<Object> set = (HashSet)this.stack.pop();
         set.addAll(top);
@@ -745,32 +745,32 @@
         this.load_reduce();
     }
     
     void load_newobj_ex() {
         final HashMap<?, ?> kwargs = (HashMap)this.stack.pop();
         final Object[] args = (Object[])this.stack.pop();
         final IObjectConstructor constructor = (IObjectConstructor)this.stack.pop();
-        if (kwargs.size() == 0) {
+        if (kwargs.isEmpty()) {
             this.stack.add(constructor.construct(args));
             return;
         }
         throw new PickleException("newobj_ex with keyword arguments not supported");
     }
     
     void load_frame() throws IOException {
         PickleUtils.readbytes(this.input, 8);
     }
     
     void load_persid() throws IOException {
         final String pid = PickleUtils.readline(this.input);
-        this.stack.add(this.persistentLoad(pid));
+        this.stack.add(this.persistentLoad((Object)pid));
     }
     
     void load_binpersid() throws IOException {
-        final String pid = this.stack.pop().toString();
+        final Object pid = this.stack.pop();
         this.stack.add(this.persistentLoad(pid));
     }
     
     void load_obj() throws IOException {
         List<Object> args = this.stack.pop_all_since_marker();
         final IObjectConstructor constructor = (IObjectConstructor)args.get(0);
         args = args.subList(1, args.size());
@@ -787,39 +787,39 @@
             constructor = (IObjectConstructor)new ClassDictConstructor(module, classname);
             args.clear();
         }
         final Object object = constructor.construct(args.toArray());
         this.stack.add(object);
     }
     
-    protected Object persistentLoad(final String pid) {
+    protected Object persistentLoad(final Object pid) {
         throw new PickleException("A load persistent id instruction was encountered, but no persistentLoad function was specified. (implement it in custom Unpickler subclass)");
     }
     
     static {
         NO_RETURN_VALUE = new Object();
-        (Unpickler.objectConstructors = new HashMap<String, IObjectConstructor>()).put("__builtin__.complex", (IObjectConstructor)new AnyClassConstructor((Class)ComplexNumber.class));
+        (objectConstructors = new HashMap<String, IObjectConstructor>()).put("__builtin__.complex", new AnyClassConstructor((Class)ComplexNumber.class));
         Unpickler.objectConstructors.put("builtins.complex", (IObjectConstructor)new AnyClassConstructor((Class)ComplexNumber.class));
         Unpickler.objectConstructors.put("array.array", (IObjectConstructor)new ArrayConstructor());
         Unpickler.objectConstructors.put("array._array_reconstructor", (IObjectConstructor)new ArrayConstructor());
         Unpickler.objectConstructors.put("__builtin__.bytearray", (IObjectConstructor)new ByteArrayConstructor());
         Unpickler.objectConstructors.put("builtins.bytearray", (IObjectConstructor)new ByteArrayConstructor());
         Unpickler.objectConstructors.put("__builtin__.bytes", (IObjectConstructor)new ByteArrayConstructor());
         Unpickler.objectConstructors.put("__builtin__.set", (IObjectConstructor)new SetConstructor());
         Unpickler.objectConstructors.put("builtins.set", (IObjectConstructor)new SetConstructor());
-        Unpickler.objectConstructors.put("datetime.datetime", (IObjectConstructor)new DateTimeConstructor(DateTimeConstructor.DATETIME));
-        Unpickler.objectConstructors.put("datetime.time", (IObjectConstructor)new DateTimeConstructor(DateTimeConstructor.TIME));
-        Unpickler.objectConstructors.put("datetime.date", (IObjectConstructor)new DateTimeConstructor(DateTimeConstructor.DATE));
-        Unpickler.objectConstructors.put("datetime.timedelta", (IObjectConstructor)new DateTimeConstructor(DateTimeConstructor.TIMEDELTA));
-        Unpickler.objectConstructors.put("pytz._UTC", (IObjectConstructor)new TimeZoneConstructor(TimeZoneConstructor.UTC));
-        Unpickler.objectConstructors.put("pytz._p", (IObjectConstructor)new TimeZoneConstructor(TimeZoneConstructor.PYTZ));
-        Unpickler.objectConstructors.put("pytz.timezone", (IObjectConstructor)new TimeZoneConstructor(TimeZoneConstructor.PYTZ));
-        Unpickler.objectConstructors.put("dateutil.tz.tzutc", (IObjectConstructor)new TimeZoneConstructor(TimeZoneConstructor.DATEUTIL_TZUTC));
-        Unpickler.objectConstructors.put("dateutil.tz.tzfile", (IObjectConstructor)new TimeZoneConstructor(TimeZoneConstructor.DATEUTIL_TZFILE));
-        Unpickler.objectConstructors.put("dateutil.zoneinfo.gettz", (IObjectConstructor)new TimeZoneConstructor(TimeZoneConstructor.DATEUTIL_GETTZ));
-        Unpickler.objectConstructors.put("datetime.tzinfo", (IObjectConstructor)new TimeZoneConstructor(TimeZoneConstructor.TZINFO));
+        Unpickler.objectConstructors.put("datetime.datetime", (IObjectConstructor)new DateTimeConstructor(1));
+        Unpickler.objectConstructors.put("datetime.time", (IObjectConstructor)new DateTimeConstructor(3));
+        Unpickler.objectConstructors.put("datetime.date", (IObjectConstructor)new DateTimeConstructor(2));
+        Unpickler.objectConstructors.put("datetime.timedelta", (IObjectConstructor)new DateTimeConstructor(4));
+        Unpickler.objectConstructors.put("pytz._UTC", (IObjectConstructor)new TimeZoneConstructor(1));
+        Unpickler.objectConstructors.put("pytz._p", (IObjectConstructor)new TimeZoneConstructor(2));
+        Unpickler.objectConstructors.put("pytz.timezone", (IObjectConstructor)new TimeZoneConstructor(2));
+        Unpickler.objectConstructors.put("dateutil.tz.tzutc", (IObjectConstructor)new TimeZoneConstructor(3));
+        Unpickler.objectConstructors.put("dateutil.tz.tzfile", (IObjectConstructor)new TimeZoneConstructor(4));
+        Unpickler.objectConstructors.put("dateutil.zoneinfo.gettz", (IObjectConstructor)new TimeZoneConstructor(5));
+        Unpickler.objectConstructors.put("datetime.tzinfo", (IObjectConstructor)new TimeZoneConstructor(6));
         Unpickler.objectConstructors.put("decimal.Decimal", (IObjectConstructor)new AnyClassConstructor((Class)BigDecimal.class));
         Unpickler.objectConstructors.put("copy_reg._reconstructor", (IObjectConstructor)new Reconstructor());
         Unpickler.objectConstructors.put("operator.attrgetter", (IObjectConstructor)new OperatorAttrGetterForCalendarTz());
         Unpickler.objectConstructors.put("_codecs.encode", (IObjectConstructor)new ByteArrayConstructor());
     }
 }
```

#### net/razorvine/pickle/objects/Tzinfo.class

##### procyon -ec {}

```diff
@@ -3,15 +3,15 @@
 
 import net.razorvine.pickle.PickleException;
 import java.util.HashMap;
 import java.util.TimeZone;
 
 public class Tzinfo
 {
-    private boolean forceTimeZone;
+    private final boolean forceTimeZone;
     private TimeZone timeZone;
     
     public Tzinfo(final TimeZone timeZone) {
         this.forceTimeZone = true;
         this.timeZone = timeZone;
     }
```

#### net/razorvine/pickle/objects/TimeZoneConstructor.class

##### procyon -ec {}

```diff
@@ -3,56 +3,56 @@
 
 import java.util.TimeZone;
 import net.razorvine.pickle.PickleException;
 import net.razorvine.pickle.IObjectConstructor;
 
 public class TimeZoneConstructor implements IObjectConstructor
 {
-    public static int UTC;
-    public static int PYTZ;
-    public static int DATEUTIL_TZUTC;
-    public static int DATEUTIL_TZFILE;
-    public static int DATEUTIL_GETTZ;
-    public static int TZINFO;
-    private int pythontype;
+    public static final int UTC = 1;
+    public static final int PYTZ = 2;
+    public static final int DATEUTIL_TZUTC = 3;
+    public static final int DATEUTIL_TZFILE = 4;
+    public static final int DATEUTIL_GETTZ = 5;
+    public static final int TZINFO = 6;
+    private final int pythontype;
     
     public TimeZoneConstructor(final int pythontype) {
         this.pythontype = pythontype;
     }
     
     public Object construct(final Object[] args) throws PickleException {
-        if (this.pythontype == TimeZoneConstructor.UTC) {
+        if (this.pythontype == 1) {
             return this.createUTC();
         }
-        if (this.pythontype == TimeZoneConstructor.PYTZ) {
+        if (this.pythontype == 2) {
             return this.createZoneFromPytz(args);
         }
-        if (this.pythontype == TimeZoneConstructor.DATEUTIL_TZUTC) {
+        if (this.pythontype == 3) {
             return this.createInfoFromDateutilTzutc(args);
         }
-        if (this.pythontype == TimeZoneConstructor.DATEUTIL_TZFILE) {
+        if (this.pythontype == 4) {
             return this.createInfoFromDateutilTzfile(args);
         }
-        if (this.pythontype == TimeZoneConstructor.DATEUTIL_GETTZ) {
+        if (this.pythontype == 5) {
             return this.createInfoFromDateutilGettz(args);
         }
-        if (this.pythontype == TimeZoneConstructor.TZINFO) {
+        if (this.pythontype == 6) {
             return this.createInfo(args);
         }
         throw new PickleException("invalid object type");
     }
     
     public Object reconstruct(final Object baseConstructor, final Object state) {
         if (!(state instanceof Tzinfo)) {
             throw new PickleException("invalid pickle data for tzinfo reconstruction; expected emtpy tzinfo state class");
         }
         if (!(baseConstructor instanceof TimeZoneConstructor)) {
             throw new PickleException("invalid pickle data for tzinfo reconstruction; expected a TimeZoneConstructor from a known tzinfo subclass");
         }
-        if (this.pythontype == TimeZoneConstructor.DATEUTIL_TZUTC) {
+        if (this.pythontype == 3) {
             return TimeZone.getTimeZone("UTC");
         }
         throw new PickleException("unsupported pickle data for tzinfo reconstruction; support for tzinfo subclasses other than tztuc has not been implemented");
     }
     
     private Object createInfo(final Object[] args) {
         return new Tzinfo();
@@ -92,17 +92,8 @@
         }
         return TimeZone.getTimeZone((String)args[0]);
     }
     
     private Object createUTC() {
         return TimeZone.getTimeZone("UTC");
     }
-    
-    static {
-        TimeZoneConstructor.UTC = 1;
-        TimeZoneConstructor.PYTZ = 2;
-        TimeZoneConstructor.DATEUTIL_TZUTC = 3;
-        TimeZoneConstructor.DATEUTIL_TZFILE = 4;
-        TimeZoneConstructor.DATEUTIL_GETTZ = 5;
-        TimeZoneConstructor.TZINFO = 6;
-    }
 }
```

#### net/razorvine/pickle/objects/DateTimeConstructor.class

##### procyon -ec {}

```diff
@@ -5,35 +5,35 @@
 import java.util.TimeZone;
 import java.util.Calendar;
 import net.razorvine.pickle.PickleException;
 import net.razorvine.pickle.IObjectConstructor;
 
 public class DateTimeConstructor implements IObjectConstructor
 {
-    public static int DATETIME;
-    public static int DATE;
-    public static int TIME;
-    public static int TIMEDELTA;
-    private int pythontype;
+    public static final int DATETIME = 1;
+    public static final int DATE = 2;
+    public static final int TIME = 3;
+    public static final int TIMEDELTA = 4;
+    private final int pythontype;
     
     public DateTimeConstructor(final int pythontype) {
         this.pythontype = pythontype;
     }
     
     public Object construct(final Object[] args) {
-        if (this.pythontype == DateTimeConstructor.DATE) {
+        if (this.pythontype == 2) {
             return this.createDate(args);
         }
-        if (this.pythontype == DateTimeConstructor.TIME) {
+        if (this.pythontype == 3) {
             return this.createTime(args);
         }
-        if (this.pythontype == DateTimeConstructor.DATETIME) {
+        if (this.pythontype == 1) {
             return this.createDateTime(args);
         }
-        if (this.pythontype == DateTimeConstructor.TIMEDELTA) {
+        if (this.pythontype == 4) {
             return this.createTimedelta(args);
         }
         throw new PickleException("invalid object type");
     }
     
     private TimeDelta createTimedelta(final Object[] args) {
         if (args.length != 3) {
@@ -202,15 +202,8 @@
             yhi = (params2[0] & 0xFF);
             ylo = (params2[1] & 0xFF);
             month2 = (params2[2] & 0xFF) - 1;
             day2 = (params2[3] & 0xFF);
         }
         return new GregorianCalendar(yhi * 256 + ylo, month2, day2);
     }
-    
-    static {
-        DateTimeConstructor.DATETIME = 1;
-        DateTimeConstructor.DATE = 2;
-        DateTimeConstructor.TIME = 3;
-        DateTimeConstructor.TIMEDELTA = 4;
-    }
 }
```

#### net/razorvine/pickle/objects/OperatorAttrGetterForCalendarTz$AttrGetterForTz.class

##### procyon -ec {}

```diff
@@ -1,21 +1,20 @@
 
 package net.razorvine.pickle.objects;
 
 import net.razorvine.pickle.PickleException;
 import java.util.TimeZone;
 import net.razorvine.pickle.IObjectConstructor;
 
-class AttrGetterForTz implements IObjectConstructor
+static class AttrGetterForTz implements IObjectConstructor
 {
-    public AttrGetterForTz(final OperatorAttrGetterForCalendarTz this$0) {
-        this.this$0 = this$0;
+    public AttrGetterForTz() {
     }
     
     public Object construct(final Object[] args) {
         if (args.length != 1 || !(args[0] instanceof TimeZone)) {
             throw new PickleException("expected exactly one TimeZone argument for construction of CalendarLocalizer");
         }
         final TimeZone tz = (TimeZone)args[0];
-        return new OperatorAttrGetterForCalendarTz.CalendarLocalizer(this.this$0, tz);
+        return new OperatorAttrGetterForCalendarTz.CalendarLocalizer(tz);
     }
 }
```

#### net/razorvine/pickle/objects/ClassDict.class

##### procyon -ec {}

```diff
@@ -1,34 +1,31 @@
 
 package net.razorvine.pickle.objects;
 
-import java.util.Iterator;
 import java.util.Map;
 import java.util.HashMap;
 
 public class ClassDict extends HashMap<String, Object>
 {
     private static final long serialVersionUID = 6157715596627049511L;
-    private String classname;
+    private final String classname;
     
     public ClassDict(final String modulename, final String classname) {
         if (modulename == null) {
             this.classname = classname;
         }
         else {
             this.classname = modulename + "." + classname;
         }
         ((HashMap<String, String>)this).put("__class__", this.classname);
     }
     
     public void __setstate__(final HashMap<String, Object> values) {
         this.clear();
         ((HashMap<String, String>)this).put("__class__", this.classname);
-        for (final Map.Entry<String, Object> e : values.entrySet()) {
-            this.put(e.getKey(), e.getValue());
-        }
+        this.putAll(values);
     }
     
     public String getClassName() {
         return this.classname;
     }
 }
```

#### net/razorvine/pickle/objects/ClassDictConstructor.class

##### procyon -ec {}

```diff
@@ -2,16 +2,16 @@
 package net.razorvine.pickle.objects;
 
 import net.razorvine.pickle.PickleException;
 import net.razorvine.pickle.IObjectConstructor;
 
 public class ClassDictConstructor implements IObjectConstructor
 {
-    String module;
-    String name;
+    final String module;
+    final String name;
     
     public ClassDictConstructor(final String module, final String name) {
         this.module = module;
         this.name = name;
     }
     
     public Object construct(final Object[] args) {
```

#### net/razorvine/pickle/objects/Time.class

##### procyon -ec {}

```diff
@@ -3,18 +3,18 @@
 
 import java.util.Calendar;
 import java.io.Serializable;
 
 public class Time implements Serializable
 {
     private static final long serialVersionUID = 2325820650757621315L;
-    public int hours;
-    public int minutes;
-    public int seconds;
-    public int microseconds;
+    public final int hours;
+    public final int minutes;
+    public final int seconds;
+    public final int microseconds;
     
     public Time(final int h, final int m, final int s, final int microsecs) {
         this.hours = h;
         this.minutes = m;
         this.seconds = s;
         this.microseconds = microsecs;
     }
```

#### net/razorvine/pickle/objects/ExceptionConstructor.class

##### procyon -ec {}

```diff
@@ -4,16 +4,16 @@
 import java.lang.reflect.Field;
 import java.lang.reflect.Constructor;
 import net.razorvine.pickle.PickleException;
 import net.razorvine.pickle.IObjectConstructor;
 
 public class ExceptionConstructor implements IObjectConstructor
 {
-    private Class<?> type;
-    private String pythonExceptionType;
+    private final Class<?> type;
+    private final String pythonExceptionType;
     
     public ExceptionConstructor(final Class<?> type, final String module, final String name) {
         if (module != null) {
             this.pythonExceptionType = module + "." + name;
         }
         else {
             this.pythonExceptionType = name;
@@ -24,15 +24,15 @@
     public Object construct(Object[] args) {
         try {
             if (this.pythonExceptionType != null) {
                 if (args == null || args.length == 0) {
                     args = new String[] { "[" + this.pythonExceptionType + "]" };
                 }
                 else {
-                    final String msg = "[" + this.pythonExceptionType + "] " + (String)args[0];
+                    final String msg = "[" + this.pythonExceptionType + "] " + args[0];
                     args = new String[] { msg };
                 }
             }
             final Class<?>[] paramtypes = new Class[args.length];
             for (int i = 0; i < args.length; ++i) {
                 paramtypes[i] = args[i].getClass();
             }
```

#### net/razorvine/pickle/objects/OperatorAttrGetterForCalendarTz.class

##### procyon -ec {}

```diff
@@ -7,12 +7,12 @@
 public class OperatorAttrGetterForCalendarTz implements IObjectConstructor
 {
     public Object construct(final Object[] args) {
         if (args.length != 1) {
             throw new PickleException("expected exactly one string argument for construction of AttrGetter");
         }
         if ("localize".equals(args[0])) {
-            return new OperatorAttrGetterForCalendarTz.AttrGetterForTz(this);
+            return new OperatorAttrGetterForCalendarTz.AttrGetterForTz();
         }
         throw new PickleException("expected 'localize' string argument for construction of AttrGetter");
     }
 }
```

#### net/razorvine/pickle/objects/OperatorAttrGetterForCalendarTz$CalendarLocalizer.class

##### procyon -ec {}

```diff
@@ -2,20 +2,19 @@
 package net.razorvine.pickle.objects;
 
 import net.razorvine.pickle.PickleException;
 import java.util.Calendar;
 import java.util.TimeZone;
 import net.razorvine.pickle.IObjectConstructor;
 
-class CalendarLocalizer implements IObjectConstructor
+static class CalendarLocalizer implements IObjectConstructor
 {
-    TimeZone tz;
+    final TimeZone tz;
     
-    public CalendarLocalizer(final OperatorAttrGetterForCalendarTz this$0, final TimeZone tz) {
-        this.this$0 = this$0;
+    public CalendarLocalizer(final TimeZone tz) {
         this.tz = tz;
     }
     
     public Object construct(final Object[] args) {
         if (args.length != 1 || !(args[0] instanceof Calendar)) {
             throw new PickleException("expected exactly one Calendar argument for construction of Calendar with timezone");
         }
```

#### net/razorvine/pickle/objects/AnyClassConstructor.class

##### procyon -ec {}

```diff
@@ -4,15 +4,15 @@
 import java.lang.reflect.Constructor;
 import net.razorvine.pickle.PickleException;
 import java.math.BigDecimal;
 import net.razorvine.pickle.IObjectConstructor;
 
 public class AnyClassConstructor implements IObjectConstructor
 {
-    private Class<?> type;
+    private final Class<?> type;
     
     public AnyClassConstructor(final Class<?> type) {
         this.type = type;
     }
     
     public Object construct(final Object[] args) {
         try {
```

#### net/razorvine/pickle/objects/ComplexNumber.class

##### procyon -ec {}

```diff
@@ -2,30 +2,30 @@
 package net.razorvine.pickle.objects;
 
 import java.io.Serializable;
 
 public class ComplexNumber implements Serializable
 {
     private static final long serialVersionUID = 4668080260997226513L;
-    private double r;
-    private double i;
+    private final double r;
+    private final double i;
     
     public ComplexNumber(final double rr, final double ii) {
         this.r = rr;
         this.i = ii;
     }
     
     public ComplexNumber(final Double rr, final Double ii) {
         this.r = rr;
         this.i = ii;
     }
     
     @Override
     public String toString() {
-        final StringBuffer sb = new StringBuffer().append(this.r);
+        final StringBuilder sb = new StringBuilder().append(this.r);
         if (this.i >= 0.0) {
             sb.append('+');
         }
         return sb.append(this.i).append('i').toString();
     }
     
     public double getReal() {
```

#### net/razorvine/pickle/objects/TimeDelta.class

##### procyon -ec {}

```diff
@@ -4,18 +4,18 @@
 import java.text.NumberFormat;
 import java.util.Locale;
 import java.io.Serializable;
 
 public class TimeDelta implements Serializable
 {
     private static final long serialVersionUID = 7655189815303876847L;
-    public int days;
-    public int seconds;
-    public int microseconds;
-    public double total_seconds;
+    public final int days;
+    public final int seconds;
+    public final int microseconds;
+    public final double total_seconds;
     
     public TimeDelta(final int days, final int seconds, final int microseconds) {
         this.days = days;
         this.seconds = seconds;
         this.microseconds = microseconds;
         this.total_seconds = days * 86400 + seconds + microseconds / 1000000.0;
     }
```

#### net/razorvine/pickle/Pickler.class

##### procyon -ec {}

```diff
@@ -1,12 +1,13 @@
 
 package net.razorvine.pickle;
 
 import java.lang.reflect.Method;
 import java.lang.reflect.InvocationTargetException;
+import java.nio.charset.StandardCharsets;
 import java.util.Iterator;
 import java.io.Serializable;
 import java.util.Collection;
 import java.util.List;
 import java.util.Set;
 import java.util.TimeZone;
 import net.razorvine.pickle.objects.TimeDelta;
@@ -20,34 +21,34 @@
 import java.util.HashMap;
 import java.util.Map;
 import java.io.OutputStream;
 
 public class Pickler
 {
     public static int HIGHEST_PROTOCOL;
-    protected static int MAX_RECURSE_DEPTH;
+    protected static final int MAX_RECURSE_DEPTH = 1000;
     protected int recurse;
     protected OutputStream out;
-    protected int PROTOCOL;
-    protected static Map<Class<?>, IObjectPickler> customPicklers;
+    protected final int PROTOCOL = 2;
+    protected static final Map<Class<?>, IObjectPickler> customPicklers;
+    protected static Map<Class<?>, IObjectDeconstructor> customDeconstructors;
     protected boolean useMemo;
     protected boolean valueCompare;
     protected HashMap<Integer, Pickler.Memo> memo;
     
     public Pickler() {
         this(true);
     }
     
     public Pickler(final boolean useMemo) {
         this(useMemo, true);
     }
     
     public Pickler(final boolean useMemo, final boolean valueCompare) {
         this.recurse = 0;
-        this.PROTOCOL = 2;
         this.useMemo = true;
         this.valueCompare = true;
         this.useMemo = useMemo;
         this.valueCompare = valueCompare;
     }
     
     public void close() throws IOException {
@@ -56,42 +57,46 @@
         this.out.close();
     }
     
     public static void registerCustomPickler(final Class<?> clazz, final IObjectPickler pickler) {
         Pickler.customPicklers.put(clazz, pickler);
     }
     
+    public static void registerCustomDeconstructor(final Class<?> clazz, final IObjectDeconstructor deconstructor) {
+        Pickler.customDeconstructors.put(clazz, deconstructor);
+    }
+    
     public byte[] dumps(final Object o) throws PickleException, IOException {
         final ByteArrayOutputStream bo = new ByteArrayOutputStream();
         this.dump(o, bo);
         bo.flush();
         return bo.toByteArray();
     }
     
     public void dump(final Object o, final OutputStream stream) throws IOException, PickleException {
         this.out = stream;
         this.recurse = 0;
         if (this.useMemo) {
             this.memo = new HashMap<Integer, Pickler.Memo>();
         }
         this.out.write(128);
-        this.out.write(this.PROTOCOL);
+        this.out.write(2);
         this.save(o);
         this.memo = null;
         this.out.write(46);
         this.out.flush();
         if (this.recurse != 0) {
             throw new PickleException("recursive structure error, please report this problem");
         }
     }
     
     public void save(final Object o) throws PickleException, IOException {
         ++this.recurse;
-        if (this.recurse > Pickler.MAX_RECURSE_DEPTH) {
-            throw new StackOverflowError("recursion too deep in Pickler.save (>" + Pickler.MAX_RECURSE_DEPTH + ")");
+        if (this.recurse > 1000) {
+            throw new StackOverflowError("recursion too deep in Pickler.save (>1000)");
         }
         if (o == null) {
             this.out.write(78);
             --this.recurse;
             return;
         }
         final Class<?> t = o.getClass();
@@ -198,14 +203,32 @@
         }
         final IObjectPickler custompickler = this.getCustomPickler(t);
         if (custompickler != null) {
             custompickler.pickle(o, this.out, this);
             this.writeMemo(o);
             return true;
         }
+        final IObjectDeconstructor customDeconstructor = this.getCustomDeconstructor(t);
+        if (customDeconstructor != null) {
+            this.put_global(customDeconstructor, o);
+            return true;
+        }
+        final Object persistentId = this.persistentId(o);
+        if (persistentId != null) {
+            if (persistentId instanceof String && !((String)persistentId).contains("\n")) {
+                this.out.write(80);
+                this.out.write(((String)persistentId).getBytes());
+                this.out.write("\n".getBytes());
+            }
+            else {
+                this.save(persistentId);
+                this.out.write(81);
+            }
+            return true;
+        }
         if (o instanceof String) {
             this.put_string((String)o);
             return true;
         }
         if (o instanceof BigInteger) {
             this.put_bigint((BigInteger)o);
             return true;
@@ -283,14 +306,18 @@
             if (((Class)x.getKey()).isAssignableFrom(t)) {
                 return x.getValue();
             }
         }
         return null;
     }
     
+    protected IObjectDeconstructor getCustomDeconstructor(final Class<?> t) {
+        return Pickler.customDeconstructors.get(t);
+    }
+    
     void put_collection(final Collection<?> list) throws IOException {
         this.out.write(93);
         this.writeMemo(list);
         this.out.write(40);
         for (final Object o : list) {
             this.save(o);
         }
@@ -525,14 +552,25 @@
         }
         this.out.write(101);
         this.out.write(134);
         this.out.write(82);
         this.writeMemo(array);
     }
     
+    void put_global(final IObjectDeconstructor deconstructor, final Object obj) throws IOException {
+        this.out.write(99);
+        this.out.write((deconstructor.getModule() + "\n" + deconstructor.getName() + "\n").getBytes());
+        final Object[] values = deconstructor.deconstruct(obj);
+        if (values.length > 0) {
+            this.save(values);
+            this.out.write(82);
+        }
+        this.writeMemo(obj);
+    }
+    
     void put_decimal(final BigDecimal d) throws IOException {
         this.out.write(99);
         this.out.write("decimal\nDecimal\n".getBytes());
         this.put_string(d.toEngineeringString());
         this.out.write(133);
         this.out.write(82);
         this.writeMemo(d);
@@ -550,15 +588,15 @@
             this.out.write(PickleUtils.integer_to_bytes(b.length));
             this.out.write(b);
         }
         this.writeMemo(i);
     }
     
     void put_string(final String string) throws IOException {
-        final byte[] encoded = string.getBytes("UTF-8");
+        final byte[] encoded = string.getBytes(StandardCharsets.UTF_8);
         this.out.write(88);
         this.out.write(PickleUtils.integer_to_bytes(encoded.length));
         this.out.write(encoded);
         this.writeMemo(string);
     }
     
     void put_float(final double d) throws IOException {
@@ -640,13 +678,17 @@
             throw new PickleException("couldn't introspect javabean: " + e2);
         }
         catch (final InvocationTargetException e3) {
             throw new PickleException("couldn't introspect javabean: " + e3);
         }
     }
     
+    protected Object persistentId(final Object obj) {
+        return null;
+    }
+    
     static {
         Pickler.HIGHEST_PROTOCOL = 2;
-        Pickler.MAX_RECURSE_DEPTH = 1000;
-        Pickler.customPicklers = new HashMap<Class<?>, IObjectPickler>();
+        customPicklers = new HashMap<Class<?>, IObjectPickler>();
+        Pickler.customDeconstructors = new HashMap<Class<?>, IObjectDeconstructor>();
     }
 }
```

#### META-INF/maven/net.razorvine/pickle/pom.xml

##### META-INF/maven/net.razorvine/pickle/pom.xml

```diff
@@ -4,15 +4,15 @@
   <parent>
     <groupId>org.sonatype.oss</groupId>
     <artifactId>oss-parent</artifactId>
     <version>9</version>
   </parent>
   <groupId>net.razorvine</groupId>
   <artifactId>pickle</artifactId>
-  <version>1.4</version>
+  <version>1.5</version>
   <packaging>jar</packaging>
   <name>pickle</name>
   <url>https://github.com/irmen/pickle</url>
   <properties>
     <project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
   </properties>
   <build>
@@ -52,23 +52,29 @@
       </plugins>
     </pluginManagement>
   </build>
   <dependencies>
     <dependency>
       <groupId>junit</groupId>
       <artifactId>junit</artifactId>
-      <version>4.13.1</version>
+      <version>4.13.2</version>
+      <scope>test</scope>
+    </dependency>
+    <dependency>
+      <groupId>org.hamcrest</groupId>
+      <artifactId>hamcrest-core</artifactId>
+      <version>1.3</version>
       <scope>test</scope>
     </dependency>
   </dependencies>
   <scm>
     <url>https://github.com/irmen/pickle</url>
     <connection>scm:git:ssh://git@github.com/irmen/pickle.git</connection>
     <developerConnection>scm:git:ssh://git@github.com/irmen/pickle.git</developerConnection>
-    <tag>pickle-1.4</tag>
+    <tag>pickle-1.5</tag>
   </scm>
   <issueManagement>
     <system>Github</system>
     <url>https://github.com/irmen/pickle/issues</url>
   </issueManagement>
   <developers>
     <developer>
```

#### META-INF/maven/net.razorvine/pickle/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Wed May 24 21:16:48 CEST 2023
+#Sun Nov 19 15:16:33 CET 2023
 groupId=net.razorvine
 artifactId=pickle
-version=1.4
+version=1.5
```

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/pmml-xgboost-1.7.4.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/pmml-xgboost-1.7.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.41.jar` & `sklearn2pmml-0.99.3/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.42.jar`

 * *Files 12% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 7607 bytes, number of entries: 15
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Oct-23 22:44 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 lightgbm/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Oct-23 22:44 lightgbm/sklearn/
--rw-rw-r--  2.0 unx      177 b- defN 23-Oct-23 22:44 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx      170 b- defN 23-Oct-23 22:44 lightgbm/sklearn/HasBooster.class
--rw-rw-r--  2.0 unx     2047 b- defN 23-Oct-23 22:44 lightgbm/sklearn/Booster.class
--rw-rw-r--  2.0 unx     2288 b- defN 23-Oct-23 22:44 lightgbm/sklearn/LGBMRegressor.class
--rw-rw-r--  2.0 unx     2312 b- defN 23-Oct-23 22:44 lightgbm/sklearn/LGBMClassifier.class
--rw-rw-r--  2.0 unx     3797 b- defN 23-Oct-23 22:44 lightgbm/sklearn/BoosterUtil.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Oct-23 22:44 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Oct-23 22:44 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Oct-23 22:44 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/
--rw-rw-r--  2.0 unx     1319 b- defN 23-Oct-23 22:44 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml
--rw-rw-r--  2.0 unx      117 b- defN 23-Oct-23 22:44 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.properties
-15 files, 12357 bytes uncompressed, 5527 bytes compressed:  55.3%
+Zip file size: 7606 bytes, number of entries: 15
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Dec-04 22:17 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 lightgbm/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Dec-04 22:17 lightgbm/sklearn/
+-rw-rw-r--  2.0 unx      177 b- defN 23-Dec-04 22:17 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx      170 b- defN 23-Dec-04 22:17 lightgbm/sklearn/HasBooster.class
+-rw-rw-r--  2.0 unx     2047 b- defN 23-Dec-04 22:17 lightgbm/sklearn/Booster.class
+-rw-rw-r--  2.0 unx     2288 b- defN 23-Dec-04 22:17 lightgbm/sklearn/LGBMRegressor.class
+-rw-rw-r--  2.0 unx     2312 b- defN 23-Dec-04 22:17 lightgbm/sklearn/LGBMClassifier.class
+-rw-rw-r--  2.0 unx     3797 b- defN 23-Dec-04 22:17 lightgbm/sklearn/BoosterUtil.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Dec-04 22:17 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Dec-04 22:17 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Dec-04 22:17 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/
+-rw-rw-r--  2.0 unx     1319 b- defN 23-Dec-04 22:16 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml
+-rw-rw-r--  2.0 unx      116 b- defN 23-Dec-04 22:17 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.properties
+15 files, 12356 bytes uncompressed, 5526 bytes compressed:  55.3%
```

#### META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.41</version>
+    <version>1.7.42</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-lightgbm</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn LightGBM converter</name>
   <description>JPMML Scikit-Learn LightGBM to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Mon Oct 23 22:44:50 EEST 2023
-version=1.7.41
+#Mon Dec 04 22:17:24 EET 2023
+version=1.7.42
 groupId=org.jpmml
 artifactId=pmml-sklearn-lightgbm
```

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/preprocessing/h2o.py` & `sklearn2pmml-0.99.3/sklearn2pmml/preprocessing/h2o.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/preprocessing/__init__.py` & `sklearn2pmml-0.99.3/sklearn2pmml/preprocessing/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from datetime import datetime
 from io import StringIO
 from pandas import DataFrame, Series
 from scipy.interpolate import BSpline
 from scipy.sparse import lil_matrix
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.pipeline import Pipeline
-from sklearn2pmml.util import cast, dt_transform, ensure_1d, ensure_def, eval_rows, eval_expr_rows, to_expr_func, Expression, Predicate
+from sklearn2pmml.util import cast, dt_transform, ensure_1d, ensure_def, eval_rows, to_expr_func, Expression, Predicate
 
 import numpy
 import pandas
 import types
 import warnings
 
 def _regex_engine(pattern):
@@ -623,56 +623,64 @@
 	result = numpy.empty((X.shape[0], step_result.shape[1]), dtype = object)
 	# Fill array
 	result[step_mask.ravel(), :] = step_result
 	return result
 
 class SelectFirstTransformer(BaseEstimator, TransformerMixin):
 
-	def __init__(self, steps, controller = None):
+	def __init__(self, steps, controller = None, eval_rows = True):
 		for step in steps:
 			if type(step) is not tuple:
 				raise TypeError("Step is not a tuple")
 			if len(step) != 3:
 				raise TypeError("Step is not a three-element (name, transformer, predicate) tuple")
 			name, transformer, predicate = step
 			if not isinstance(predicate, (str, Predicate)):
 				raise TypeError()
 		self.steps = steps
 		if controller:
 			if not hasattr(controller, "transform"):
 				raise TypeError()
 		self.controller = controller
+		self.eval_rows = eval_rows
 
 	def _to_evaluation_dataset(self, X):
 		if self.controller is not None:
 			return self.controller.transform(X)
 		return X
 
+	def _eval_step_mask(self, X, predicate):
+		step_func = to_expr_func(predicate)
+		if self.eval_rows:
+			return eval_rows(X, step_func, dtype = bool)
+		else:
+			return step_func(X)
+
 	def fit(self, X, y = None):
 		X_eval = self._to_evaluation_dataset(X)
-		mask = numpy.zeros(X.shape[0], dtype = bool)
+		mask = numpy.full(X.shape[0], fill_value = False)
 		for name, transformer, predicate in self.steps:
 			step_mask = numpy.logical_not(mask)
-			step_mask_eval = eval_expr_rows(X_eval[step_mask], predicate, dtype = bool)
+			step_mask_eval = self._eval_step_mask(X_eval[step_mask], predicate)
 			if numpy.sum(step_mask_eval) < 1:
 				raise ValueError(predicate)
 			step_mask[step_mask] = step_mask_eval
 			step_X = X[step_mask]
 			step_y = y[step_mask] if y is not None else None
 			transformer.fit(step_X, step_y)
 			mask = numpy.logical_or(mask, step_mask)
 		return self
 
 	def transform(self, X):
 		result = None
 		X_eval = self._to_evaluation_dataset(X)
-		mask = numpy.zeros(X.shape[0], dtype = bool)
+		mask = numpy.full(X.shape[0], fill_value = False)
 		for name, transformer, predicate in self.steps:
 			step_mask = numpy.logical_not(mask)
-			step_mask_eval = eval_expr_rows(X_eval[step_mask], predicate, dtype = bool)
+			step_mask_eval = self._eval_step_mask(X_eval[step_mask], predicate)
 			if numpy.sum(step_mask_eval) < 1:
 				continue
 			step_mask[step_mask] = step_mask_eval
 			step_X = X[step_mask]
 			step_result = transformer.transform(step_X)
 			step_result = _to_sparse(X, step_mask, step_result)
 			if result is None:
```

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/preprocessing/xgboost.py` & `sklearn2pmml-0.99.3/sklearn2pmml/preprocessing/xgboost.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/preprocessing/lightgbm.py` & `sklearn2pmml-0.99.3/sklearn2pmml/preprocessing/lightgbm.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/tree/chaid.py` & `sklearn2pmml-0.99.3/sklearn2pmml/tree/chaid.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.99.2/sklearn2pmml/expression/__init__.py` & `sklearn2pmml-0.99.3/sklearn2pmml/expression/__init__.py`

 * *Files identical despite different names*

