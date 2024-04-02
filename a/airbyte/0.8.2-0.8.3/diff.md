# Comparing `tmp/airbyte-0.8.2.tar.gz` & `tmp/airbyte-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-0.8.2.tar", max compression
+gzip compressed data, was "airbyte-0.8.3.tar", max compression
```

## Comparing `airbyte-0.8.2.tar` & `airbyte-0.8.3.tar`

### file list

```diff
@@ -1,57 +1,56 @@
--rw-r--r--   0        0        0     3804 2024-03-28 22:08:57.339184 airbyte-0.8.2/LICENSE.md
--rw-r--r--   0        0        0     6191 2024-03-28 22:08:57.339184 airbyte-0.8.2/README.md
--rw-r--r--   0        0        0     1154 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/__init__.py
--rw-r--r--   0        0        0     2262 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/_batch_handles.py
--rw-r--r--   0        0        0    16354 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/_executor.py
--rw-r--r--   0        0        0        0 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/_processors/__init__.py
--rw-r--r--   0        0        0     9095 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/_processors/base.py
--rw-r--r--   0        0        0      352 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/_processors/file/__init__.py
--rw-r--r--   0        0        0     7510 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/_processors/file/base.py
--rw-r--r--   0        0        0      869 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/_processors/file/jsonl.py
--rw-r--r--   0        0        0       79 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/_processors/sql/__init__.py
--rw-r--r--   0        0        0    32880 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/_processors/sql/base.py
--rw-r--r--   0        0        0     8397 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/_processors/sql/bigquery.py
--rw-r--r--   0        0        0     3918 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/_processors/sql/duckdb.py
--rw-r--r--   0        0        0     1235 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/_processors/sql/motherduck.py
--rw-r--r--   0        0        0      837 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/_processors/sql/postgres.py
--rw-r--r--   0        0        0     3735 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/_processors/sql/snowflake.py
--rw-r--r--   0        0        0      420 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/_util/__init__.py
--rw-r--r--   0        0        0     3855 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/_util/document_rendering.py
--rw-r--r--   0        0        0     1854 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/_util/google_secrets.py
--rw-r--r--   0        0        0     3355 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/_util/meta.py
--rw-r--r--   0        0        0     7065 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/_util/name_normalizers.py
--rw-r--r--   0        0        0     1683 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/_util/pip_util.py
--rw-r--r--   0        0        0     3133 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/_util/protocol_util.py
--rw-r--r--   0        0        0    10605 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/_util/telemetry.py
--rw-r--r--   0        0        0      903 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/caches/__init__.py
--rw-r--r--   0        0        0    10139 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/caches/_catalog_manager.py
--rw-r--r--   0        0        0     3775 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/caches/base.py
--rw-r--r--   0        0        0     1882 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/caches/bigquery.py
--rw-r--r--   0        0        0     1947 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/caches/duckdb.py
--rw-r--r--   0        0        0      471 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/caches/generic.py
--rw-r--r--   0        0        0     1169 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/caches/motherduck.py
--rw-r--r--   0        0        0     1213 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/caches/postgres.py
--rw-r--r--   0        0        0     1627 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/caches/snowflake.py
--rw-r--r--   0        0        0     1998 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/caches/util.py
--rw-r--r--   0        0        0      346 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/datasets/__init__.py
--rw-r--r--   0        0        0     2212 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/datasets/_base.py
--rw-r--r--   0        0        0      917 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/datasets/_lazy.py
--rw-r--r--   0        0        0      819 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/datasets/_map.py
--rw-r--r--   0        0        0     5481 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/datasets/_sql.py
--rw-r--r--   0        0        0     1861 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/documents.py
--rw-r--r--   0        0        0     9245 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/exceptions.py
--rw-r--r--   0        0        0    13834 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/progress.py
--rw-r--r--   0        0        0        0 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/py.typed
--rw-r--r--   0        0        0     1580 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/results.py
--rw-r--r--   0        0        0     3519 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/secrets.py
--rw-r--r--   0        0        0      517 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/sources/__init__.py
--rw-r--r--   0        0        0    28433 2024-03-28 22:08:57.339184 airbyte-0.8.2/airbyte/sources/base.py
--rw-r--r--   0        0        0     3718 2024-03-28 22:08:57.343184 airbyte-0.8.2/airbyte/sources/registry.py
--rw-r--r--   0        0        0     5516 2024-03-28 22:08:57.343184 airbyte-0.8.2/airbyte/sources/util.py
--rw-r--r--   0        0        0      987 2024-03-28 22:08:57.343184 airbyte-0.8.2/airbyte/strategies.py
--rw-r--r--   0        0        0     4733 2024-03-28 22:08:57.343184 airbyte-0.8.2/airbyte/types.py
--rw-r--r--   0        0        0     5423 2024-03-28 22:08:57.343184 airbyte-0.8.2/airbyte/validate.py
--rw-r--r--   0        0        0      232 2024-03-28 22:08:57.343184 airbyte-0.8.2/airbyte/version.py
--rw-r--r--   0        0        0      369 2024-03-28 22:08:57.343184 airbyte-0.8.2/airbyte/warnings.py
--rw-r--r--   0        0        0     8366 2024-03-28 22:09:08.591331 airbyte-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     7582 1970-01-01 00:00:00.000000 airbyte-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     3804 2024-04-02 00:35:03.698301 airbyte-0.8.3/LICENSE.md
+-rw-r--r--   0        0        0     6176 2024-04-02 00:35:03.698301 airbyte-0.8.3/README.md
+-rw-r--r--   0        0        0     1154 2024-04-02 00:35:03.698301 airbyte-0.8.3/airbyte/__init__.py
+-rw-r--r--   0        0        0     2262 2024-04-02 00:35:03.698301 airbyte-0.8.3/airbyte/_batch_handles.py
+-rw-r--r--   0        0        0    16354 2024-04-02 00:35:03.698301 airbyte-0.8.3/airbyte/_executor.py
+-rw-r--r--   0        0        0        0 2024-04-02 00:35:03.698301 airbyte-0.8.3/airbyte/_processors/__init__.py
+-rw-r--r--   0        0        0     9095 2024-04-02 00:35:03.698301 airbyte-0.8.3/airbyte/_processors/base.py
+-rw-r--r--   0        0        0      352 2024-04-02 00:35:03.698301 airbyte-0.8.3/airbyte/_processors/file/__init__.py
+-rw-r--r--   0        0        0     7496 2024-04-02 00:35:03.698301 airbyte-0.8.3/airbyte/_processors/file/base.py
+-rw-r--r--   0        0        0      928 2024-04-02 00:35:03.698301 airbyte-0.8.3/airbyte/_processors/file/jsonl.py
+-rw-r--r--   0        0        0       79 2024-04-02 00:35:03.698301 airbyte-0.8.3/airbyte/_processors/sql/__init__.py
+-rw-r--r--   0        0        0    32880 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/_processors/sql/base.py
+-rw-r--r--   0        0        0     8397 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/_processors/sql/bigquery.py
+-rw-r--r--   0        0        0     3949 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/_processors/sql/duckdb.py
+-rw-r--r--   0        0        0     1235 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/_processors/sql/motherduck.py
+-rw-r--r--   0        0        0      837 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/_processors/sql/postgres.py
+-rw-r--r--   0        0        0     3762 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/_processors/sql/snowflake.py
+-rw-r--r--   0        0        0      420 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/_util/__init__.py
+-rw-r--r--   0        0        0     3855 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/_util/document_rendering.py
+-rw-r--r--   0        0        0     1854 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/_util/google_secrets.py
+-rw-r--r--   0        0        0     3355 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/_util/meta.py
+-rw-r--r--   0        0        0     6988 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/_util/name_normalizers.py
+-rw-r--r--   0        0        0     1683 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/_util/pip_util.py
+-rw-r--r--   0        0        0    10605 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/_util/telemetry.py
+-rw-r--r--   0        0        0      903 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/caches/__init__.py
+-rw-r--r--   0        0        0    10139 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/caches/_catalog_manager.py
+-rw-r--r--   0        0        0     3775 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/caches/base.py
+-rw-r--r--   0        0        0     1882 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/caches/bigquery.py
+-rw-r--r--   0        0        0     1947 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/caches/duckdb.py
+-rw-r--r--   0        0        0      471 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/caches/generic.py
+-rw-r--r--   0        0        0     1169 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/caches/motherduck.py
+-rw-r--r--   0        0        0     1213 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/caches/postgres.py
+-rw-r--r--   0        0        0     1627 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/caches/snowflake.py
+-rw-r--r--   0        0        0     1998 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/caches/util.py
+-rw-r--r--   0        0        0      346 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/datasets/__init__.py
+-rw-r--r--   0        0        0     2212 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/datasets/_base.py
+-rw-r--r--   0        0        0      917 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/datasets/_lazy.py
+-rw-r--r--   0        0        0      819 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/datasets/_map.py
+-rw-r--r--   0        0        0     5481 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/datasets/_sql.py
+-rw-r--r--   0        0        0     1861 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/documents.py
+-rw-r--r--   0        0        0     9245 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/exceptions.py
+-rw-r--r--   0        0        0    13834 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/progress.py
+-rw-r--r--   0        0        0        0 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/py.typed
+-rw-r--r--   0        0        0     1580 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/results.py
+-rw-r--r--   0        0        0     3519 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/secrets.py
+-rw-r--r--   0        0        0      517 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/sources/__init__.py
+-rw-r--r--   0        0        0    28443 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/sources/base.py
+-rw-r--r--   0        0        0     3718 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/sources/registry.py
+-rw-r--r--   0        0        0     5516 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/sources/util.py
+-rw-r--r--   0        0        0      987 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/strategies.py
+-rw-r--r--   0        0        0     4733 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/types.py
+-rw-r--r--   0        0        0     5423 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/validate.py
+-rw-r--r--   0        0        0      232 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/version.py
+-rw-r--r--   0        0        0      369 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/warnings.py
+-rw-r--r--   0        0        0     8366 2024-04-02 00:35:15.246369 airbyte-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     7567 1970-01-01 00:00:00.000000 airbyte-0.8.3/PKG-INFO
```

### Comparing `airbyte-0.8.2/LICENSE.md` & `airbyte-0.8.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/README.md` & `airbyte-0.8.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # PyAirbyte
 
-PyAirbyte brings the power of Airbyte to every Python developer. PyAirbyte provides a set of utilities to use Airbyte connectors in Python. It is meant to be used in situations where setting up an Airbyte server or cloud account is not possible or desirable. 
+PyAirbyte brings the power of Airbyte to every Python developer. PyAirbyte provides a set of utilities to use Airbyte connectors in Python. It is meant to be used in situations where setting up an Airbyte server or cloud account is not possible or desirable.
 
 - [Getting Started](#getting-started)
 - [Secrets Management](#secrets-management)
 - [Connector compatibility](#connector-compatibility)
 - [Contributing](#contributing)
 - [Frequently asked Questions](#frequently-asked-questions)
 
-## Getting Started 
+## Getting Started
 
-Watch this [Getting Started Loom video](https://www.loom.com/share/3de81ca3ce914feca209bf83777efa3f?sid=8804e8d7-096c-4aaa-a8a4-9eb93a44e850) or run one of our Quickstart tutorials below to see how you can use PyAirbyte in your python code. 
+Watch this [Getting Started Loom video](https://www.loom.com/share/3de81ca3ce914feca209bf83777efa3f?sid=8804e8d7-096c-4aaa-a8a4-9eb93a44e850) or run one of our Quickstart tutorials below to see how you can use PyAirbyte in your python code.
 
 * [Basic Demo](https://github.com/airbytehq/quickstarts/blob/main/pyairbyte_notebooks/PyAirbyte_Basic_Features_Demo.ipynb)
 * [CoinAPI](https://github.com/airbytehq/quickstarts/blob/main/pyairbyte_notebooks/PyAirbyte_CoinAPI_Demo.ipynb)
-* [GA4](https://github.com/airbytehq/quickstarts/blob/main/pyairbyte_notebooks/PyAirbyte_GA4_Demo.ipynb) 
-* [Shopify](https://github.com/airbytehq/quickstarts/blob/main/pyairbyte_notebooks/PyAirbyte_Shopify_Demo.ipynb) 
-* [GitHub](https://github.com/airbytehq/quickstarts/blob/main/pyairbyte_notebooks/PyAirbyte_Github_Incremental_Demo.ipynb) 
-* [Postgres (cache)](https://github.com/airbytehq/quickstarts/blob/main/pyairbyte_notebooks/PyAirbyte_Postgres_Custom_Cache_Demo.ipynb)  
+* [GA4](https://github.com/airbytehq/quickstarts/blob/main/pyairbyte_notebooks/PyAirbyte_GA4_Demo.ipynb)
+* [Shopify](https://github.com/airbytehq/quickstarts/blob/main/pyairbyte_notebooks/PyAirbyte_Shopify_Demo.ipynb)
+* [GitHub](https://github.com/airbytehq/quickstarts/blob/main/pyairbyte_notebooks/PyAirbyte_Github_Incremental_Demo.ipynb)
+* [Postgres (cache)](https://github.com/airbytehq/quickstarts/blob/main/pyairbyte_notebooks/PyAirbyte_Postgres_Custom_Cache_Demo.ipynb)
 
 
 ## Secrets Management
 
 PyAirbyte can auto-import secrets from the following sources:
 
 1. Environment variables.
@@ -32,15 +32,15 @@
 _Note: Additional secret store options may be supported in the future. [More info here.](https://github.com/airbytehq/airbyte-lib-private-beta/discussions/5)_
 
 ### Retrieving Secrets
 
 ```python
 from airbyte import get_secret, SecretSource
 
-source = get_connection("source-github")
+source = get_source("source-github")
 source.set_config(
    "credentials": {
       "personal_access_token": get_secret("GITHUB_PERSONAL_ACCESS_TOKEN"),
    }
 )
 ```
 
@@ -96,31 +96,31 @@
 
 For a more lightweight check, the `--validate-install-only` flag can be used. This will only check that the connector can be installed and returns a spec, no sample config required.
 
 ## Contributing
 
 To learn how you can contribute to PyAirbyte, please see our [PyAirbyte Contributors Guide](./CONTRIBUTING.md).
 
-## Frequently asked Questions 
+## Frequently asked Questions
 
 **1. Does PyAirbyte replace Airbyte?**
-No. 
+No.
 
 **2. What is the PyAirbyte cache? Is it a destination?**
 Yes, you can think of it as a built-in destination implementation, but we avoid the word "destination" in our docs to prevent confusion with our certified destinations list [here](https://docs.airbyte.com/integrations/destinations/).
 
 **3. Does PyAirbyte work with data orchestration frameworks like Airflow, Dagster, and Snowpark,**
 Yes, it should. Please give it a try and report any problems you see. Also, drop us a note if works for you!
 
 **4. Can I use PyAirbyte to develop or test when developing Airbyte sources?**
 Yes, you can, but only for Python-based sources.
 
 **5. Can I develop traditional ETL pipelines with PyAirbyte?**
 Yes. Just pick the cache type matching the destination - like SnowflakeCache for landing data in Snowflake.
 
 **6. Can PyAirbyte import a connector from a local directory that has python project files, or does it have to be pip install**
-Yes, PyAirbyte can use any local install that has a CLI - and will automatically find connectors by name if they are on PATH. 
+Yes, PyAirbyte can use any local install that has a CLI - and will automatically find connectors by name if they are on PATH.
 
 
 ## Changelog and Release Notes
 
 For a version history and list of all changes, please see our [GitHub Releases](https://github.com/airbytehq/PyAirbyte/releases) page.
```

### Comparing `airbyte-0.8.2/airbyte/__init__.py` & `airbyte-0.8.3/airbyte/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/_batch_handles.py` & `airbyte-0.8.3/airbyte/_batch_handles.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/_executor.py` & `airbyte-0.8.3/airbyte/_executor.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/_processors/base.py` & `airbyte-0.8.3/airbyte/_processors/base.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/_processors/file/base.py` & `airbyte-0.8.3/airbyte/_processors/file/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pathlib import Path
 from typing import IO, TYPE_CHECKING, final
 
 import ulid
 
 from airbyte import exceptions as exc
 from airbyte._batch_handles import BatchHandle
-from airbyte._util.protocol_util import airbyte_record_message_to_dict
+from airbyte._util.name_normalizers import LowerCaseNormalizer, StreamRecord
 from airbyte.progress import progress
 
 
 if TYPE_CHECKING:
     from airbyte_protocol.models import (
         AirbyteRecordMessage,
     )
@@ -142,17 +142,14 @@
         self,
         record_msg: AirbyteRecordMessage,
         stream_schema: dict,
     ) -> None:
         """Write a record to the cache.
 
         This method is called for each record message, before the batch is written.
-
-        Returns:
-            A tuple of the stream name and the batch handle.
         """
         stream_name = record_msg.stream
 
         batch_handle: BatchHandle
         if stream_name not in self._active_batches:
             batch_handle = self._new_batch(stream_name=stream_name)
 
@@ -163,17 +160,18 @@
             # Already at max batch size, so start a new batch.
             batch_handle = self._new_batch(stream_name=stream_name)
 
         if batch_handle.open_file_writer is None:
             raise exc.AirbyteLibInternalError(message="Expected open file writer.")
 
         self._write_record_dict(
-            record_dict=airbyte_record_message_to_dict(
-                record_message=record_msg,
-                stream_schema=stream_schema,
+            record_dict=StreamRecord(
+                from_dict=record_msg.data,
+                expected_keys=stream_schema["properties"].keys(),
+                normalizer=LowerCaseNormalizer,
                 prune_extra_fields=self.prune_extra_fields,
             ),
             open_file_writer=batch_handle.open_file_writer,
         )
         batch_handle.increment_record_count()
 
     def flush_active_batches(
@@ -212,15 +210,15 @@
             self.cleanup_all()
 
     # Abstract methods
 
     @abc.abstractmethod
     def _write_record_dict(
         self,
-        record_dict: dict,
+        record_dict: StreamRecord,
         open_file_writer: IO[bytes],
     ) -> None:
         """Write one record to a file."""
         raise NotImplementedError("No default implementation.")
 
     # Public methods (for use by Cache and SQL Processor classes)
```

### Comparing `airbyte-0.8.2/airbyte/_processors/file/jsonl.py` & `airbyte-0.8.3/airbyte/_processors/file/jsonl.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     FileWriterBase,
 )
 
 
 if TYPE_CHECKING:
     from pathlib import Path
 
-    pass
+    from airbyte._util.name_normalizers import StreamRecord
 
 
 class JsonlWriter(FileWriterBase):
     """A Jsonl cache implementation."""
 
     default_cache_file_suffix = ".jsonl.gz"
     prune_extra_fields = True
@@ -30,11 +30,11 @@
         file_path: Path,
     ) -> IO[bytes]:
         """Open a new file for writing."""
         return cast(IO[bytes], gzip.open(file_path, "w"))
 
     def _write_record_dict(
         self,
-        record_dict: dict,
+        record_dict: StreamRecord,
         open_file_writer: gzip.GzipFile | IO[bytes],
     ) -> None:
         open_file_writer.write(orjson.dumps(record_dict) + b"\n")
```

### Comparing `airbyte-0.8.2/airbyte/_processors/sql/base.py` & `airbyte-0.8.3/airbyte/_processors/sql/base.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/_processors/sql/bigquery.py` & `airbyte-0.8.3/airbyte/_processors/sql/bigquery.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/_processors/sql/duckdb.py` & `airbyte-0.8.3/airbyte/_processors/sql/duckdb.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,22 +83,22 @@
         temp_table_name = self._create_table_for_loading(
             stream_name=stream_name,
             batch_id=batch_id,
         )
         properties_list = list(self.get_stream_properties(stream_name).keys())
         columns_list = list(self._get_sql_column_definitions(stream_name=stream_name).keys())
         columns_list_str = indent(
-            "\n, ".join([self._quote_identifier(c) for c in columns_list]),
+            "\n, ".join([self._quote_identifier(col) for col in columns_list]),
             "    ",
         )
         files_list = ", ".join([f"'{f!s}'" for f in files])
         columns_type_map = indent(
             "\n, ".join(
                 [
-                    self._quote_identifier(prop_name)
+                    self._quote_identifier(self.normalizer.normalize(prop_name))
                     + ": "
                     + str(
                         self._get_sql_column_definitions(stream_name)[
                             self.normalizer.normalize(prop_name)
                         ]
                     )
                     for prop_name in properties_list
```

### Comparing `airbyte-0.8.2/airbyte/_processors/sql/motherduck.py` & `airbyte-0.8.3/airbyte/_processors/sql/motherduck.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/_processors/sql/postgres.py` & `airbyte-0.8.3/airbyte/_processors/sql/postgres.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/_processors/sql/snowflake.py` & `airbyte-0.8.3/airbyte/_processors/sql/snowflake.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         columns_list = [
             self._quote_identifier(c)
             for c in list(self._get_sql_column_definitions(stream_name).keys())
         ]
         files_list = ", ".join([f"'{f.name}'" for f in files])
         columns_list_str: str = indent("\n, ".join(columns_list), " " * 12)
         variant_cols_str: str = ("\n" + " " * 21 + ", ").join(
-            [f"$1:{col}" for col in properties_list]
+            [f"$1:{self.normalizer.normalize(col)}" for col in properties_list]
         )
         copy_statement = dedent(
             f"""
             COPY INTO {temp_table_name}
             (
                 {columns_list_str}
             )
```

### Comparing `airbyte-0.8.2/airbyte/_util/document_rendering.py` & `airbyte-0.8.3/airbyte/_util/document_rendering.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/_util/google_secrets.py` & `airbyte-0.8.3/airbyte/_util/google_secrets.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/_util/meta.py` & `airbyte-0.8.3/airbyte/_util/meta.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/_util/name_normalizers.py` & `airbyte-0.8.3/airbyte/_util/name_normalizers.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from __future__ import annotations
 
 import abc
 from typing import TYPE_CHECKING, Any
 
 
 if TYPE_CHECKING:
-    from collections.abc import Iterable, Iterator
+    from collections.abc import Iterable
 
 
 class NameNormalizerBase(abc.ABC):
     """Abstract base class for name normalizers."""
 
     @staticmethod
     @abc.abstractmethod
@@ -46,24 +46,27 @@
 
     @staticmethod
     def normalize(name: str) -> str:
         """Return the normalized name."""
         return name.lower().replace(" ", "_").replace("-", "_")
 
 
-class CaseInsensitiveDict(dict[str, Any]):
-    """A case-aware, case-insensitive dictionary implementation.
+class StreamRecord(dict[str, Any]):
+    """The StreamRecord class is a case-aware, case-insensitive dictionary implementation.
 
     It has these behaviors:
     - When a key is retrieved, deleted, or checked for existence, it is always checked in a
       case-insensitive manner.
     - The original case is stored in a separate dictionary, so that the original case can be
       retrieved when needed.
 
-    There are two ways to store keys internally:
+    This behavior mirrors how a case-aware, case-insensitive SQL database would handle column
+    references.
+
+    There are two ways this class can store keys internally:
     - If normalize_keys is True, the keys are normalized using the given normalizer.
     - If normalize_keys is False, the original case of the keys is stored.
 
     In regards to missing values, the dictionary accepts an 'expected_keys' input. When set, the
     dictionary will be initialized with the given keys. If a key is not found in the input data, it
     will be initialized with a value of None. When provided, the 'expected_keys' input will also
     determine the original case of the keys.
@@ -84,45 +87,55 @@
 
         return self._display_case(key)
 
     def __init__(
         self,
         from_dict: dict,
         *,
+        prune_extra_fields: bool,
         normalize_keys: bool = True,
         normalizer: type[NameNormalizerBase] | None = None,
         expected_keys: list[str] | None = None,
     ) -> None:
         """Initialize the dictionary with the given data.
 
-        If normalize_keys is True, the keys will be normalized using the given normalizer.
-        If expected_keys is provided, the dictionary will be initialized with the given keys.
+        Args:
+        - normalize_keys: If `True`, the keys will be normalized using the given normalizer.
+        - expected_keys: If provided, the dictionary will be initialized with these given keys.
+        - expected_keys: If provided and `prune_extra_fields` is True, then unexpected fields
+          will be removed. This option is ignored if `expected_keys` is not provided.
         """
         # If no normalizer is provided, use LowerCaseNormalizer.
         self._normalize_keys = normalize_keys
         self._normalizer: type[NameNormalizerBase] = normalizer or LowerCaseNormalizer
 
         # If no expected keys are provided, use all keys from the input dictionary.
         if not expected_keys:
             expected_keys = list(from_dict.keys())
+            prune_extra_fields = False  # No expected keys provided.
 
         # Store a lookup from normalized keys to pretty cased (originally cased) keys.
         self._pretty_case_keys: dict[str, str] = {
             self._normalizer.normalize(pretty_case.lower()): pretty_case
             for pretty_case in expected_keys
         }
 
         if normalize_keys:
             index_keys = [self._normalizer.normalize(key) for key in expected_keys]
         else:
             index_keys = expected_keys
 
         self.update({k: None for k in index_keys})  # Start by initializing all values to None
         for k, v in from_dict.items():
-            self[self._index_case(k)] = v
+            index_cased_key = self._index_case(k)
+            if prune_extra_fields and index_cased_key not in index_keys:
+                # Dropping undeclared field
+                continue
+
+            self[index_cased_key] = v
 
     def __getitem__(self, key: str) -> Any:  # noqa: ANN401
         if super().__contains__(key):
             return super().__getitem__(key)
 
         if super().__contains__(self._index_case(key)):
             return super().__getitem__(self._index_case(key))
@@ -162,44 +175,22 @@
     def __iter__(self) -> Any:  # noqa: ANN401
         return iter(super().__iter__())
 
     def __len__(self) -> int:
         return super().__len__()
 
     def __eq__(self, other: object) -> bool:
-        if isinstance(other, CaseInsensitiveDict):
+        if isinstance(other, StreamRecord):
             return dict(self) == dict(other)
 
         if isinstance(other, dict):
             return {k.lower(): v for k, v in self.items()} == {
                 k.lower(): v for k, v in other.items()
             }
         return False
 
 
-def normalize_records(
-    records: Iterable[dict[str, Any]],
-    expected_keys: list[str],
-) -> Iterator[CaseInsensitiveDict]:
-    """Add missing columns to the record with null values.
-
-    Also conform the column names to the case in the catalog.
-
-    This is a generator that yields CaseInsensitiveDicts, which allows for case-insensitive
-    lookups of columns. This is useful because the case of the columns in the records may
-    not match the case of the columns in the catalog.
-    """
-    yield from (
-        CaseInsensitiveDict(
-            from_dict=record,
-            expected_keys=expected_keys,
-        )
-        for record in records
-    )
-
-
 __all__ = [
     "NameNormalizerBase",
     "LowerCaseNormalizer",
-    "CaseInsensitiveDict",
-    "normalize_records",
+    "StreamRecord",
 ]
```

### Comparing `airbyte-0.8.2/airbyte/_util/pip_util.py` & `airbyte-0.8.3/airbyte/_util/pip_util.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/_util/telemetry.py` & `airbyte-0.8.3/airbyte/_util/telemetry.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/caches/__init__.py` & `airbyte-0.8.3/airbyte/caches/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/caches/_catalog_manager.py` & `airbyte-0.8.3/airbyte/caches/_catalog_manager.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/caches/base.py` & `airbyte-0.8.3/airbyte/caches/base.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/caches/bigquery.py` & `airbyte-0.8.3/airbyte/caches/bigquery.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/caches/duckdb.py` & `airbyte-0.8.3/airbyte/caches/duckdb.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/caches/motherduck.py` & `airbyte-0.8.3/airbyte/caches/motherduck.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/caches/postgres.py` & `airbyte-0.8.3/airbyte/caches/postgres.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/caches/snowflake.py` & `airbyte-0.8.3/airbyte/caches/snowflake.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/caches/util.py` & `airbyte-0.8.3/airbyte/caches/util.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/datasets/_base.py` & `airbyte-0.8.3/airbyte/datasets/_base.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/datasets/_lazy.py` & `airbyte-0.8.3/airbyte/datasets/_lazy.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/datasets/_map.py` & `airbyte-0.8.3/airbyte/datasets/_map.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/datasets/_sql.py` & `airbyte-0.8.3/airbyte/datasets/_sql.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/documents.py` & `airbyte-0.8.3/airbyte/documents.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/exceptions.py` & `airbyte-0.8.3/airbyte/exceptions.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/progress.py` & `airbyte-0.8.3/airbyte/progress.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/results.py` & `airbyte-0.8.3/airbyte/results.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/secrets.py` & `airbyte-0.8.3/airbyte/secrets.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/sources/__init__.py` & `airbyte-0.8.3/airbyte/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/sources/base.py` & `airbyte-0.8.3/airbyte/sources/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,15 @@
     Status,
     SyncMode,
     TraceType,
     Type,
 )
 
 from airbyte import exceptions as exc
-from airbyte._util import protocol_util
-from airbyte._util.name_normalizers import normalize_records
+from airbyte._util.name_normalizers import StreamRecord
 from airbyte._util.telemetry import (
     EventState,
     EventType,
     log_config_validation_result,
     log_source_check_result,
     send_telemetry,
 )
@@ -69,15 +68,15 @@
             )
             temp_file.flush()
             temp_files.append(temp_file)
         yield [file.name for file in temp_files]
     finally:
         for temp_file in temp_files:
             with suppress(Exception):
-                temp_file.unlink()
+                Path(temp_file.name).unlink()
 
 
 class Source:
     """A class representing a source that can be called."""
 
     def __init__(
         self,
@@ -433,21 +432,22 @@
 
         def _with_logging(records: Iterable[dict[str, Any]]) -> Iterator[dict[str, Any]]:
             self._log_sync_start(cache=None)
             yield from records
             self._log_sync_success(cache=None)
 
         iterator: Iterator[dict[str, Any]] = _with_logging(
-            normalize_records(
-                records=protocol_util.airbyte_messages_to_record_dicts(
-                    self._read_with_catalog(configured_catalog),
-                    stream_schema=self.get_stream_json_schema(stream),
+            records=(  # Generator comprehension yields StreamRecord objects for each record
+                StreamRecord(
+                    from_dict=record.record.data,
+                    expected_keys=all_properties,
                     prune_extra_fields=True,
-                ),
-                expected_keys=all_properties,
+                )
+                for record in self._read_with_catalog(configured_catalog)
+                if record.record
             )
         )
         return LazyDataset(
             iterator,
             stream_metadata=configured_stream,
         )
```

### Comparing `airbyte-0.8.2/airbyte/sources/registry.py` & `airbyte-0.8.3/airbyte/sources/registry.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/sources/util.py` & `airbyte-0.8.3/airbyte/sources/util.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/strategies.py` & `airbyte-0.8.3/airbyte/strategies.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/types.py` & `airbyte-0.8.3/airbyte/types.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/airbyte/validate.py` & `airbyte-0.8.3/airbyte/validate.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.2/pyproject.toml` & `airbyte-0.8.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "PyAirbyte"
 authors = ["Airbyte <contact@airbyte.io>"]
 readme = "README.md"
 packages = [{include = "airbyte"}]
 
 # This project uses dynamic versioning
 # https://github.com/mtkennerly/poetry-dynamic-versioning
-version = "0.8.2"
+version = "0.8.3"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
```

### Comparing `airbyte-0.8.2/PKG-INFO` & `airbyte-0.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte
-Version: 0.8.2
+Version: 0.8.3
 Summary: PyAirbyte
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -32,32 +32,32 @@
 Requires-Dist: sqlalchemy-bigquery (==1.9.0) ; python_version < "3.13"
 Requires-Dist: types-pyyaml (>=6.0.12.12,<7.0.0.0)
 Requires-Dist: ulid (>=1.1,<2.0)
 Description-Content-Type: text/markdown
 
 # PyAirbyte
 
-PyAirbyte brings the power of Airbyte to every Python developer. PyAirbyte provides a set of utilities to use Airbyte connectors in Python. It is meant to be used in situations where setting up an Airbyte server or cloud account is not possible or desirable. 
+PyAirbyte brings the power of Airbyte to every Python developer. PyAirbyte provides a set of utilities to use Airbyte connectors in Python. It is meant to be used in situations where setting up an Airbyte server or cloud account is not possible or desirable.
 
 - [Getting Started](#getting-started)
 - [Secrets Management](#secrets-management)
 - [Connector compatibility](#connector-compatibility)
 - [Contributing](#contributing)
 - [Frequently asked Questions](#frequently-asked-questions)
 
-## Getting Started 
+## Getting Started
 
-Watch this [Getting Started Loom video](https://www.loom.com/share/3de81ca3ce914feca209bf83777efa3f?sid=8804e8d7-096c-4aaa-a8a4-9eb93a44e850) or run one of our Quickstart tutorials below to see how you can use PyAirbyte in your python code. 
+Watch this [Getting Started Loom video](https://www.loom.com/share/3de81ca3ce914feca209bf83777efa3f?sid=8804e8d7-096c-4aaa-a8a4-9eb93a44e850) or run one of our Quickstart tutorials below to see how you can use PyAirbyte in your python code.
 
 * [Basic Demo](https://github.com/airbytehq/quickstarts/blob/main/pyairbyte_notebooks/PyAirbyte_Basic_Features_Demo.ipynb)
 * [CoinAPI](https://github.com/airbytehq/quickstarts/blob/main/pyairbyte_notebooks/PyAirbyte_CoinAPI_Demo.ipynb)
-* [GA4](https://github.com/airbytehq/quickstarts/blob/main/pyairbyte_notebooks/PyAirbyte_GA4_Demo.ipynb) 
-* [Shopify](https://github.com/airbytehq/quickstarts/blob/main/pyairbyte_notebooks/PyAirbyte_Shopify_Demo.ipynb) 
-* [GitHub](https://github.com/airbytehq/quickstarts/blob/main/pyairbyte_notebooks/PyAirbyte_Github_Incremental_Demo.ipynb) 
-* [Postgres (cache)](https://github.com/airbytehq/quickstarts/blob/main/pyairbyte_notebooks/PyAirbyte_Postgres_Custom_Cache_Demo.ipynb)  
+* [GA4](https://github.com/airbytehq/quickstarts/blob/main/pyairbyte_notebooks/PyAirbyte_GA4_Demo.ipynb)
+* [Shopify](https://github.com/airbytehq/quickstarts/blob/main/pyairbyte_notebooks/PyAirbyte_Shopify_Demo.ipynb)
+* [GitHub](https://github.com/airbytehq/quickstarts/blob/main/pyairbyte_notebooks/PyAirbyte_Github_Incremental_Demo.ipynb)
+* [Postgres (cache)](https://github.com/airbytehq/quickstarts/blob/main/pyairbyte_notebooks/PyAirbyte_Postgres_Custom_Cache_Demo.ipynb)
 
 
 ## Secrets Management
 
 PyAirbyte can auto-import secrets from the following sources:
 
 1. Environment variables.
@@ -68,15 +68,15 @@
 _Note: Additional secret store options may be supported in the future. [More info here.](https://github.com/airbytehq/airbyte-lib-private-beta/discussions/5)_
 
 ### Retrieving Secrets
 
 ```python
 from airbyte import get_secret, SecretSource
 
-source = get_connection("source-github")
+source = get_source("source-github")
 source.set_config(
    "credentials": {
       "personal_access_token": get_secret("GITHUB_PERSONAL_ACCESS_TOKEN"),
    }
 )
 ```
 
@@ -132,32 +132,32 @@
 
 For a more lightweight check, the `--validate-install-only` flag can be used. This will only check that the connector can be installed and returns a spec, no sample config required.
 
 ## Contributing
 
 To learn how you can contribute to PyAirbyte, please see our [PyAirbyte Contributors Guide](./CONTRIBUTING.md).
 
-## Frequently asked Questions 
+## Frequently asked Questions
 
 **1. Does PyAirbyte replace Airbyte?**
-No. 
+No.
 
 **2. What is the PyAirbyte cache? Is it a destination?**
 Yes, you can think of it as a built-in destination implementation, but we avoid the word "destination" in our docs to prevent confusion with our certified destinations list [here](https://docs.airbyte.com/integrations/destinations/).
 
 **3. Does PyAirbyte work with data orchestration frameworks like Airflow, Dagster, and Snowpark,**
 Yes, it should. Please give it a try and report any problems you see. Also, drop us a note if works for you!
 
 **4. Can I use PyAirbyte to develop or test when developing Airbyte sources?**
 Yes, you can, but only for Python-based sources.
 
 **5. Can I develop traditional ETL pipelines with PyAirbyte?**
 Yes. Just pick the cache type matching the destination - like SnowflakeCache for landing data in Snowflake.
 
 **6. Can PyAirbyte import a connector from a local directory that has python project files, or does it have to be pip install**
-Yes, PyAirbyte can use any local install that has a CLI - and will automatically find connectors by name if they are on PATH. 
+Yes, PyAirbyte can use any local install that has a CLI - and will automatically find connectors by name if they are on PATH.
 
 
 ## Changelog and Release Notes
 
 For a version history and list of all changes, please see our [GitHub Releases](https://github.com/airbytehq/PyAirbyte/releases) page.
```

