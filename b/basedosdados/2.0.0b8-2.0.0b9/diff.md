# Comparing `tmp/basedosdados-2.0.0b8.tar.gz` & `tmp/basedosdados-2.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basedosdados-2.0.0b8.tar", max compression
+gzip compressed data, was "basedosdados-2.0.0b9.tar", max compression
```

## Comparing `basedosdados-2.0.0b8.tar` & `basedosdados-2.0.0b9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     2514 2023-05-17 15:25:36.000000 basedosdados-2.0.0b8/README.md
--rw-r--r--   0        0        0      909 2023-07-06 00:29:58.316017 basedosdados-2.0.0b8/basedosdados/__init__.py
--rw-r--r--   0        0        0      156 2023-05-17 15:25:36.000000 basedosdados-2.0.0b8/basedosdados/__main__.py
--rw-r--r--   0        0        0       84 2023-07-06 00:29:58.316143 basedosdados-2.0.0b8/basedosdados/_version.py
--rw-r--r--   0        0        0     4082 2023-07-06 00:29:58.316264 basedosdados-2.0.0b8/basedosdados/_warnings.py
--rw-r--r--   0        0        0     9545 2023-05-17 16:26:49.000000 basedosdados-2.0.0b8/basedosdados/backend/__init__.py
--rw-r--r--   0        0        0     6737 2023-05-17 15:25:36.000000 basedosdados-2.0.0b8/basedosdados/cli/cli.py
--rw-r--r--   0        0        0      277 2023-05-17 15:25:36.000000 basedosdados-2.0.0b8/basedosdados/configs/config.toml
--rw-r--r--   0        0        0      469 2022-02-13 03:48:24.000000 basedosdados-2.0.0b8/basedosdados/configs/templates/dataset/README.md
--rw-r--r--   0        0        0      856 2022-02-13 03:48:24.000000 basedosdados-2.0.0b8/basedosdados/configs/templates/dataset/dataset_description.txt
--rw-r--r--   0        0        0     1036 2022-02-13 03:48:24.000000 basedosdados-2.0.0b8/basedosdados/configs/templates/table/publish.sql
--rw-r--r--   0        0        0     2511 2022-03-17 20:15:08.000000 basedosdados-2.0.0b8/basedosdados/configs/templates/table/table_description.txt
--rw-r--r--   0        0        0      895 2023-05-17 15:25:36.000000 basedosdados-2.0.0b8/basedosdados/constants.py
--rw-r--r--   0        0        0        0 2022-02-13 03:48:24.000000 basedosdados-2.0.0b8/basedosdados/download/__init__.py
--rw-r--r--   0        0        0     1641 2023-05-17 15:25:36.000000 basedosdados-2.0.0b8/basedosdados/download/base.py
--rw-r--r--   0        0        0    17788 2023-05-17 15:25:36.000000 basedosdados-2.0.0b8/basedosdados/download/download.py
--rw-r--r--   0        0        0    13689 2023-05-17 15:25:36.000000 basedosdados-2.0.0b8/basedosdados/download/metadata.py
--rw-r--r--   0        0        0     3903 2023-05-17 15:25:36.000000 basedosdados-2.0.0b8/basedosdados/exceptions.py
--rw-r--r--   0        0        0     6779 2023-05-17 15:25:36.000000 basedosdados-2.0.0b8/basedosdados/schemas/columns_schema.json
--rw-r--r--   0        0        0    65118 2023-05-17 15:25:36.000000 basedosdados-2.0.0b8/basedosdados/schemas/dataset_schema.json
--rw-r--r--   0        0        0    30753 2023-05-17 15:25:36.000000 basedosdados-2.0.0b8/basedosdados/schemas/table_schema.json
--rw-r--r--   0        0        0        0 2022-02-13 03:48:24.000000 basedosdados-2.0.0b8/basedosdados/upload/__init__.py
--rw-r--r--   0        0        0    15604 2023-07-26 15:13:33.274155 basedosdados-2.0.0b8/basedosdados/upload/base.py
--rw-r--r--   0        0        0     4957 2023-05-17 15:25:36.000000 basedosdados-2.0.0b8/basedosdados/upload/connection.py
--rw-r--r--   0        0        0     9399 2023-05-17 15:25:36.000000 basedosdados-2.0.0b8/basedosdados/upload/dataset.py
--rw-r--r--   0        0        0     3552 2023-08-21 14:44:35.788427 basedosdados-2.0.0b8/basedosdados/upload/datatypes.py
--rw-r--r--   0        0        0    18883 2023-05-19 20:35:33.000000 basedosdados-2.0.0b8/basedosdados/upload/storage.py
--rw-r--r--   0        0        0    32020 2023-08-21 15:05:25.460979 basedosdados-2.0.0b8/basedosdados/upload/table.py
--rw-r--r--   0        0        0     3434 2023-05-17 15:25:36.000000 basedosdados-2.0.0b8/basedosdados/upload/utils.py
--rw-r--r--   0        0        0     1453 2023-08-21 15:06:34.430734 basedosdados-2.0.0b8/pyproject.toml
--rw-r--r--   0        0        0     3993 1970-01-01 00:00:00.000000 basedosdados-2.0.0b8/PKG-INFO
+-rw-r--r--   0        0        0     2497 2023-08-24 18:04:24.351987 basedosdados-2.0.0b9/README.md
+-rw-r--r--   0        0        0      906 2023-08-24 18:04:24.352661 basedosdados-2.0.0b9/basedosdados/__init__.py
+-rw-r--r--   0        0        0      156 2023-05-17 15:25:36.000000 basedosdados-2.0.0b9/basedosdados/__main__.py
+-rw-r--r--   0        0        0       84 2023-07-06 00:29:58.316143 basedosdados-2.0.0b9/basedosdados/_version.py
+-rw-r--r--   0        0        0     4106 2023-08-24 18:04:24.353269 basedosdados-2.0.0b9/basedosdados/_warnings.py
+-rw-r--r--   0        0        0    10326 2023-08-24 18:04:24.353943 basedosdados-2.0.0b9/basedosdados/backend/__init__.py
+-rw-r--r--   0        0        0     7159 2023-08-24 18:04:24.354237 basedosdados-2.0.0b9/basedosdados/cli/cli.py
+-rw-r--r--   0        0        0      276 2023-08-24 18:04:24.354592 basedosdados-2.0.0b9/basedosdados/configs/config.toml
+-rw-r--r--   0        0        0      469 2022-02-13 03:48:24.000000 basedosdados-2.0.0b9/basedosdados/configs/templates/dataset/README.md
+-rw-r--r--   0        0        0      856 2022-02-13 03:48:24.000000 basedosdados-2.0.0b9/basedosdados/configs/templates/dataset/dataset_description.txt
+-rw-r--r--   0        0        0     1035 2023-08-24 18:04:24.355498 basedosdados-2.0.0b9/basedosdados/configs/templates/table/publish.sql
+-rw-r--r--   0        0        0     2511 2022-03-17 20:15:08.000000 basedosdados-2.0.0b9/basedosdados/configs/templates/table/table_description.txt
+-rw-r--r--   0        0        0      895 2023-08-24 18:04:24.356463 basedosdados-2.0.0b9/basedosdados/constants.py
+-rw-r--r--   0        0        0        0 2022-02-13 03:48:24.000000 basedosdados-2.0.0b9/basedosdados/download/__init__.py
+-rw-r--r--   0        0        0     1639 2023-08-24 18:04:24.356835 basedosdados-2.0.0b9/basedosdados/download/base.py
+-rw-r--r--   0        0        0    17763 2023-08-24 18:04:24.357325 basedosdados-2.0.0b9/basedosdados/download/download.py
+-rw-r--r--   0        0        0    13698 2023-08-24 18:04:24.357906 basedosdados-2.0.0b9/basedosdados/download/metadata.py
+-rw-r--r--   0        0        0     4049 2023-08-24 18:04:24.358503 basedosdados-2.0.0b9/basedosdados/exceptions.py
+-rw-r--r--   0        0        0     6779 2023-05-17 15:25:36.000000 basedosdados-2.0.0b9/basedosdados/schemas/columns_schema.json
+-rw-r--r--   0        0        0    65118 2023-05-17 15:25:36.000000 basedosdados-2.0.0b9/basedosdados/schemas/dataset_schema.json
+-rw-r--r--   0        0        0    30753 2023-05-17 15:25:36.000000 basedosdados-2.0.0b9/basedosdados/schemas/table_schema.json
+-rw-r--r--   0        0        0        0 2022-02-13 03:48:24.000000 basedosdados-2.0.0b9/basedosdados/upload/__init__.py
+-rw-r--r--   0        0        0    15542 2023-08-24 18:04:24.359260 basedosdados-2.0.0b9/basedosdados/upload/base.py
+-rw-r--r--   0        0        0     5026 2023-08-24 18:04:24.359575 basedosdados-2.0.0b9/basedosdados/upload/connection.py
+-rw-r--r--   0        0        0     9389 2023-08-24 18:04:24.359987 basedosdados-2.0.0b9/basedosdados/upload/dataset.py
+-rw-r--r--   0        0        0     4066 2023-08-24 18:04:24.360240 basedosdados-2.0.0b9/basedosdados/upload/datatypes.py
+-rw-r--r--   0        0        0    18920 2023-08-24 18:04:24.360593 basedosdados-2.0.0b9/basedosdados/upload/storage.py
+-rw-r--r--   0        0        0    31976 2023-08-24 18:04:24.361143 basedosdados-2.0.0b9/basedosdados/upload/table.py
+-rw-r--r--   0        0        0     3434 2023-08-24 18:04:24.361475 basedosdados-2.0.0b9/basedosdados/upload/utils.py
+-rw-r--r--   0        0        0     2072 2023-08-24 18:04:24.363026 basedosdados-2.0.0b9/pyproject.toml
+-rw-r--r--   0        0        0     4076 1970-01-01 00:00:00.000000 basedosdados-2.0.0b9/PKG-INFO
```

### Comparing `basedosdados-2.0.0b8/README.md` & `basedosdados-2.0.0b9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Python Package
 
-## Desenvolvimento Linux e Mac: 
+## Desenvolvimento Linux e Mac:
 
 Clone o repositório principal:
 
 ```sh
 git clone https://github.com/basedosdados/mais.git
 ```
 Entre na pasta local do repositório usando `cd mais/` e suba o ambiente localmente:
@@ -16,50 +16,50 @@
 python setup.py develop
 ```
 
 ### Desenvolva uma nova feature
 
 1. Abra uma branch com o nome issue-<X>
 2. Faça as modificações necessárias
-3. Suba o Pull Request apontando para a branch `python-next-minor` ou `python-next-patch`. 
+3. Suba o Pull Request apontando para a branch `python-next-minor` ou `python-next-patch`.
     Sendo, minor e patch referentes ao bump da versão: v1.5.7 --> v\<major>.\<minor>.\<patch>.
 4. O nome do PR deve seguir o padrão
     `[infra] <titulo explicativo>`
 
 
 ### O que uma modificação precisa ter
 
-  
+
 - Resolver o problema
 - Lista de modificações efetuadas
     1. Mudei a função X para fazer Y
     2. Troquei o nome da variavel Z
 - Referência aos issues atendidos
 - Documentação e Docstrings
 - Testes
-  
+
 
 ## Versionamento
 
 **Para publicar uma nova versão do pacote é preciso seguir os seguintes passos:**
 
 1. Fazer o pull da branch:
 
     ```bash
     git pull origin [python-version]
     ```
-  
+
     Onde `[python-version]` é a branch da nova versão do pacote.
 
 2. Se necessario adicionar novas dependências:
     ```bash
       poetry add <package-name>
     ```
 
-3. Gerar novo `requirements-dev.txt` 
+3. Gerar novo `requirements-dev.txt`
 
     ```bash
     poetry export -f requirements.txt --output requirements-dev.txt --without-hashes
     ```
 
 4. Editar `pyproject.toml`:
 
@@ -73,27 +73,27 @@
     packages = [
       {include = "basedosdados"},
     ]
     readme = "README.md"
     repository = "https://github.com/base-dos-dados/bases"
     version = "1.6.1-beta.2"
     ```
-    
+
     O campo `version` deve ser alterado para o número da versão sendo lançada.
 
 5. Push para branch:
 
     ```bash
     git push origin [python-version]
     ```
 
 6. Publicação do pacote no PyPI (exige usuário e senha):
 
     Para publicar o pacote no PyPI, use:
-    
+
     ```bash
     poetry version [python-version]
     poetry publish --build
     ```
 
 7. Faz merge da branch para a master
 8. Faz release usando a UI do GitHub
```

### Comparing `basedosdados-2.0.0b8/basedosdados/__init__.py` & `basedosdados-2.0.0b9/basedosdados/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 """
 Importing the module will automatically import the submodules.
 """
-
-import sys
+# flake8: noqa
 import os
+import sys
 
 from basedosdados._version import __version__
 from basedosdados._warnings import show_warnings
 
 show_warnings()
 
 sys.path.append(f"{os.getcwd()}/python-package")
 
 # pylint: disable=C0413
 
 from basedosdados.backend import Backend
-from basedosdados.constants import constants, config
-from basedosdados.upload.connection import Connection
-from basedosdados.upload.dataset import Dataset
-from basedosdados.upload.storage import Storage
-from basedosdados.upload.table import Table
+from basedosdados.constants import config, constants
 from basedosdados.download.base import reauth
-from basedosdados.download.download import (
-    read_sql,
-    download,
-    read_table,
-)
+from basedosdados.download.download import download, read_sql, read_table
 from basedosdados.download.metadata import (
-    list_datasets,
-    list_dataset_tables,
-    get_table_description,
     get_dataset_description,
     get_table_columns,
+    get_table_description,
     get_table_size,
+    list_dataset_tables,
+    list_datasets,
     search,
 )
+from basedosdados.upload.connection import Connection
+from basedosdados.upload.dataset import Dataset
+from basedosdados.upload.storage import Storage
+from basedosdados.upload.table import Table
```

### Comparing `basedosdados-2.0.0b8/basedosdados/_warnings.py` & `basedosdados-2.0.0b9/basedosdados/_warnings.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 def get_latest_version_number():
     """Get the latest version number from PyPI."""
     try:
         response = requests.get("https://pypi.python.org/pypi/basedosdados/json")
         return response.json()["info"]["version"]
-    except:
+    except:  # noqa
         logger.warning(
             "Could not check for updates. Please check your internet connection."
         )
         return None
 
 
 def compare_version_numbers(versionA: str, versionB: str) -> Tuple[int, str, str]:
@@ -87,15 +87,15 @@
             comparison = compare_version_numbers(__version__, latest_version)
             if comparison[0] == -1:
                 logger.warning(
                     f"You are using an outdated version of basedosdados ({__version__}). "
                     f"Please upgrade to the latest version ({latest_version}) using "
                     "'pip install --upgrade basedosdados'."
                 )
-    except:
+    except:  # noqa
         logger.warning(
             "Could not check for updates. Please check your internet connection."
         )
     # General-purpose warnings and messages
     try:
         response = requests.get(
             "https://basedosdados.github.io/notifications/data.json"
@@ -111,11 +111,11 @@
         if "python" in data:
             if "messages" in data["python"]:
                 for message in data["python"]["messages"]:
                     logger.info(message)
             if "warnings" in data["python"]:
                 for warning in data["python"]["warnings"]:
                     logger.warning(warning)
-    except:
+    except:  # noqa
         logger.warning(
             "Could not check for warnings and messages. Please check your internet connection."
         )
```

### Comparing `basedosdados-2.0.0b8/basedosdados/backend/__init__.py` & `basedosdados-2.0.0b9/basedosdados/backend/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 """
 Module for interacting with the backend.
 """
 from typing import Any, Dict
+
 from loguru import logger
 
-from gql import gql, Client
-from gql.transport.requests import RequestsHTTPTransport
+try:
+    from gql import Client, gql
+    from gql.transport.requests import RequestsHTTPTransport
+
+    _backend_dependencies = True
+except ImportError:
+    _backend_dependencies = False
 
-from basedosdados.exceptions import BaseDosDadosException
+from basedosdados.exceptions import BaseDosDadosMissingDependencyException
 
 
 class Backend:
     def __init__(self, graphql_url: str):
         """
         Backend class for interacting with the backend.
 
@@ -25,39 +31,45 @@
         """
         GraphQL endpoint URL.
         """
         return self._graphql_url
 
     def _get_client(
         self, headers: Dict[str, str] = None, fetch_schema_from_transport: bool = False
-    ) -> Client:
+    ) -> "Client":
         """
         Get a GraphQL client.
 
         Args:
             headers (Dict[str, str], optional): Headers to be passed to the client. Defaults to
                 None.
             fetch_schema_from_transport (bool, optional): Whether to fetch the schema from the
                 transport. Defaults to False.
 
         Returns:
             Client: GraphQL client.
         """
+        if not _backend_dependencies:
+            raise BaseDosDadosMissingDependencyException(
+                "Optional dependencies for backend interaction are not installed. "
+                'Please install basedosdados with the "backend" extra, such as:'
+                "\n\npip install basedosdados[backend]"
+            )
         transport = RequestsHTTPTransport(
             url=self.graphql_url, headers=headers, use_json=True
         )
         return Client(
             transport=transport, fetch_schema_from_transport=fetch_schema_from_transport
         )
 
     def _execute_query(
         self,
         query: str,
         variables: Dict[str, str] = None,
-        client: Client = None,
+        client: "Client" = None,
         headers: Dict[str, str] = None,
         fetch_schema_from_transport: bool = False,
     ) -> Dict[str, Any]:
         """
         Execute a GraphQL query.
 
         Args:
@@ -69,14 +81,20 @@
                 None.
             fetch_schema_from_transport (bool, optional): Whether to fetch the schema from the
                 transport. Defaults to False.
 
         Returns:
             Dict: GraphQL response.
         """
+        if not _backend_dependencies:
+            raise BaseDosDadosMissingDependencyException(
+                "Optional dependencies for backend interaction are not installed. "
+                'Please install basedosdados with the "backend" extra, such as:'
+                "\n\npip install basedosdados[backend]"
+            )
         if not client:
             client = self._get_client(
                 headers=headers, fetch_schema_from_transport=fetch_schema_from_transport
             )
         try:
             return client.execute(gql(query), variable_values=variables)
         except Exception as e:
@@ -176,15 +194,15 @@
                             organization {
                                 namePt
                             }
                         }
                     }
                 }
             }
-        
+
         """
         dataset_id = self._get_dataset_id_from_name(dataset_id)
         if dataset_id:
             variables = {"dataset_id": dataset_id}
             response = self._execute_query(query=query, variables=variables)
             return self._simplify_graphql_response(response).get("allDataset")[0]
         else:
@@ -229,15 +247,15 @@
                                     }
                                 }
                             }
                         }
                     }
                 }
                 }
-            }    
+            }
         """
         table_id = self._get_table_id_from_name(
             gcp_dataset_id=dataset_id, gcp_table_id=table_id
         )
 
         if table_id:
             variables = {"table_id": table_id}
@@ -259,15 +277,15 @@
 
         output_ = {}
 
         for key in response:
             try:
                 if (
                     isinstance(response[key], dict)
-                    and response[key].get("edges") is not None
+                    and response[key].get("edges") is not None  # noqa
                 ):
                     output_[key] = [
                         v.get("node")
                         for v in list(
                             map(self._simplify_graphql_response, response[key]["edges"])
                         )
                     ]
```

### Comparing `basedosdados-2.0.0b8/basedosdados/cli/cli.py` & `basedosdados-2.0.0b9/basedosdados/cli/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,30 @@
 """
 CLI package for the application.
 """
 
 # pylint: disable=locally-disabled, multiple-statements, fixme, line-too-long, too-many-arguments, invalid-name, too-many-lines, protected-access, unused-argument, no-value-for-parameter, redefined-builtin
 
-import click
-from basedosdados.upload.base import Base
+try:
+    import click
+
+    _cli_dependencies = True
+except ImportError:
+    _cli_dependencies = False
 
 import basedosdados as bd
+from basedosdados.exceptions import BaseDosDadosMissingDependencyException
+from basedosdados.upload.base import Base
+
+if not _cli_dependencies:
+    raise BaseDosDadosMissingDependencyException(
+        "Optional dependencies for the CLI are not installed. "
+        'Please install basedosdados with the "cli" extra, such as:'
+        "\n\npip install basedosdados[cli]"
+    )
 
 
 @click.group()
 @click.option("--bucket_name", default=None, help="Project bucket name")
 @click.version_option(package_name="basedosdados")
 @click.pass_context
 def cli(ctx, bucket_name):
@@ -191,15 +204,15 @@
 # Allow anomalous backslash in string: '\ ' (it's used in gcloud sdk)
 # pylint: disable=W1401
 @click.command(
     name="download",
     help=(
         "Downloads data do SAVEPATH. SAVEPATH must point to a .csv file.\n\n"
         "Example: \n\n"
-        'basedosdados download data.csv  --query="select * from basedosdados.br_ibge_pib.municipio limit 10" \ --billing_project_id=basedosdados-dev'
+        'basedosdados download data.csv  --query="select * from basedosdados.br_ibge_pib.municipio limit 10" --billing_project_id=basedosdados-dev'
     ),
 )
 @click.argument(
     "savepath",
     type=click.Path(exists=False),
 )
 @click.option(
```

### Comparing `basedosdados-2.0.0b8/basedosdados/configs/templates/dataset/dataset_description.txt` & `basedosdados-2.0.0b9/basedosdados/configs/templates/dataset/dataset_description.txt`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b8/basedosdados/configs/templates/table/publish.sql` & `basedosdados-2.0.0b9/basedosdados/configs/templates/table/publish.sql`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     - Para modificar tipos de colunas, basta substituir STRING por outro tipo válido.
     - Exemplo: `SAFE_CAST(column_name AS NUMERIC) column_name`
     - Mais detalhes: https://cloud.google.com/bigquery/docs/reference/standard-sql/data-types
 
 */
 {% set project = project_id_prod %}
 CREATE VIEW {{ project }}.{{ dataset_id }}.{{ table_id }} AS
-SELECT 
+SELECT
 {% for column in columns|list + partition_columns|list -%}
 {%- if not loop.last -%}
     SAFE_CAST({{ column }} AS STRING) {{ column }},
 {% else -%}
     SAFE_CAST({{ column }} AS STRING) {{ column }}
 {% endif -%}{% endfor -%}
 from {{ project_id }}.{{ dataset_id }}_staging.{{ table_id }} as t
```

### Comparing `basedosdados-2.0.0b8/basedosdados/configs/templates/table/table_description.txt` & `basedosdados-2.0.0b9/basedosdados/configs/templates/table/table_description.txt`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b8/basedosdados/constants.py` & `basedosdados-2.0.0b9/basedosdados/constants.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Constants for the project.
 """
 # pylint: disable=C0103
 __all__ = ["config", "constants"]
 
-from enum import Enum
 from dataclasses import dataclass
+from enum import Enum
 
 
 @dataclass
 class config:
     """
     Configuration for the project.
     """
```

### Comparing `basedosdados-2.0.0b8/basedosdados/download/base.py` & `basedosdados-2.0.0b9/basedosdados/download/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """
 Functions for manage auth and credentials
 """
-# pylint: disable=redefined-outer-name, protected-access, no-name-in-module, import-error,line-too-long
-from functools import lru_cache
-
 import sys
 
-from google.cloud import bigquery, storage
+# pylint: disable=redefined-outer-name, protected-access, no-name-in-module, import-error,line-too-long
+from functools import lru_cache
 
 import pydata_google_auth
-
+from google.cloud import bigquery, storage
 
 from basedosdados.upload.base import Base
 
 SCOPES = [
     "https://www.googleapis.com/auth/cloud-platform",
 ]
```

### Comparing `basedosdados-2.0.0b8/basedosdados/download/download.py` & `basedosdados-2.0.0b9/basedosdados/download/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 """
 Functions for managing downloads
 """
-# pylint: disable=too-many-arguments, fixme, invalid-name, protected-access,line-too-long
-from pathlib import Path
-from functools import partialmethod
+import gzip
+import os
 import re
-import time
 import shutil
-import os
-import gzip
+import time
+from functools import partialmethod
+
+# pylint: disable=too-many-arguments, fixme, invalid-name, protected-access,line-too-long
+from pathlib import Path
 
-from pydata_google_auth.exceptions import PyDataCredentialsError
-from google.cloud import bigquery_storage_v1
-from google.cloud import bigquery
 import pandas_gbq
+from google.cloud import bigquery, bigquery_storage_v1
 from pandas_gbq.gbq import GenericGBQException
+from pydata_google_auth.exceptions import PyDataCredentialsError
 
-from basedosdados.download.base import google_client, credentials
+from basedosdados.constants import config
+from basedosdados.download.base import credentials, google_client
 from basedosdados.exceptions import (
-    BaseDosDadosException,
     BaseDosDadosAccessDeniedException,
     BaseDosDadosAuthorizationException,
+    BaseDosDadosException,
     BaseDosDadosInvalidProjectIDException,
     BaseDosDadosNoBillingProjectIDException,
 )
-from basedosdados.constants import config
 
 
 def _set_config_variables(billing_project_id, from_file):
     """
     Set billing_project_id and from_file variables
     """
 
@@ -147,15 +147,15 @@
 
     billing_project_id, from_file = _set_config_variables(
         billing_project_id=billing_project_id, from_file=from_file
     )
 
     if (dataset_id is not None) and (table_id is not None):
         query = f"""
-        SELECT * 
+        SELECT *
         FROM `{query_project_id}.{dataset_id}.{table_id}`"""
 
         if limit is not None:
             query += f" LIMIT {limit}"
     else:
         raise BaseDosDadosException("Both table_id and dataset_id should be filled.")
 
@@ -239,15 +239,15 @@
     # if query is not defined (so it won't be overwritten) and if
     # table is a view or external or if limit is specified,
     # convert it to a query.
     if not query and (
         not _is_table(client, dataset_id, table_id, query_project_id) or limit
     ):
         query = f"""
-        SELECT * 
+        SELECT *
           FROM {query_project_id}.{dataset_id}.{table_id}
         """
 
         if limit is not None:
             query += f" limit {limit}"
 
     if query:
```

### Comparing `basedosdados-2.0.0b8/basedosdados/download/metadata.py` & `basedosdados-2.0.0b9/basedosdados/download/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 Functions to get metadata from BD's API
 """
+import math
+
 # pylint: disable=invalid-name,use-maxsplit-arg,line-too-long
 from collections import defaultdict
-import math
 
-from google.cloud import bigquery
 import pandas as pd
 import requests
+from google.cloud import bigquery
 
 
 def _safe_fetch(url: str):
     """
     Safely fetchs urls and, if somehting goes wrong, informs user what is the possible cause
     """
     response = None
@@ -46,15 +47,15 @@
 
     return temp_dict
 
 
 def _fix_size(s, step=80):
     final = ""
 
-    for l in s.split(" "):
+    for l in s.split(" "):  # noqa
         final += (l + " ") if len(final.split("\n")[-1]) < step else "\n"
 
     return final
 
 
 def _print_output(df):
     """Prints dataframe contents as print blocks
```

### Comparing `basedosdados-2.0.0b8/basedosdados/exceptions.py` & `basedosdados-2.0.0b9/basedosdados/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,7 +80,11 @@
             "\nYou can try again by rerunning this command with the flag "
             "`reauth=True`. \n\tLike `read_table('br_ibge_pib', 'municipios',"
             " billing_project_id=<YOUR_PROJECT_ID>, reauth=True)`"
             "\nThen you can click at the provided link and get the right "
             "authorization code."
         )
         super().__init__(self.message)
+
+
+class BaseDosDadosMissingDependencyException(BaseDosDadosException):
+    """Exception raised if one of the optional dependencies is missing."""
```

### Comparing `basedosdados-2.0.0b8/basedosdados/schemas/columns_schema.json` & `basedosdados-2.0.0b9/basedosdados/schemas/columns_schema.json`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b8/basedosdados/schemas/dataset_schema.json` & `basedosdados-2.0.0b9/basedosdados/schemas/dataset_schema.json`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b8/basedosdados/schemas/table_schema.json` & `basedosdados-2.0.0b9/basedosdados/schemas/table_schema.json`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b8/basedosdados/upload/base.py` & `basedosdados-2.0.0b9/basedosdados/upload/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """
 Module for manage dataset using local credentials and config files
 """
-from datetime import datetime
-
-# pylint: disable=line-too-long, invalid-name, too-many-arguments, invalid-envvar-value,line-too-long
-from pathlib import Path
-import sys
-from os import getenv
-import shutil
-import warnings
 import base64
 import json
+import shutil
+import sys
+import warnings
 from functools import lru_cache
+from os import getenv
+
+# pylint: disable=line-too-long, invalid-name, too-many-arguments, invalid-envvar-value,line-too-long
+from pathlib import Path
 from typing import Dict, List, Union
 
+import googleapiclient.discovery
+import tomlkit
 from google.cloud import bigquery, bigquery_connection_v1, storage
 from google.oauth2 import service_account
-import googleapiclient.discovery
 from loguru import logger
-import tomlkit
 
 from basedosdados.backend import Backend
 from basedosdados.constants import config, constants
 
 warnings.filterwarnings("ignore")
 
 
@@ -51,14 +50,21 @@
         self._init_config(force=overwrite_cli_config)
         self.config = self._load_config()
         self._config_log(config.verbose)
         self.bucket_name = bucket_name or self.config["bucket_name"]
         self.uri = f"gs://{self.bucket_name}" + "/staging/{dataset}/{table}/*"
         self._backend = Backend(self.config.get("api", {}).get("url", None))
 
+    @property
+    def backend(self):
+        """
+        Backend class
+        """
+        return self._backend
+
     @staticmethod
     def _decode_env(env: str) -> str:
         """
         Decode environment variable
         """
         return base64.b64decode(getenv(env).encode("utf-8")).decode("utf-8")
 
@@ -194,17 +200,17 @@
         # Create credentials folder
         credentials_folder = self.config_path / "credentials"
         credentials_folder.mkdir(exist_ok=True, parents=True)
 
         # If environments are set but no files exist
         if (
             (not config_file.exists())
-            and (getenv(constants.ENV_CONFIG.value))
-            and (getenv(constants.ENV_CREDENTIALS_PROD.value))
-            and (getenv(constants.ENV_CREDENTIALS_STAGING.value))
+            and (getenv(constants.ENV_CONFIG.value))  # noqa
+            and (getenv(constants.ENV_CREDENTIALS_PROD.value))  # noqa
+            and (getenv(constants.ENV_CREDENTIALS_STAGING.value))  # noqa
         ):
             # Create basedosdados files from envs
             with open(config_file, "w", encoding="utf-8") as f:
                 f.write(self._decode_env(constants.ENV_CONFIG.value))
                 f.close()
             with open(credentials_folder / "prod.json", "w", encoding="utf-8") as f:
                 f.write(self._decode_env(constants.ENV_CREDENTIALS_PROD.value))
@@ -225,15 +231,15 @@
                 "\n\nApparently, that is the first time that you are using "
                 "basedosdados :)\n"
                 "Before you go, we need to setup your workspace.\n"
                 "It will not take long, I promise!\n"
                 "[press enter to continue]"
             )
 
-            ############# STEP 1 - CREDENTIALS PATH ######################
+            # STEP 1 - CREDENTIALS PATH #
 
             credentials_path = self.config_path / "credentials"
             credentials_path = Path(
                 self._selection_yn(
                     first_question=(
                         "\n********* STEP 1 **********\n"
                         "Where do you want to save your Google Cloud credentials?\n"
@@ -244,15 +250,15 @@
                     no_question=(
                         "\nWhere would you like to save it?\n" "credentials path: "
                     ),
                     with_lower=False,
                 )
             )
 
-            ############# STEP 2 - STAGING CREDS. #######################
+            # STEP 2 - STAGING CREDS. #
             project_staging = self._input_validator(
                 "\n********* STEP 2 **********\n"
                 "What is the Google Cloud Project that you are going to use "
                 "to upload and treat data?\nIt might be something with 'staging'"
                 "in the name. If you just have one project, put its name.\n"
                 "Project id [basedosdados-staging]: ",
                 "basedosdados-staging",
@@ -261,15 +267,15 @@
             self._check_credentials(project_staging, "staging", credentials_path)
 
             c_file["gcloud-projects"]["staging"]["credentials_path"] = str(
                 credentials_path / "staging.json"
             )
             c_file["gcloud-projects"]["staging"]["name"] = project_staging
 
-            ############# STEP 3 - PROD CREDS. #######################
+            # STEP 3 - PROD CREDS. #
 
             project_prod = self._selection_yn(
                 first_question=(
                     "\n********* STEP 3 **********\n"
                     "Is your production project the same as the staging? [y/N]\n"
                 ),
                 default_yn="n",
@@ -290,26 +296,26 @@
                 self._check_credentials(project_prod, "prod", credentials_path)
 
             c_file["gcloud-projects"]["prod"]["credentials_path"] = str(
                 credentials_path / "prod.json"
             )
             c_file["gcloud-projects"]["prod"]["name"] = project_prod
 
-            ############# STEP 4 - BUCKET NAME #######################
+            # STEP 4 - BUCKET NAME #
 
             bucket_name = self._input_validator(
                 "\n********* STEP 4 **********\n"
                 "What is the Storage Bucket that you are going to be using to save the data?\n"
                 "Bucket name [basedosdados]: ",
                 "basedosdados",
             )
 
             c_file["bucket_name"] = bucket_name
 
-            ############# STEP 5 - CONFIGURE API #######################
+            # STEP 5 - CONFIGURE API #
 
             api_base_url = self._input_validator(
                 "\n********* STEP 5 **********\n"
                 "What is the URL of the API that you are going to use?\n"
                 "API url [https://staging.api.basedosdados.org/api/v1/graphql]: ",
                 "https://staging.api.basedosdados.org/api/v1/graphql",
             )
```

### Comparing `basedosdados-2.0.0b8/basedosdados/upload/connection.py` & `basedosdados-2.0.0b9/basedosdados/upload/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 from typing import Union
 
 import google.auth
 from google.cloud.bigquery_connection_v1.types import CloudResourceProperties
 from google.cloud.bigquery_connection_v1.types.connection import (
     Connection as BQConnection,
+)
+from google.cloud.bigquery_connection_v1.types.connection import (
     CreateConnectionRequest,
     DeleteConnectionRequest,
     GetConnectionRequest,
 )
 
 from basedosdados.upload.base import Base
```

### Comparing `basedosdados-2.0.0b8/basedosdados/upload/dataset.py` & `basedosdados-2.0.0b9/basedosdados/upload/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """
 Module for manage dataset to the server.
 """
 # pylint: disable=line-too-long, fixme, invalid-name,line-too-long
 from functools import lru_cache
-from pathlib import Path
-from loguru import logger
 
-from google.cloud import bigquery
 from google.api_core.exceptions import Conflict
+from google.cloud import bigquery
+from loguru import logger
 
 from basedosdados.upload.base import Base
 
 
 class Dataset(Base):
     """
     Manage datasets in BigQuery.
@@ -23,23 +22,25 @@
 
     @property
     @lru_cache
     def dataset_config(self):
         """
         Dataset config file.
         """
-        return self._backend.get_dataset_config(self.dataset_id)
+        return self.backend.get_dataset_config(self.dataset_id)
 
     def _loop_modes(self, mode="all"):
         """
         Loop modes.
         """
 
+        def dataset_tag(m):
+            return f"_{m}" if m == "staging" else ""
+
         mode = ["prod", "staging"] if mode == "all" else [mode]
-        dataset_tag = lambda m: f"_{m}" if m == "staging" else ""
         return (
             {
                 "client": self.client[f"bigquery_{m}"],
                 "id": f"{self.client[f'bigquery_{m}'].project}.{self.dataset_id}{dataset_tag(m)}",
                 "mode": m,
             }
             for m in mode
```

### Comparing `basedosdados-2.0.0b8/basedosdados/upload/datatypes.py` & `basedosdados-2.0.0b9/basedosdados/upload/datatypes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 """
 Class for define external and partiton configs for each datatype
 """
 # pylint: disable=protected-access,line-too-long
 import csv
 
-from google.cloud import bigquery
 import pandas as pd
-import pandavro
+from google.cloud import bigquery
+
+try:
+    import pandavro
+
+    _avro_dependencies = True
+except ImportError:
+    _avro_dependencies = False
+
+from basedosdados.exceptions import BaseDosDadosMissingDependencyException
 
 
 class Datatype:
     """
     Manage external and partition config
     """
 
@@ -41,14 +49,20 @@
         """
         Retrieve the header of the data sample
         """
 
         if self.source_format == "csv":
             return next(csv.reader(open(data_sample_path, "r", encoding="utf-8")))
         if self.source_format == "avro":
+            if not _avro_dependencies:
+                raise BaseDosDadosMissingDependencyException(
+                    "Optional dependencies for handling AVRO files are not installed. "
+                    'Please install basedosdados with the "avro" extra, such as:'
+                    "\n\npip install basedosdados[avro]"
+                )
             dataframe = pandavro.read_avro(str(data_sample_path))
             return list(dataframe.columns.values)
         if self.source_format == "parquet":
             dataframe = pd.read_parquet(str(data_sample_path))
             return list(dataframe.columns.values)
         raise NotImplementedError(
             "Base dos Dados just supports comma separated csv, avro and parquet files"
```

### Comparing `basedosdados-2.0.0b8/basedosdados/upload/storage.py` & `basedosdados-2.0.0b9/basedosdados/upload/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """
 Class for managing the files in cloud storage.
 """
+import sys
+
 # pylint: disable=invalid-name, too-many-arguments, undefined-loop-variable,line-too-long,broad-except,R0801
 import time
-from pathlib import Path
-import sys
 import traceback
+from pathlib import Path
 
-from tqdm import tqdm
 from loguru import logger
+from tqdm import tqdm
 
-from basedosdados.upload.base import Base
 from basedosdados.exceptions import BaseDosDadosException
+from basedosdados.upload.base import Base
 
 # google retryble exceptions. References: https://googleapis.dev/python/storage/latest/retry_timeout.html#module-google.cloud.storage.retry
 
 
 class Storage(Base):
     """
     Manage files on Google Cloud Storage.
@@ -396,15 +397,15 @@
             if not_found_ok:
                 return
             raise FileNotFoundError(
                 f"Could not find the requested table {self.dataset_id}.{self.table_id}"
             )
         # Divides table_blobs list for maximum batch request size
         table_blobs_chunks = [
-            table_blobs[i : i + 999] for i in range(0, len(table_blobs), 999)
+            table_blobs[i : i + 999] for i in range(0, len(table_blobs), 999)  # noqa
         ]
 
         for i, source_table in enumerate(
             tqdm(table_blobs_chunks, desc="Delete Table Chunk")
         ):
             counter = 0
             while counter < 10:
@@ -470,15 +471,16 @@
         else:
             destination_bucket = self.client["storage_staging"].bucket(
                 destination_bucket_name
             )
 
         # Divides source_table_ref list for maximum batch request size
         source_table_ref_chunks = [
-            source_table_ref[i : i + 999] for i in range(0, len(source_table_ref), 999)
+            source_table_ref[i : i + 999]  # noqa
+            for i in range(0, len(source_table_ref), 999)  # noqa
         ]
 
         for i, source_table in enumerate(
             tqdm(source_table_ref_chunks, desc="Copy Table Chunk")
         ):
             counter = 0
             while counter < 10:
```

### Comparing `basedosdados-2.0.0b8/basedosdados/upload/table.py` & `basedosdados-2.0.0b9/basedosdados/upload/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """
 Class for manage tables in Storage and Big Query
 """
 
 import contextlib
+import inspect
+import textwrap
+from copy import deepcopy
+from functools import lru_cache
 
 # pylint: disable=invalid-name, too-many-locals, too-many-branches, too-many-arguments,line-too-long,R0801,consider-using-f-string
 from pathlib import Path
-from copy import deepcopy
-import textwrap
-import inspect
-from functools import lru_cache
 
-from loguru import logger
+import google.api_core.exceptions
 from google.cloud import bigquery
 from google.cloud.bigquery import SchemaField
-import google.api_core.exceptions
+from loguru import logger
 
+from basedosdados.exceptions import BaseDosDadosException
 from basedosdados.upload.base import Base
 from basedosdados.upload.connection import Connection
-from basedosdados.upload.storage import Storage
 from basedosdados.upload.dataset import Dataset
 from basedosdados.upload.datatypes import Datatype
-from basedosdados.exceptions import BaseDosDadosException
+from basedosdados.upload.storage import Storage
 
 
 class Table(Base):
     """
     Manage tables in Google Cloud Storage and BigQuery.
     """
 
@@ -43,15 +43,15 @@
     @property
     @lru_cache(256)
     def table_config(self):
         """
         Load table config
         """
         # return self._load_yaml(self.table_folder / "table_config.yaml")
-        return self._backend.get_table_config(self.dataset_id, self.table_id)
+        return self.backend.get_table_config(self.dataset_id, self.table_id)
 
     def _get_table_obj(self, mode):
         """
         Get table object from BigQuery
         """
 
         return self.client[f"bigquery_{mode}"].get_table(self.table_full_name[mode])
@@ -71,15 +71,15 @@
     def _load_schema_from_json(
         self,
         columns=None,
     ):
         schema = []
 
         for col in columns:
-            ## ref: https://cloud.google.com/python/docs/reference/bigquery/latest/google.cloud.bigquery.schema.SchemaField
+            # ref: https://cloud.google.com/python/docs/reference/bigquery/latest/google.cloud.bigquery.schema.SchemaField
             if col.get("name") is None:
                 msg = "Columns must have a name! Check your data files for columns without name"
                 raise BaseDosDadosException(msg)
 
             schema.append(
                 SchemaField(
                     name=col.get("name"),
@@ -235,15 +235,15 @@
             return
         blobs = (
             self.client["storage_staging"]
             .bucket(self.bucket_name)
             .list_blobs(prefix=f"staging/{self.dataset_id}/{self.table_id}/")
         )
         partitions_dict = {}
-        ## only needs the first bloob
+        # only needs the first bloob
         for blob in blobs:
             for folder in blob.name.split("/"):
                 if "=" in folder:
                     key = folder.split("=")[0]
                     value = folder.split("=")
                     try:
                         partitions_dict[key].append(value)
@@ -315,15 +315,15 @@
                         bq_col["description"] = api_col.get("description")
 
         return bq_columns
 
     def _make_publish_sql(self):
         """Create publish.sql with columns and bigquery_type"""
 
-        ### publish.sql header and instructions
+        # publish.sql header and instructions
         publish_txt = """
         /*
         Query para publicar a tabela.
 
         Esse é o lugar para:
             - modificar nomes, ordem e tipos de colunas
             - dar join com outras tabelas
@@ -359,15 +359,15 @@
         for col in columns:
             name = col.get("name")
             bigquery_type = (
                 "STRING" if col.get("type") is None else col.get("type").upper()
             )
 
             publish_txt += f"SAFE_CAST({name} AS {bigquery_type}) {name},\n"
-        ## remove last comma
+        # remove last comma
         publish_txt = publish_txt[:-2] + "\n"
 
         # add from statement
         project_id_staging = self.client["bigquery_staging"].project
         publish_txt += (
             f"FROM {project_id_staging}.{self.dataset_id}_staging.{self.table_id} AS t"
         )
@@ -687,15 +687,15 @@
                 columns=self._get_cross_columns_from_bq_api()
             )
         if mode == "prod" and custom_schema is not None:
             table.schema = self._load_schema_from_json(custom_schema)
 
         fields = ["description", "schema"]
 
-        self.client[f"bigquery_prod"].update_table(table, fields=fields)
+        self.client["bigquery_prod"].update_table(table, fields=fields)
 
         logger.success(
             " {object} {object_id} was {action} in {mode}!",
             object_id=self.table_id,
             mode=mode,
             object="Table",
             action="updated",
@@ -728,23 +728,23 @@
         # TODO: review this method
 
         if if_exists == "replace" and self.table_exists(mode="prod"):
             self.delete(mode="prod")
 
         publish_sql = self._make_publish_sql()
 
-        ## create view using API metadata
+        # create view using API metadata
         if custon_publish_sql is None:
             self.client["bigquery_prod"].query(publish_sql).result()
             self.update(mode="prod")
 
-        ## create view using custon query
+        # create view using custon query
         if custon_publish_sql is not None:
             self.client["bigquery_prod"].query(custon_publish_sql).result()
-            ## update schema using a custom schema
+            # update schema using a custom schema
             if custom_schema is not None:
                 self.update(custom_schema=custom_schema)
 
         logger.success(
             " {object} {object_id} was {action}!",
             object_id=self.table_id,
             object="Table",
@@ -813,18 +813,15 @@
                 This must be a multiple of 256 KB per the API specification.
                 If not specified, the chunk_size of the blob itself is used. If that is not specified, a default value of 40 MB is used.
         """
         if not self.table_exists("staging"):
             raise BaseDosDadosException(
                 "You cannot append to a table that does not exist"
             )
-        Storage(
-            self.dataset_id,
-            self.table_id,
-        ).upload(
+        Storage(self.dataset_id, self.table_id,).upload(
             filepath,
             mode="staging",
             partitions=partitions,
             if_exists=if_exists,
             chunk_size=chunk_size,
             **upload_args,
         )
```

### Comparing `basedosdados-2.0.0b8/basedosdados/upload/utils.py` & `basedosdados-2.0.0b9/basedosdados/upload/utils.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ Utilities functions for Upload sub-module"""
 # pylint: disable=invalid-name,too-many-arguments,too-many-locals,too-many-branches,too-many-statements, protected-access,line-too-long
-from typing import List
-from pathlib import Path
 import os
+from pathlib import Path
+from typing import List
 
 import pandas as pd
 
 
 def to_partitions(data: pd.DataFrame, partition_columns: List[str], savepath: str):
     """Save data in to hive patitions schema, given a dataframe and a list of partition columns.
     Args:
```

### Comparing `basedosdados-2.0.0b8/pyproject.toml` & `basedosdados-2.0.0b9/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,58 @@
 [tool.poetry]
+name = "basedosdados"
+version = "2.0.0-beta.9"
+description = "Organizar e facilitar o acesso a dados brasileiros através de tabelas públicas no BigQuery."
 authors = ["Joao Carabetta <joao.carabetta@gmail.com>", "Ricardo Dahis", "Diego Oliveira"]
 classifiers = [
-  "Topic :: Software Development :: Build Tools",
-  "Topic :: Software Development :: Libraries :: Python Modules",
+    "Topic :: Software Development :: Build Tools",
+    "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-description = "Organizar e facilitar o acesso a dados brasileiros através de tabelas públicas no BigQuery."
-homepage = "https://github.com/base-dos-dados/bases"
+homepage = "https://github.com/basedosdados/mais"
+repository = "https://github.com/basedosdados/mais"
 license = "MIT"
-name = "basedosdados"
+readme = "README.md"
 packages = [
-  {include = "basedosdados"},
+    {include = "basedosdados"},
 ]
-readme = "README.md"
-repository = "https://github.com/base-dos-dados/bases"
-version = "2.0.0-beta.8"
+
+[tool.poetry.dependencies]
+python = ">=3.8.1,<4"
+google-api-python-client = "^2.86"
+google-cloud-bigquery = "^3.10"
+google-cloud-bigquery-connection = "^1.12"
+google-cloud-bigquery-storage = "^2.19"
+google-cloud-storage = "^2.9"
+gql = { version = "^3.4", optional = true }
+loguru = "^0.6"
+pandas = "^2.0"
+pandas-gbq = "^0.19"
+pandavro = { version = "^1.7", optional = true }
+pydata-google-auth = "^1.8"
+requests-toolbelt = { version = "^1", optional = true }
+tomlkit = "^0.11"
+tqdm = "^4"
+click = { version = ">=8.1,<9", optional = true }
+
+[tool.poetry.extras]
+avro = ["pandavro"]
+cli = ["click"]
+upload = ["gql", "requests-toolbelt"]
+
+[tool.poetry.group.dev.dependencies]
+black = "^23.7.0"
+flake8 = "^6.1.0"
+isort = "^5.12.0"
+pre-commit = "^3.3.3"
+semgrep = "^1.36.0"
+taskipy = "^1.12.0"
 
 [tool.poetry.scripts]
 basedosdados = 'basedosdados.cli.cli:cli'
 
-[tool.poetry.dependencies]
-google-api-python-client = "^2.86.0"
-google-cloud-bigquery = "^3.10.0"
-google-cloud-bigquery-connection = "^1.12.0"
-google-cloud-bigquery-storage = "^2.19.1"
-google-cloud-storage = "^2.9.0"
-gql = "^3.4.1"
-loguru = "^0.7.0"
-pandas = "^2.0.1"
-pandas-gbq = "^0.19.2"
-pandavro = "^1.7.2"
-pydata-google-auth = "^1.8.0"
-python = ">=3.8, <3.11"
-requests-toolbelt = "^1.0.0"
-tomlkit = "^0.11.8"
-tqdm = "^4.65.0"
-
 [tool.black]
 # Use the more relaxed max line length permitted in PEP8.
 exclude = '''
 /(
     \.eggs
   | \.git
   | \.mypy_cache
@@ -46,15 +60,21 @@
   | \venv
   | build
   | dist
   | htmlcov
 )/
 '''
 line-length = 88
-target-version = ["py36", "py37", "py38", "py39"]
+target-version = ["py38", "py39", "py310"]
+
+[tool.isort]
+profile = "black"
+
+[tool.taskipy.tasks]
+lint = "semgrep scan --error --config auto --exclude-rule yaml.github-actions.security.third-party-action-not-pinned-to-commit-sha.third-party-action-not-pinned-to-commit-sha && black . && isort . && flake8 ."
 
 [build-system]
-build-backend = "poetry.masonry.api"
-requires = ["poetry>=0.12"]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
 
 [pytest]
 addopts = "-p no:warnings"
```

### Comparing `basedosdados-2.0.0b8/PKG-INFO` & `basedosdados-2.0.0b9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 Metadata-Version: 2.1
 Name: basedosdados
-Version: 2.0.0b8
+Version: 2.0.0b9
 Summary: Organizar e facilitar o acesso a dados brasileiros através de tabelas públicas no BigQuery.
-Home-page: https://github.com/base-dos-dados/bases
+Home-page: https://github.com/basedosdados/mais
 License: MIT
 Author: Joao Carabetta
 Author-email: joao.carabetta@gmail.com
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8.1,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: google-api-python-client (>=2.86.0,<3.0.0)
-Requires-Dist: google-cloud-bigquery (>=3.10.0,<4.0.0)
-Requires-Dist: google-cloud-bigquery-connection (>=1.12.0,<2.0.0)
-Requires-Dist: google-cloud-bigquery-storage (>=2.19.1,<3.0.0)
-Requires-Dist: google-cloud-storage (>=2.9.0,<3.0.0)
-Requires-Dist: gql (>=3.4.1,<4.0.0)
-Requires-Dist: loguru (>=0.7.0,<0.8.0)
-Requires-Dist: pandas (>=2.0.1,<3.0.0)
-Requires-Dist: pandas-gbq (>=0.19.2,<0.20.0)
-Requires-Dist: pandavro (>=1.7.2,<2.0.0)
-Requires-Dist: pydata-google-auth (>=1.8.0,<2.0.0)
-Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
-Requires-Dist: tomlkit (>=0.11.8,<0.12.0)
-Requires-Dist: tqdm (>=4.65.0,<5.0.0)
-Project-URL: Repository, https://github.com/base-dos-dados/bases
+Provides-Extra: avro
+Provides-Extra: cli
+Provides-Extra: upload
+Requires-Dist: click (>=8.1,<9) ; extra == "cli"
+Requires-Dist: google-api-python-client (>=2.86,<3.0)
+Requires-Dist: google-cloud-bigquery (>=3.10,<4.0)
+Requires-Dist: google-cloud-bigquery-connection (>=1.12,<2.0)
+Requires-Dist: google-cloud-bigquery-storage (>=2.19,<3.0)
+Requires-Dist: google-cloud-storage (>=2.9,<3.0)
+Requires-Dist: gql (>=3.4,<4.0) ; extra == "upload"
+Requires-Dist: loguru (>=0.6,<0.7)
+Requires-Dist: pandas (>=2.0,<3.0)
+Requires-Dist: pandas-gbq (>=0.19,<0.20)
+Requires-Dist: pandavro (>=1.7,<2.0) ; extra == "avro"
+Requires-Dist: pydata-google-auth (>=1.8,<2.0)
+Requires-Dist: requests-toolbelt (>=1,<2) ; extra == "upload"
+Requires-Dist: tomlkit (>=0.11,<0.12)
+Requires-Dist: tqdm (>=4,<5)
+Project-URL: Repository, https://github.com/basedosdados/mais
 Description-Content-Type: text/markdown
 
 # Python Package
 
-## Desenvolvimento Linux e Mac: 
+## Desenvolvimento Linux e Mac:
 
 Clone o repositório principal:
 
 ```sh
 git clone https://github.com/basedosdados/mais.git
 ```
 Entre na pasta local do repositório usando `cd mais/` e suba o ambiente localmente:
@@ -49,50 +53,50 @@
 python setup.py develop
 ```
 
 ### Desenvolva uma nova feature
 
 1. Abra uma branch com o nome issue-<X>
 2. Faça as modificações necessárias
-3. Suba o Pull Request apontando para a branch `python-next-minor` ou `python-next-patch`. 
+3. Suba o Pull Request apontando para a branch `python-next-minor` ou `python-next-patch`.
     Sendo, minor e patch referentes ao bump da versão: v1.5.7 --> v\<major>.\<minor>.\<patch>.
 4. O nome do PR deve seguir o padrão
     `[infra] <titulo explicativo>`
 
 
 ### O que uma modificação precisa ter
 
-  
+
 - Resolver o problema
 - Lista de modificações efetuadas
     1. Mudei a função X para fazer Y
     2. Troquei o nome da variavel Z
 - Referência aos issues atendidos
 - Documentação e Docstrings
 - Testes
-  
+
 
 ## Versionamento
 
 **Para publicar uma nova versão do pacote é preciso seguir os seguintes passos:**
 
 1. Fazer o pull da branch:
 
     ```bash
     git pull origin [python-version]
     ```
-  
+
     Onde `[python-version]` é a branch da nova versão do pacote.
 
 2. Se necessario adicionar novas dependências:
     ```bash
       poetry add <package-name>
     ```
 
-3. Gerar novo `requirements-dev.txt` 
+3. Gerar novo `requirements-dev.txt`
 
     ```bash
     poetry export -f requirements.txt --output requirements-dev.txt --without-hashes
     ```
 
 4. Editar `pyproject.toml`:
 
@@ -106,27 +110,27 @@
     packages = [
       {include = "basedosdados"},
     ]
     readme = "README.md"
     repository = "https://github.com/base-dos-dados/bases"
     version = "1.6.1-beta.2"
     ```
-    
+
     O campo `version` deve ser alterado para o número da versão sendo lançada.
 
 5. Push para branch:
 
     ```bash
     git push origin [python-version]
     ```
 
 6. Publicação do pacote no PyPI (exige usuário e senha):
 
     Para publicar o pacote no PyPI, use:
-    
+
     ```bash
     poetry version [python-version]
     poetry publish --build
     ```
 
 7. Faz merge da branch para a master
 8. Faz release usando a UI do GitHub
```

