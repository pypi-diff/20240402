# Comparing `tmp/langchain_google_cloud_sql_pg-0.2.0-py3-none-any.whl.zip` & `tmp/langchain_google_cloud_sql_pg-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 29499 bytes, number of entries: 13
--rw-r--r--  2.0 unx     1034 b- defN 24-Mar-27 18:14 langchain_google_cloud_sql_pg/__init__.py
--rw-r--r--  2.0 unx     4964 b- defN 24-Mar-27 18:14 langchain_google_cloud_sql_pg/chat_message_history.py
--rw-r--r--  2.0 unx    14432 b- defN 24-Mar-27 18:14 langchain_google_cloud_sql_pg/engine.py
--rw-r--r--  2.0 unx     2580 b- defN 24-Mar-27 18:14 langchain_google_cloud_sql_pg/indexes.py
--rw-r--r--  2.0 unx    17740 b- defN 24-Mar-27 18:14 langchain_google_cloud_sql_pg/loader.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Mar-27 18:14 langchain_google_cloud_sql_pg/py.typed
--rw-r--r--  2.0 unx    29629 b- defN 24-Mar-27 18:14 langchain_google_cloud_sql_pg/vectorstore.py
--rw-r--r--  2.0 unx      622 b- defN 24-Mar-27 18:14 langchain_google_cloud_sql_pg/version.py
--rw-rw-r--  2.0 unx    11358 b- defN 24-Mar-27 18:16 langchain_google_cloud_sql_pg-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    18749 b- defN 24-Mar-27 18:16 langchain_google_cloud_sql_pg-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-27 18:16 langchain_google_cloud_sql_pg-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       30 b- defN 24-Mar-27 18:16 langchain_google_cloud_sql_pg-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1287 b- defN 24-Mar-27 18:16 langchain_google_cloud_sql_pg-0.2.0.dist-info/RECORD
-13 files, 102517 bytes uncompressed, 27283 bytes compressed:  73.4%
+Zip file size: 28147 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     1034 b- defN 24-Apr-02 18:58 langchain_google_cloud_sql_pg/__init__.py
+-rw-r--r--  2.0 unx     4964 b- defN 24-Apr-02 18:58 langchain_google_cloud_sql_pg/chat_message_history.py
+-rw-r--r--  2.0 unx    14432 b- defN 24-Apr-02 18:58 langchain_google_cloud_sql_pg/engine.py
+-rw-r--r--  2.0 unx     2580 b- defN 24-Apr-02 18:58 langchain_google_cloud_sql_pg/indexes.py
+-rw-r--r--  2.0 unx    17740 b- defN 24-Apr-02 18:58 langchain_google_cloud_sql_pg/loader.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-02 18:58 langchain_google_cloud_sql_pg/py.typed
+-rw-r--r--  2.0 unx    29570 b- defN 24-Apr-02 18:58 langchain_google_cloud_sql_pg/vectorstore.py
+-rw-r--r--  2.0 unx      622 b- defN 24-Apr-02 18:58 langchain_google_cloud_sql_pg/version.py
+-rw-rw-r--  2.0 unx    11358 b- defN 24-Apr-02 19:00 langchain_google_cloud_sql_pg-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    14684 b- defN 24-Apr-02 19:00 langchain_google_cloud_sql_pg-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-02 19:00 langchain_google_cloud_sql_pg-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       30 b- defN 24-Apr-02 19:00 langchain_google_cloud_sql_pg-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1287 b- defN 24-Apr-02 19:00 langchain_google_cloud_sql_pg-0.3.0.dist-info/RECORD
+13 files, 98393 bytes uncompressed, 25931 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: langchain_google_cloud_sql_pg/vectorstore.py
 Comment: 
 
 Filename: langchain_google_cloud_sql_pg/version.py
 Comment: 
 
-Filename: langchain_google_cloud_sql_pg-0.2.0.dist-info/LICENSE
+Filename: langchain_google_cloud_sql_pg-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: langchain_google_cloud_sql_pg-0.2.0.dist-info/METADATA
+Filename: langchain_google_cloud_sql_pg-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: langchain_google_cloud_sql_pg-0.2.0.dist-info/WHEEL
+Filename: langchain_google_cloud_sql_pg-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: langchain_google_cloud_sql_pg-0.2.0.dist-info/top_level.txt
+Filename: langchain_google_cloud_sql_pg-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: langchain_google_cloud_sql_pg-0.2.0.dist-info/RECORD
+Filename: langchain_google_cloud_sql_pg-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langchain_google_cloud_sql_pg/vectorstore.py

```diff
@@ -91,24 +91,22 @@
         k: int = 4,
         fetch_k: int = 20,
         lambda_mult: float = 0.5,
         index_query_options: Optional[QueryOptions] = None,
     ):
         """Constructor for PostgresVectorStore.
         Args:
-            engine (PostgresEngine): AsyncEngine with pool connection to the postgres database. Required.
+            engine (PostgresEngine): Connection pool engine for managing connections to Cloud SQL for PostgreSQL database.
             embedding_service (Embeddings): Text embedding model to use.
-            table_name (str): Name of the existing table or the table to be created.
-            id_column (str): Column that represents the Document's id. Defaults to "langchain_id".
-            content_column (str): Column that represent a Document’s page_content. Defaults to "content".
-            embedding_column (str): Column for embedding vectors.
-                              The embedding is generated from the document value. Defaults to "embedding".
+            table_name (str): Name of an existing table or table to be created.
+            content_column (str): Column that represent a Document's page_content. Defaults to "content".
+            embedding_column (str): Column for embedding vectors. The embedding is generated from the document value. Defaults to "embedding".
             metadata_columns (List[str]): Column(s) that represent a document's metadata.
-            ignore_metadata_columns (List[str]): Column(s) to ignore in pre-existing tables for a document’s metadata.
-                                     Can not be used with metadata_columns. Defaults to None.
+            ignore_metadata_columns (List[str]): Column(s) to ignore in pre-existing tables for a document's metadata. Can not be used with metadata_columns. Defaults to None.
+            id_column (str): Column that represents the Document's id. Defaults to "langchain_id".
             metadata_json_column (str): Column to store metadata as JSON. Defaults to "langchain_metadata".
         """
         if metadata_columns and ignore_metadata_columns:
             raise ValueError(
                 "Can not use both metadata_columns and ignore_metadata_columns."
             )
         # Get field type information
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## langchain_google_cloud_sql_pg/version.py

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.2.0"
+__version__ = "0.3.0"
```

## Comparing `langchain_google_cloud_sql_pg-0.2.0.dist-info/LICENSE` & `langchain_google_cloud_sql_pg-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langchain_google_cloud_sql_pg-0.2.0.dist-info/METADATA` & `langchain_google_cloud_sql_pg-0.3.0.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-google-cloud-sql-pg
-Version: 0.2.0
+Version: 0.3.0
 Summary: LangChain integrations for Google Cloud SQL for PostgreSQL
 Author-email: Google LLC <googleapis-packages@google.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -206,14 +206,23 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/googleapis/langchain-google-cloud-sql-pg-python
 Project-URL: Repository, https://github.com/googleapis/langchain-google-cloud-sql-pg-python.git
 Project-URL: Bug Tracker, https://github.com/googleapis/langchain-google-cloud-sql-pg-python/issues
 Project-URL: Changelog, https://github.com/googleapis/langchain-google-cloud-sql-pg-python/blob/main/CHANGELOG.md
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cloud-sql-python-connector[asyncpg] <2.0.0,>=1.7.0
 Requires-Dist: langchain-core <2.0.0,>=0.1.1
 Requires-Dist: langchain-community <0.1.0,>=0.0.18
 Requires-Dist: numpy <2.0.0,>=1.24.4
@@ -222,129 +231,7 @@
 Provides-Extra: test
 Requires-Dist: black[jupyter] ==23.12.1 ; extra == 'test'
 Requires-Dist: isort ==5.13.2 ; extra == 'test'
 Requires-Dist: mypy ==1.9.0 ; extra == 'test'
 Requires-Dist: pytest-asyncio ==0.23.5.post1 ; extra == 'test'
 Requires-Dist: pytest ==7.4.4 ; extra == 'test'
 
-# Cloud SQL for PostgreSQL for LangChain
-
-This package contains the [LangChain][langchain] integrations for Cloud SQL for PostgreSQL.
-
-> **🧪 Preview:** This feature is covered by the Pre-GA Offerings Terms of the Google Cloud Terms of Service. Please note that pre-GA products and features might have limited support, and changes to pre-GA products and features might not be compatible with other pre-GA versions. For more information, see the [launch stage descriptions](https://cloud.google.com/products#product-launch-stages)
-
-* [Documentation][docs]
-* [API Reference]()
-
-## Getting Started
-
-In order to use this library, you first need to go through the following steps:
-
-1. [Select or create a Cloud Platform project.][project]
-2. [Enable billing for your project.][billing]
-3. [Enable the Google Cloud SQL API.][api]
-4. [Setup Authentication.][auth]
-
-### Installation
-
-Install this library in a [`virtualenv`][venv] using pip. [`virtualenv`][venv] is a tool to
-create isolated Python environments. The basic problem it addresses is one of
-dependencies and versions, and indirectly permissions.
-
-With [`virtualenv`][venv], it's possible to install this library without needing system
-install permissions, and without clashing with the installed system
-dependencies.
-
-```bash
-pip install virtualenv
-virtualenv <your-env>
-source <your-env>/bin/activate
-<your-env>/bin/pip install langchain-google-cloud-sql-pg
-```
-
-## Vector Store Usage
-
-Use a vector store to store embedded data and perform vector search.
-
-```python
-from langchain_google_cloud_sql_pg import PostgresVectorstore, PostgresEngine
-from langchain.embeddings import VertexAIEmbeddings
-
-
-engine = PostgresEngine.from_instance("project-id", "region", "my-instance", "my-database")
-embeddings_service = VertexAIEmbeddings()
-vectorstore = PostgresVectorStore(
-    engine,
-    table_name="my-table",
-    embeddings=embedding_service
-)
-```
-
-See the full [Vector Store][vectorstore] tutorial.
-
-## Document Loader Usage
-
-Use a document loader to load data as LangChain `Document`s.
-
-```python
-from langchain_google_cloud_sql_pg import PostgresEngine, PostgresLoader
-
-
-engine = PostgresEngine.from_instance("project-id", "region", "my-instance", "my-database")
-loader = PostgresSQLLoader(
-    engine,
-    table_name="my-table-name"
-)
-docs = loader.lazy_load()
-```
-
-See the full [Document Loader][loader] tutorial.
-
-## Chat Message History Usage
-
-Use `ChatMessageHistory` to store messages and provide conversation history to LLMs.
-
-```python
-from langchain_google_cloud_sql_pg import PostgresChatMessageHistory, PostgresEngine
-
-
-engine = PostgresEngine.from_instance("project-id", "region", "my-instance", "my-database")
-history = PostgresChatMessageHistory(
-    engine,
-    table_name="my-message-store",
-    session_id="my-session_id"
-)
-```
-
-See the full [Chat Message History][history] tutorial.
-
-## Contributing
-
-Contributions to this library are always welcome and highly encouraged.
-
-See [CONTRIBUTING][contributing] for more information how to get started.
-
-Please note that this project is released with a Contributor Code of Conduct. By participating in
-this project you agree to abide by its terms. See [Code of Conduct][coc] for more
-information.
-
-## License
-
-Apache 2.0 - See [LICENSE][license] for more information.
-
-## Disclaimer
-
-This is not an officially supported Google product.
-
-[project]: https://console.cloud.google.com/project
-[billing]: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-[api]: https://console.cloud.google.com/flows/enableapi?apiid=sqladmin.googleapis.com
-[auth]: https://googleapis.dev/python/google-api-core/latest/auth.html
-[venv]: https://virtualenv.pypa.io/en/latest/
-[vectorstore]: https://github.com/googleapis/langchain-google-cloud-sql-pg-python/tree/main/docs/vector_store.ipynb
-[loader]: https://github.com/googleapis/langchain-google-cloud-sql-pg-python/tree/main/docs/document_loader.ipynb
-[history]: https://github.com/googleapis/langchain-google-cloud-sql-pg-python/tree/main/docs/chat_message_history.ipynb
-[langchain]: https://github.com/langchain-ai/langchain
-[docs]: https://github.com/googleapis/langchain-google-cloud-sql-pg-python/tree/main/docs
-[license]: https://github.com/googleapis/langchain-google-cloud-sql-pg-python/tree/main/LICENSE
-[contributing]: https://github.com/googleapis/langchain-google-cloud-sql-pg-python/tree/main/CONTRIBUTING.md
-[coc]: https://github.com/googleapis/langchain-google-cloud-sql-pg-python/tree/main/CODE_OF_CONDUCT.md
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

