# Comparing `tmp/opentldr-0.3.0.tar.gz` & `tmp/opentldr-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentldr-0.3.0.tar", last modified: Wed Mar 20 00:11:25 2024, max compression
+gzip compressed data, was "opentldr-0.3.1.tar", last modified: Tue Apr  2 20:25:41 2024, max compression
```

## Comparing `opentldr-0.3.0.tar` & `opentldr-0.3.1.tar`

### file list

```diff
@@ -1,25 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 00:11:25.064926 opentldr-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-20 00:11:20.000000 opentldr-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 00:11:20.000000 opentldr-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-03-20 00:11:25.064926 opentldr-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-03-20 00:11:20.000000 opentldr-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-20 00:11:20.000000 opentldr-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 00:11:25.064926 opentldr-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 00:11:25.056926 opentldr-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 00:11:25.060926 opentldr-0.3.0/src/opentldr/
--rw-r--r--   0 runner    (1001) docker     (127)    11986 2024-03-20 00:11:20.000000 opentldr-0.3.0/src/opentldr/ContentRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)    16948 2024-03-20 00:11:20.000000 opentldr-0.3.0/src/opentldr/Domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    27413 2024-03-20 00:11:20.000000 opentldr-0.3.0/src/opentldr/KnowledgeGraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-03-20 00:11:20.000000 opentldr-0.3.0/src/opentldr/Workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-20 00:11:20.000000 opentldr-0.3.0/src/opentldr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 00:11:25.060926 opentldr-0.3.0/src/opentldr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-03-20 00:11:25.000000 opentldr-0.3.0/src/opentldr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-20 00:11:25.000000 opentldr-0.3.0/src/opentldr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 00:11:25.000000 opentldr-0.3.0/src/opentldr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-20 00:11:25.000000 opentldr-0.3.0/src/opentldr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-20 00:11:25.000000 opentldr-0.3.0/src/opentldr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 00:11:25.060926 opentldr-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-20 00:11:20.000000 opentldr-0.3.0/tests/test_contentrepo.py
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-20 00:11:20.000000 opentldr-0.3.0/tests/test_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-20 00:11:20.000000 opentldr-0.3.0/tests/test_knowledgegraph.py
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-20 00:11:20.000000 opentldr-0.3.0/tests/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:25:41.705143 opentldr-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 20:25:34.000000 opentldr-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:25:34.000000 opentldr-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-04-02 20:25:41.705143 opentldr-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-04-02 20:25:34.000000 opentldr-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-02 20:25:34.000000 opentldr-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 20:25:41.705143 opentldr-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:25:41.701143 opentldr-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:25:41.701143 opentldr-0.3.1/src/opentldr/
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-02 20:25:34.000000 opentldr-0.3.1/src/opentldr/AbstractDataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-02 20:25:34.000000 opentldr-0.3.1/src/opentldr/DataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-04-02 20:25:34.000000 opentldr-0.3.1/src/opentldr/DataRepoJson.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26173 2024-04-02 20:25:34.000000 opentldr-0.3.1/src/opentldr/Domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30006 2024-04-02 20:25:34.000000 opentldr-0.3.1/src/opentldr/KnowledgeGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-02 20:25:34.000000 opentldr-0.3.1/src/opentldr/S3DataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-04-02 20:25:34.000000 opentldr-0.3.1/src/opentldr/TextFileDataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-02 20:25:34.000000 opentldr-0.3.1/src/opentldr/Workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-02 20:25:34.000000 opentldr-0.3.1/src/opentldr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-02 20:25:34.000000 opentldr-0.3.1/src/opentldr/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:25:41.705143 opentldr-0.3.1/src/opentldr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-04-02 20:25:41.000000 opentldr-0.3.1/src/opentldr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-02 20:25:41.000000 opentldr-0.3.1/src/opentldr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:25:41.000000 opentldr-0.3.1/src/opentldr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-02 20:25:41.000000 opentldr-0.3.1/src/opentldr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 20:25:41.000000 opentldr-0.3.1/src/opentldr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:25:41.705143 opentldr-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 20:25:34.000000 opentldr-0.3.1/tests/test_contentrepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 20:25:34.000000 opentldr-0.3.1/tests/test_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-02 20:25:34.000000 opentldr-0.3.1/tests/test_knowledgegraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 20:25:34.000000 opentldr-0.3.1/tests/test_workflow.py
```

### Comparing `opentldr-0.3.0/LICENSE` & `opentldr-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opentldr-0.3.0/PKG-INFO` & `opentldr-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: opentldr
-Version: 0.3.0
+Version: 0.3.1
 Summary: An open framework for creation of a Tailored Daily Report.
 Author-email: Chris Argenta <cargenta@rockfishresearch.com>
-Project-URL: Source, https://github.com/RockfishResearch/OpenTLDR
-Project-URL: Issues, https://github.com/RockfishResearch/OpenTLDR/issues
+Project-URL: Source, https://github.com/RockfishResearch/OpenTLDR-Core.git
+Project-URL: Issues, https://github.com/RockfishResearch/OpenTLDR-Core/issues
 Project-URL: Documentation, http://www.opentldr.org/docs
 Project-URL: Homepage, http://www.opentldr.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-dotenv>=1.0.0
 Requires-Dist: neo4j>=5.15.0
 Requires-Dist: neomodel>=5.2.1
 Requires-Dist: papermill>=2.5.0
 Requires-Dist: boto3>=1.34.55
@@ -30,15 +30,15 @@
 
 OpenTLDR is an open source framework written in Python to implement the process of creating a Tailored Daily Report from a series of news-like articles. This repository contains the Core classes used as a library by OpenTLDR implementations, like the example notebooks you canf ind in the OpenTLDR-Example repo on GitHub.
 
 OpenTLDR is composed of Python modules:
 - A **KnowledgeGraph** modulethat has been implemented as a layer on top of the Neo4j Graph Database
 - A module with a set of **Domain** classes that implement the nodes and edges in a TLDR-focused knowledge graph
 - A **Workflow** module and tool that wraps the execution of a series of Python Notebooks to make them behave like components
-- A **ContentRepo** module that abstracts the data ingest from Python Notebooks using a config parameter for either S3 or Files
+- A **DataRepo** module that abstracts the data ingest from Python Notebooks using a config parameter for either S3 or Files
 
 This GitHub repo handles the back-end code that and is only required if you with to modify this functionality directly. Otherwise, you should use the OpenTDLR-Example repository, which implements analytic pieces of the process in a series of Jupyter Notebooks. All of the code in this repo is availible
 to Python code as a pip library using a command like `python3 -m pip install opentldr` please make sure that you need to modify this library directly before using this codebase.
 
 ## KnowledgeGraph
 
 OpenTLDR uses a neo4j graph database as the storage layer of its KnowledgeGraph. The default (and easiest) way to do this is to run the Community Edition neo4j Server in a Docker container on the local machine that you execute OpenTLDR workflows. A linux shell script (start_neo4j.sh) and docker-compose configuraiton file (scripts/Neo4j/docker-compose) automate this process. The default container does not require authentication but only connects to localhost loopback interface. You can change all of this and use .env or system environment variables to direct the OpenTLDR library to use the desired neo4j server and user credientials.
@@ -96,16 +96,16 @@
    ...
     "repo_config": {'repo_type': 'files', 'path': './sample_data'}
     }
 </pre>
 
 Note that this format is likely to change to better support passing different parameters into individual steps.
 
-## ContentRepo
-The ContentRepo class provides an abstraction for locating data to use within the steps of the workflow. For example, in the above variables_to_set specification, there is a config json string `repo_config` that indicates to pull data from a directory of files located at the given path. At this time, only files and S3 buckets are implemented:
+## DataRepo
+The DataRepo class provides an abstraction for locating data to use within the steps of the workflow. For example, in the above variables_to_set specification, there is a config json string `repo_config` that indicates to pull data from a directory of files located at the given path. At this time, only files and S3 buckets are implemented:
 
 Config for using files, in this case from the local sample_data folder:
 <pre>
 repo_config = {
         'repo_type': 'files',
         'path': './sample_data'
         }
@@ -117,19 +117,19 @@
         'repo_type': 's3',
         'bucket': os.getenv("S3_BUCKET"),
         'aws_access_key_id': os.getenv("S3_ACCESS_KEY_ID"),
         'aws_secret_access_key': os.getenv("S3_SECRET_KEY")
         }
 </pre>
 
-Below is an example of using the ContentRepo to load news content from either of the above:
+Below is an example of using the DataRepo to load news content from either of the above:
 <pre>
-from opentldr import KnowledgeGraph, ContentRepo
+from opentldr import KnowledgeGraph, DataRepo
 
 kg = KnowledgeGraph()
-cr = ContentRepo(kg, repo_config)
+cr = DataRepo(kg, repo_config)
 
 for uid in cr.importContentData():
     print ("Loaded Content: {uid}".format(uid=uid))
 </pre>
-This will create a ContentRepo that writes to the KnowledgeGraph kg from the parsed Content configured above. The return value is a list of the uids of Content nodes created (note Source nodes would be created if needed but not returned here).
+This will create a DataRepo that writes to the KnowledgeGraph kg from the parsed Content configured above. The return value is a list of the uids of Content nodes created (note Source nodes would be created if needed but not returned here).
```

### Comparing `opentldr-0.3.0/README.md` & `opentldr-0.3.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 OpenTLDR is an open source framework written in Python to implement the process of creating a Tailored Daily Report from a series of news-like articles. This repository contains the Core classes used as a library by OpenTLDR implementations, like the example notebooks you canf ind in the OpenTLDR-Example repo on GitHub.
 
 OpenTLDR is composed of Python modules:
 - A **KnowledgeGraph** modulethat has been implemented as a layer on top of the Neo4j Graph Database
 - A module with a set of **Domain** classes that implement the nodes and edges in a TLDR-focused knowledge graph
 - A **Workflow** module and tool that wraps the execution of a series of Python Notebooks to make them behave like components
-- A **ContentRepo** module that abstracts the data ingest from Python Notebooks using a config parameter for either S3 or Files
+- A **DataRepo** module that abstracts the data ingest from Python Notebooks using a config parameter for either S3 or Files
 
 This GitHub repo handles the back-end code that and is only required if you with to modify this functionality directly. Otherwise, you should use the OpenTDLR-Example repository, which implements analytic pieces of the process in a series of Jupyter Notebooks. All of the code in this repo is availible
 to Python code as a pip library using a command like `python3 -m pip install opentldr` please make sure that you need to modify this library directly before using this codebase.
 
 ## KnowledgeGraph
 
 OpenTLDR uses a neo4j graph database as the storage layer of its KnowledgeGraph. The default (and easiest) way to do this is to run the Community Edition neo4j Server in a Docker container on the local machine that you execute OpenTLDR workflows. A linux shell script (start_neo4j.sh) and docker-compose configuraiton file (scripts/Neo4j/docker-compose) automate this process. The default container does not require authentication but only connects to localhost loopback interface. You can change all of this and use .env or system environment variables to direct the OpenTLDR library to use the desired neo4j server and user credientials.
@@ -73,16 +73,16 @@
    ...
     "repo_config": {'repo_type': 'files', 'path': './sample_data'}
     }
 </pre>
 
 Note that this format is likely to change to better support passing different parameters into individual steps.
 
-## ContentRepo
-The ContentRepo class provides an abstraction for locating data to use within the steps of the workflow. For example, in the above variables_to_set specification, there is a config json string `repo_config` that indicates to pull data from a directory of files located at the given path. At this time, only files and S3 buckets are implemented:
+## DataRepo
+The DataRepo class provides an abstraction for locating data to use within the steps of the workflow. For example, in the above variables_to_set specification, there is a config json string `repo_config` that indicates to pull data from a directory of files located at the given path. At this time, only files and S3 buckets are implemented:
 
 Config for using files, in this case from the local sample_data folder:
 <pre>
 repo_config = {
         'repo_type': 'files',
         'path': './sample_data'
         }
@@ -94,19 +94,19 @@
         'repo_type': 's3',
         'bucket': os.getenv("S3_BUCKET"),
         'aws_access_key_id': os.getenv("S3_ACCESS_KEY_ID"),
         'aws_secret_access_key': os.getenv("S3_SECRET_KEY")
         }
 </pre>
 
-Below is an example of using the ContentRepo to load news content from either of the above:
+Below is an example of using the DataRepo to load news content from either of the above:
 <pre>
-from opentldr import KnowledgeGraph, ContentRepo
+from opentldr import KnowledgeGraph, DataRepo
 
 kg = KnowledgeGraph()
-cr = ContentRepo(kg, repo_config)
+cr = DataRepo(kg, repo_config)
 
 for uid in cr.importContentData():
     print ("Loaded Content: {uid}".format(uid=uid))
 </pre>
-This will create a ContentRepo that writes to the KnowledgeGraph kg from the parsed Content configured above. The return value is a list of the uids of Content nodes created (note Source nodes would be created if needed but not returned here).
+This will create a DataRepo that writes to the KnowledgeGraph kg from the parsed Content configured above. The return value is a list of the uids of Content nodes created (note Source nodes would be created if needed but not returned here).
```

### Comparing `opentldr-0.3.0/pyproject.toml` & `opentldr-0.3.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ['setuptools>=61.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "opentldr"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Chris Argenta", email="cargenta@rockfishresearch.com" },
 ]
 description = "An open framework for creation of a Tailored Daily Report."
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers"
 ]
 dependencies = ['python-dotenv>=1.0.0','neo4j>=5.15.0','neomodel>=5.2.1','papermill>=2.5.0','boto3>=1.34.55']
 
 [project.urls]
-Source = "https://github.com/RockfishResearch/OpenTLDR"
-Issues = "https://github.com/RockfishResearch/OpenTLDR/issues"
+Source = "https://github.com/RockfishResearch/OpenTLDR-Core.git"
+Issues = "https://github.com/RockfishResearch/OpenTLDR-Core/issues"
 Documentation = "http://www.opentldr.org/docs"
 Homepage = "http://www.opentldr.org"
```

### Comparing `opentldr-0.3.0/src/opentldr/KnowledgeGraph.py` & `opentldr-0.3.1/src/opentldr/KnowledgeGraph.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,29 +3,27 @@
 
 import datetime
 
 from neo4j import GraphDatabase
 import neomodel as nm
 
 from opentldr.Domain import *
+from .log import log
 
-import logging
-logging.basicConfig(format='OpenTLDR Logging: %(message)s')
-_log=logging.getLogger("OpenTLDR")
 load_dotenv()
 
 def _getenv(variable:str , default:str):
         '''
         _getenv(variable, default) attempts to resolve the value of the environment variable specified.
         If it cannot find the variable in the OS or .env (from dotenv package) it will fail over to the
         provided default value while giving a warning to the logging system.
         '''
         value:str = os.getenv(variable)
         if value == None:
-            _log.warning("No environment variable '"+variable+"' so defaulting to '"+default+"'.")
+            log.warning("No environment variable '"+variable+"' so defaulting to '"+default+"'.")
             return default
         return value
 
 class KnowledgeGraph:
     '''
     KnowledgeGraph is the API for OpenTLDR's interface to Neo4j graph database. It attempts to make the
     driver connection using OS, .env, and then default values for connections. This API maps neo4j
@@ -64,22 +62,22 @@
             self.user=user
         if password is not None:
             self.password=password
         if database is not None:
             self.database=database
          
         if neo4j_driver is None:        
-            _log.info("Connecting to Neo4J using environment specification.")
-            _log.info("\tconnection:\t{v}".format(v=self.connection))
-            _log.info("\tuser:\t\t{v}".format(v=self.user))
-            #_log.info("\tpassword:\t{v}".format(v=self.password))
-            _log.info("\tdatabase:\t{v}".format(v=self.database))
+            log.info("Connecting to Neo4J using environment specification.")
+            log.info("\tconnection:\t{v}".format(v=self.connection))
+            log.info("\tuser:\t\t{v}".format(v=self.user))
+            #log.info("\tpassword:\t{v}".format(v=self.password))
+            log.info("\tdatabase:\t{v}".format(v=self.database))
             self.connect()
         else:
-            _log.info("Using Neo4j driver passed into initialization.")
+            log.info("Using Neo4j driver passed into initialization.")
             self.connect(neo4j_driver)
 
     def __del__(self):
         if self.driver is not None:
             self.driver.close()
 
     def __enter__(self):
@@ -99,20 +97,20 @@
         Use this if you are following neo4j documentation, otherwise use cypher_query().
         '''
         if self.driver == None:
             self.connect()
 
         try:
             records, summary, keys = self.driver.execute_query(cql, database_=self.database,)
-            _log.info("The query `{query}` returned {records_count} records in {time} ms.".format(
+            log.info("The query `{query}` returned {records_count} records in {time} ms.".format(
                 query=summary.query, records_count=len(records),
                 time=summary.result_available_after))
             return records, summary
         except Exception as e:
-            _log.error(e)
+            log.error(e)
 
     def neomodel_query(self,cypher_query):
         '''
         performs a cypher query in the standard neomodel method, which will return a list of lists of neomodel.
         Use this if you are following Neomodel documentation, otherwise use cypher_query().
         '''
         if self.driver == None:
@@ -123,30 +121,30 @@
     def connect(self, driver=None):
         '''
         ensures that a connection to Neo4j has been established and is functioning.
         '''
         if driver==None:
             driver = GraphDatabase.driver(self.connection, auth=(self.user,self.password))
         
-        _log.info("Testing Neo4j Connectivity...")
+        log.info("Testing Neo4j Connectivity...")
         driver.verify_connectivity()
         
         if driver.verify_connectivity:
-            _log.info("Successfully connected to Neo4J server for KnowledgeGraph.")
+            log.info("Successfully connected to Neo4J server for KnowledgeGraph.")
         else:
-            _log.error("Unable to connect to Neo4J for KnowledgeGraph. Check that Neo4j server is running.")
+            log.error("Unable to connect to Neo4J for KnowledgeGraph. Check that Neo4j server is running.")
             return False
 
-        _log.info("Testing Neo4j Authentication...")
+        log.info("Testing Neo4j Authentication...")
         driver.verify_authentication()
         
         if driver.verify_authentication:
-            _log.info("Successfully logged into Neo4J server for KnowledgeGraph.")
+            log.info("Successfully logged into Neo4J server for KnowledgeGraph.")
         else:
-            _log.error("Unable to log in to Neo4J for KnowledgeGraph. Check that your user and password are correct.")
+            log.error("Unable to log in to Neo4J for KnowledgeGraph. Check that your user and password are correct.")
             return False
         
         self.driver=driver
         return True
     
     def getNeo4jDriver(self):
         '''
@@ -168,18 +166,32 @@
 
     def _ensure_saved(self,node:OpenTldrMeta):
         '''
         OpenTLDR objects all inherit from the OpenTldrMeta mixin class. They will be assigned a "uid" when they are saved.
         So, we can use this to determine if an object has been saved or not and respond appropriately.
         '''
         if node.uid is None:
-            _log.warn("Nodes must be persisted with node.save() before being connected. Forcing this now.")
+            log.warn("Nodes must be persisted with node.save() before being connected. Forcing this now.")
             return node.save()
         return node
 
+
+    def get_all_node_uids_by_tag(self, tag:str ) -> list[str]:
+        '''
+        returns the list of uids for the tag specified as a string.
+        '''
+        return self.cypher_query("MATCH (n:{tag}) RETURN n.uid".format(tag=tag))
+
+    def get_all_nodes_by_tag(self, tag:str ):
+        '''
+        returns the list of uids for the tag specified as a string.
+        '''
+        return self.cypher_query("MATCH (n:{tag}) RETURN n".format(tag=tag),"n")
+
+
 # -----------------
 # KnowedgeGraph API 
 # -----------------
 
     def cypher_query(self,cypher_query,extract_variable=None) ->list:
         '''
         performs a cypher query and returns a single simple list of Neomodel objects based on the variable indicated (or first).
@@ -193,15 +205,15 @@
         results, meta = nm.db.cypher_query(cypher_query, resolve_objects = True)
         
         index=0
         if extract_variable is not None:
             index=meta.index(extract_variable)
         else:
             if len(meta)>1:
-                _log.warn("cypher_query is defaulting to return the first element of multiple return values in results.")       
+                log.warn("cypher_query is defaulting to return the first element of multiple return values in results.")       
         
         return [item[index] for item in results]
 
     def cypher_query_one(self,cypher_query,extract_variable=None):
         '''
         performs a query that is intended to LIMIT the return values to one single Neomodel object. This simplifies the processing
         of the query results to consistently only get a single object for the extract_variable, it is undefined which unless you sort them.
@@ -219,47 +231,53 @@
     def cypher_import(self,filename):
         '''
         processes a text file containing cypher commands and executes them on the KnowledgeGraph.
         '''
         count=0
         with open(filename) as fp:
             lines = fp.readlines()
-            for line in lines:    
+            for line in lines:
+                if len(line.strip()) == 0:
+                    continue;   
                 with self.driver.session() as session:
                     session.run(line)
                 count=count+1
-        _log.info("Imported {count} lines of Cypher from {filename}".format(count=count, filename=filename))
+        log.info("Imported {count} lines of Cypher from {filename}".format(count=count, filename=filename))
 
     def delete_all(self):
         '''
         clears the neo4j graph database.
         '''
         self.cypher_query("MATCH(x) DETACH DELETE x")
 
     def shortest_path(self,start:OpenTldrMeta,end:OpenTldrMeta):
         '''
         this is a special cypher command to run neo4j's shortest path algorithm and return the path (list of edges) found.
-        We remove Recommendation, Tldr, Source, and User nodes to avoid irrelevant paths that circumvent Reference Data.
+        We remove EvalKey, Recommendation, Tldr, Source, and User nodes to avoid irrelevant paths that circumvent Reference Data.
         '''
         results,meta = self.neomodel_query("""
             MATCH path=shortestPath((s)-[*..10]-(e))
             WHERE s.uid='{start_id}'
             AND e.uid='{end_id}'                         
             AND NONE(n IN nodes(path) WHERE 'Recommendation' IN LABELS(n))
             AND NONE(n IN nodes(path) WHERE 'Tldr' IN LABELS(n))
             AND NONE(n IN nodes(path) WHERE 'Source' IN LABELS(n))
             AND NONE(n IN nodes(path) WHERE 'User' IN LABELS(n))
+            AND NONE(n IN nodes(path) WHERE 'EvalKey' IN LABELS(n))
             RETURN path
             """.format(start_id=start.uid, end_id=end.uid))    
                      
         if len(results) == 0:
             return None
         else:
             return results[0][meta.index("path")]
 
+    def get_by_uid(self, uid:str):
+        return self.cypher_query_one("MATCH (n) WHERE n.uid='{uid}' RETURN n".format(uid=uid))
+
 # -----------------
 # Reference Data API
 # -----------------
 
 ## Reference Nodes in KG these are labeled as ReferenceNode
          
     def add_reference_node(self, text:str, type:str, hypothesized:bool=False) -> ReferenceNode:
@@ -349,15 +367,15 @@
         '''
         creates new source node, or if one by the same name already exists it reuses it.
         '''
         source = Source.nodes.get_or_none(name=name)
         if source is None:
             source= Source(name=name).save()
         else:
-            _log.warn("Found existing Source node for name {name}, returning pre-existing node.".format(name=name))
+            log.warn("Found existing Source node for name {name}, returning pre-existing node.".format(name=name))
         return source
     
     def update_source(self, node:Source) -> Source:
         '''
         updates the KG with changes to a Source properties
         '''
         return node.save()
@@ -393,37 +411,42 @@
 
     def add_content(self, source:Source, type:str, url:str, date:datetime.date, title:str, text:str) -> Content:
         content = Content.nodes.get_or_none(url=url)
         if content is None:
             content=Content(url=url,date=date,title=title,text=text, type=type).save()
             content.is_from.connect(source)
         else:
-            _log.warn("Found existing Content node for url {url}, returning pre-existing node.".format(url=url))
+            log.warn("Found existing Content node for url {url}, returning pre-existing node.".format(url=url))
         return content
 
     def get_all_content(self) -> list[Content]:
         content = Content.nodes
         return content
 
     def get_content_by_uid(self, uid:str) -> Content:
         content = Content.nodes.get_or_none(uid=uid)
         return content
 
     def get_content_by_url(self, url:str) -> Content:
         content = Content.nodes.get_or_none(url=url)
         return content
 
-    def get_content_for_source(self,source:Source) -> list[Content]:
+    def get_content_by_source(self,source:Source) -> list[Content]:
         return source.get_content()
     
-    def get_content_for_date(self,date:datetime.date) -> list[Content]:
+    def get_content_by_date(self,date:datetime.date) -> list[Content]:
         content = Content.nodes.get_or_none(date=date)
         return content
     
-    def get_content_for_recommendation(self,recommendation:Recommendation) -> list[Content]:
+    def get_content_by_title(self,title:str) -> Request:
+       return self.cypher_query_one("""
+            MATCH (c:Content) WHERE c.title='{title}'
+            RETURN c """.format(title=title),"c")
+    
+    def get_content_by_recommendation(self,recommendation:Recommendation) -> list[Content]:
         return recommendation.get_content()
     
 # Active Data / Entity
     
     def add_entity(self, content:Content, text:str, type:str ) -> Entity:
         entity=Entity(text=text,type=type).save()
         entity.mentioned_in.connect(content)
@@ -463,15 +486,15 @@
 # Users
 
     def add_user(self, name:str, email:str) -> User:
         user = User.nodes.get_or_none(name=name)
         if user is None:
             user=User(name=name, email=email).save()
         else:
-            _log.warn("Found existing User node for name {name}, returning pre-existing node.".
+            log.warn("Found existing User node for name {name}, returning pre-existing node.".
                       format(name=name))
         return user      
 
     def get_user_by_uid(self,uid:str) -> User:
         user = User.nodes.get_or_none(uid=uid)
         return user
 
@@ -484,15 +507,15 @@
     
     def add_request(self, title:str, text:str, user:User) -> Request:
         request = Request.nodes.get_or_none(title=title)
         if request is None or request.requested_by.single().uid != user.uid:
             request = Request(title=title, text=text).save()
             request.requested_by.connect(user)
         else:
-            _log.warn("Found existing Request node for {title}, returning pre-existing node.".format(title=title))
+            log.warn("Found existing Request node for {title}, returning pre-existing node.".format(title=title))
         return request
 
     def get_request_by_uid(self, uid:str) -> Request:
         request = Request.nodes.get_or_none(uid=uid)
         return request
 
     def get_request(self, name:str) -> Request:
@@ -506,14 +529,19 @@
     def get_requests_by_user(self,user:User) -> list[Request]:
        return self.cypher_query("""
             MATCH (u:User) WHERE u.uid='{user_id}'
             MATCH (q:Request)
             MATCH (q)-[y:REQUESTED_BY]->(u)
             RETURN q """.format(
                 user_id=user.uid),"q")
+    
+    def get_request_by_title(self,title:str) -> Request:
+       return self.cypher_query_one("""
+            MATCH (q:Request) WHERE q.title='{title}'
+            RETURN q """.format(title=title),"q")
 
     def get_entities_by_request(self,request:Request) -> list[Entity]:
         return self.cypher_query("""
             MATCH (r:Request) WHERE r.uid='{request_uid}'
             MATCH (e:Entity)
             MATCH (e)-[y:MENTIONED_IN]->(r)
             RETURN e """.format(
@@ -523,25 +551,25 @@
 # Workflow Products API 
 # -----------------
 
 # Recommedations
     
     def add_recommendation(self, score:float, content:Content, request:Request) -> Recommendation:
         if content.uid is None or request.uid is None:
-            _log.error("Adding Recommendation requires an existing and saved Content and Request node. Attempting to save them...")
+            log.error("Adding Recommendation requires an existing and saved Content and Request node. Attempting to save them...")
             content.save()
             request.save()
         
         recommendation = self.get_recommendation(content,request)
         if recommendation is None:
             recommendation= Recommendation(score=score).save()
             recommendation.recommends.connect(content)
             recommendation.relates_to.connect(request)
         else:
-            _log.warn("Found existing Recommendation node between content and request, returning pre-existing node.")
+            log.warn("Found existing Recommendation node between content and request, returning pre-existing node.")
         return recommendation
     
     def get_recommendation_by_id(self, uid:str) -> Recommendation:
         recommendation = Recommendation.nodes.get_or_none(uid=uid)
         return recommendation
 
     def get_recommendation(self, content:Content, request:Request) -> Recommendation:      
@@ -561,15 +589,15 @@
     def delete_all_recommendations(self):
         self.cypher_query("MATCH (r:Recommendation) DETACH DELETE (r)")
          
     def get_all_recommendations(self) -> list[Recommendation]:
         recommendations = Recommendation.nodes
         return recommendations
     
-    def get_recommendations_for_request(self,request:Request) -> list[Recommendation]:
+    def get_recommendations_by_request(self,request:Request) -> list[Recommendation]:
         return self.cypher_query("""
             MATCH (q:Request) WHERE q.uid='{request_id}'
             MATCH (r:Recommendation)
             MATCH (r)-[y:RELATES_TO]->(q)
             RETURN r ORDER BY r.score DESC """.format(
                 request_id=request.uid),"r")
 
@@ -579,15 +607,15 @@
         summary = self.get_summary(content,recommendation)
         if summary is None:
             summary= Summary(text=text).save()
             summary.summarizes.connect(content)
             if recommendation is not None:
                 summary.focus_on.connect(recommendation)
         else:
-            _log.warn("Found existing Summary node, returning pre-existing node.")
+            log.warn("Found existing Summary node, returning pre-existing node.")
         return summary
     
     def get_summary_by_id(self, uid:str) -> Summary:
         summary = Summary.nodes.get_or_none(uid=uid)
         return summary
 
     def get_summary(self, content:Content, recommendation:Recommendation) -> Summary:      
@@ -623,37 +651,37 @@
     
     def add_tldr(self, request:Request, date:datetime.date) -> Tldr:
         tldr = self.get_tldr(request, date)
         if tldr is None:
             tldr= Tldr(date=date).save()
             tldr.response_to.connect(request)
         else:
-            _log.warn("Found existing Tldr node for request on given date, returning pre-existing node.")
+            log.warn("Found existing Tldr node for request on given date, returning pre-existing node.")
         return tldr
     
     def add_entry_to_tldr(self, tldr:Tldr, score:float, recommendation:Recommendation, summary:Summary, content:Content) -> TldrEntry:
         tldr_entry=TldrEntry(link=content.url).save()
         tldr_entry.includes.connect(summary)
         tldr_entry.based_on.connect(recommendation)
-        tldr.priority.connect(tldr_entry, {'score': score })
+        tldr.contains.connect(tldr_entry, {'score': score })
 
     def get_tldr_by_id(self, uid:str) -> Tldr:
         tldr = Tldr.nodes.get_or_none(uid=uid)
         return tldr
 
     def delete_tldr_entry(self, tldr_entry:TldrEntry):
         tldr_entry.delete()
 
     def delete_tldr(self, tldr:Tldr):
-        for tldr_entry in tldr.priority.all():
+        for tldr_entry in tldr.contains.all():
             self.delete_tldr_entry(tldr_entry)
         tldr.delete()
 
     def delete_tldr_entries_by_tldr(self, tldr:Tldr):
-        for tldr_entry in tldr.priority.all():
+        for tldr_entry in tldr.contains.all():
             self.delete_tldr_entry(tldr_entry)
 
     def delete_all_tldrs(self):
         for tldr in Tldr.nodes:
             self.delete_tldr(tldr)
 
     def get_tldrs_by_date(self, date:datetime.date):
@@ -674,15 +702,15 @@
         tldrs = Tldr.nodes
         return tldrs
     
     def get_entries_by_tldr(self, tldr:Tldr) -> list[TldrEntry]:
         return self.cypher_query("""
             MATCH (t:Tldr) WHERE t.uid='{tldr_id}'
             MATCH (e:TldrEntry)
-            MATCH (t)-[x:PRIORITY]->(e)
+            MATCH (t)-[x:CONTAINS]->(e)
             RETURN e ORDER BY e.score DESC""".format(tldr_id=tldr.uid),"e")                 
 
     def get_tldr_by_request(self,request:Request) -> list[Tldr]:
         return self.cypher_query("""
             MATCH (q:Request) WHERE q.uid='{request_id}'
             MATCH (t:Tldr)
             MATCH (t)-[y:RESPONSE_TO]->(q)
@@ -694,7 +722,43 @@
             MATCH (q:Request) WHERE q.uid='{request_id}'
             MATCH (t:Tldr) where t.date='{date}'
             MATCH (t)-[y:RESPONSE_TO]->(q)
             RETURN t """.format( date=date,
                 request_id=request.uid),"t")
 
 
+## EvalKey Nodes - rubric for evaluation metrics
+
+    def add_evalkey(self, content:Source, request:Request, score:float, text:str) -> EvalKey:
+        evalkey = EvalKey.nodes.get_or_none(url=url)
+        if content is None:
+            content=Content(url=url,date=date,title=title,text=text, type=type).save()
+            content.is_from.connect(source)
+        else:
+            log.warn("Found existing Content node for url {url}, returning pre-existing node.".format(url=url))
+        return content
+
+    def get_all_evalkeys(self) -> list[EvalKey]:
+        evalkeys = EvalKey.nodes
+        return evalkeys
+
+    def get_evalkey_by_uid(self, uid:str) -> Content:
+        content = Content.nodes.get_or_none(uid=uid)
+        return content
+
+    def get_evalkeys_by_content(self, url:str) -> Content:
+        content = Content.nodes.get_or_none(url=url)
+        return content
+    
+    def get_evalkeys_by_request(self,date:datetime.date) -> list[Content]:
+        content = Content.nodes.get_or_none(date=date)
+        return content
+    
+    def get_evalkey_by_content_and_request(self, content:Content, request:Request) -> EvalKey:
+        return self.cypher_query_one("""
+            MATCH (c:Content) WHERE c.uid='{content_id}'
+            MATCH (q:Request) WHERE q.uid='{request_id}'
+            MATCH (c)<-[ec:KEY_FOR_CONTENT]-(e:EvalKey)-[eq:KEY_FOR_REQUEST]->(q)
+            RETURN e """.format( content_id=content.uid, request_id=request.uid),"e")
+
+    def delete_all_evalkeys(self):
+        self.cypher_query("MATCH (r:EvalKey) DETACH DELETE (r)")
```

### Comparing `opentldr-0.3.0/src/opentldr.egg-info/PKG-INFO` & `opentldr-0.3.1/src/opentldr.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: opentldr
-Version: 0.3.0
+Version: 0.3.1
 Summary: An open framework for creation of a Tailored Daily Report.
 Author-email: Chris Argenta <cargenta@rockfishresearch.com>
-Project-URL: Source, https://github.com/RockfishResearch/OpenTLDR
-Project-URL: Issues, https://github.com/RockfishResearch/OpenTLDR/issues
+Project-URL: Source, https://github.com/RockfishResearch/OpenTLDR-Core.git
+Project-URL: Issues, https://github.com/RockfishResearch/OpenTLDR-Core/issues
 Project-URL: Documentation, http://www.opentldr.org/docs
 Project-URL: Homepage, http://www.opentldr.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-dotenv>=1.0.0
 Requires-Dist: neo4j>=5.15.0
 Requires-Dist: neomodel>=5.2.1
 Requires-Dist: papermill>=2.5.0
 Requires-Dist: boto3>=1.34.55
@@ -30,15 +30,15 @@
 
 OpenTLDR is an open source framework written in Python to implement the process of creating a Tailored Daily Report from a series of news-like articles. This repository contains the Core classes used as a library by OpenTLDR implementations, like the example notebooks you canf ind in the OpenTLDR-Example repo on GitHub.
 
 OpenTLDR is composed of Python modules:
 - A **KnowledgeGraph** modulethat has been implemented as a layer on top of the Neo4j Graph Database
 - A module with a set of **Domain** classes that implement the nodes and edges in a TLDR-focused knowledge graph
 - A **Workflow** module and tool that wraps the execution of a series of Python Notebooks to make them behave like components
-- A **ContentRepo** module that abstracts the data ingest from Python Notebooks using a config parameter for either S3 or Files
+- A **DataRepo** module that abstracts the data ingest from Python Notebooks using a config parameter for either S3 or Files
 
 This GitHub repo handles the back-end code that and is only required if you with to modify this functionality directly. Otherwise, you should use the OpenTDLR-Example repository, which implements analytic pieces of the process in a series of Jupyter Notebooks. All of the code in this repo is availible
 to Python code as a pip library using a command like `python3 -m pip install opentldr` please make sure that you need to modify this library directly before using this codebase.
 
 ## KnowledgeGraph
 
 OpenTLDR uses a neo4j graph database as the storage layer of its KnowledgeGraph. The default (and easiest) way to do this is to run the Community Edition neo4j Server in a Docker container on the local machine that you execute OpenTLDR workflows. A linux shell script (start_neo4j.sh) and docker-compose configuraiton file (scripts/Neo4j/docker-compose) automate this process. The default container does not require authentication but only connects to localhost loopback interface. You can change all of this and use .env or system environment variables to direct the OpenTLDR library to use the desired neo4j server and user credientials.
@@ -96,16 +96,16 @@
    ...
     "repo_config": {'repo_type': 'files', 'path': './sample_data'}
     }
 </pre>
 
 Note that this format is likely to change to better support passing different parameters into individual steps.
 
-## ContentRepo
-The ContentRepo class provides an abstraction for locating data to use within the steps of the workflow. For example, in the above variables_to_set specification, there is a config json string `repo_config` that indicates to pull data from a directory of files located at the given path. At this time, only files and S3 buckets are implemented:
+## DataRepo
+The DataRepo class provides an abstraction for locating data to use within the steps of the workflow. For example, in the above variables_to_set specification, there is a config json string `repo_config` that indicates to pull data from a directory of files located at the given path. At this time, only files and S3 buckets are implemented:
 
 Config for using files, in this case from the local sample_data folder:
 <pre>
 repo_config = {
         'repo_type': 'files',
         'path': './sample_data'
         }
@@ -117,19 +117,19 @@
         'repo_type': 's3',
         'bucket': os.getenv("S3_BUCKET"),
         'aws_access_key_id': os.getenv("S3_ACCESS_KEY_ID"),
         'aws_secret_access_key': os.getenv("S3_SECRET_KEY")
         }
 </pre>
 
-Below is an example of using the ContentRepo to load news content from either of the above:
+Below is an example of using the DataRepo to load news content from either of the above:
 <pre>
-from opentldr import KnowledgeGraph, ContentRepo
+from opentldr import KnowledgeGraph, DataRepo
 
 kg = KnowledgeGraph()
-cr = ContentRepo(kg, repo_config)
+cr = DataRepo(kg, repo_config)
 
 for uid in cr.importContentData():
     print ("Loaded Content: {uid}".format(uid=uid))
 </pre>
-This will create a ContentRepo that writes to the KnowledgeGraph kg from the parsed Content configured above. The return value is a list of the uids of Content nodes created (note Source nodes would be created if needed but not returned here).
+This will create a DataRepo that writes to the KnowledgeGraph kg from the parsed Content configured above. The return value is a list of the uids of Content nodes created (note Source nodes would be created if needed but not returned here).
```

### Comparing `opentldr-0.3.0/tests/test_knowledgegraph.py` & `opentldr-0.3.1/tests/test_knowledgegraph.py`

 * *Files identical despite different names*

