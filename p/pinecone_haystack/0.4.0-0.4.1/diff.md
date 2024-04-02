# Comparing `tmp/pinecone_haystack-0.4.0.tar.gz` & `tmp/pinecone_haystack-0.4.1.tar.gz`

## Comparing `pinecone_haystack-0.4.0.tar` & `pinecone_haystack-0.4.1.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.0/examples/example.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.0/pydoc/config.yml
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.0/src/haystack_integrations/components/retrievers/pinecone/__init__.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.0/src/haystack_integrations/components/retrievers/pinecone/embedding_retriever.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.0/src/haystack_integrations/document_stores/pinecone/__init__.py
--rw-r--r--   0        0        0    11936 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.0/src/haystack_integrations/document_stores/pinecone/document_store.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.0/src/haystack_integrations/document_stores/pinecone/errors.py
--rw-r--r--   0        0        0     6065 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.0/src/haystack_integrations/document_stores/pinecone/filters.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0     4749 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.0/tests/test_document_store.py
--rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.0/tests/test_emebedding_retriever.py
--rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.0/tests/test_filters.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.0/.gitignore
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.0/README.md
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.1/examples/example.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.1/pydoc/config.yml
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.1/src/haystack_integrations/components/retrievers/pinecone/__init__.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.1/src/haystack_integrations/components/retrievers/pinecone/embedding_retriever.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.1/src/haystack_integrations/document_stores/pinecone/__init__.py
+-rw-r--r--   0        0        0    12194 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.1/src/haystack_integrations/document_stores/pinecone/document_store.py
+-rw-r--r--   0        0        0     6065 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.1/src/haystack_integrations/document_stores/pinecone/filters.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.1/tests/conftest.py
+-rw-r--r--   0        0        0     5486 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.1/tests/test_document_store.py
+-rw-r--r--   0        0        0     4464 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.1/tests/test_emebedding_retriever.py
+-rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.1/tests/test_filters.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.1/.gitignore
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.1/README.md
+-rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 pinecone_haystack-0.4.1/PKG-INFO
```

### Comparing `pinecone_haystack-0.4.0/examples/example.py` & `pinecone_haystack-0.4.1/examples/example.py`

 * *Files identical despite different names*

### Comparing `pinecone_haystack-0.4.0/src/haystack_integrations/document_stores/pinecone/document_store.py` & `pinecone_haystack-0.4.1/src/haystack_integrations/document_stores/pinecone/document_store.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 # Pinecone has a limit of 1000 documents that can be returned in a query
 # with include_metadata=True or include_data=True
 # https://docs.pinecone.io/docs/limits
 TOP_K_LIMIT = 1_000
 
 
 class PineconeDocumentStore:
+    """
+    A Document Store using [Pinecone vector database](https://www.pinecone.io/).
+    """
+
     def __init__(
         self,
         *,
         api_key: Secret = Secret.from_env_var("PINECONE_API_KEY"),  # noqa: B008
         environment: str = "us-west1-gcp",
         index: str = "default",
         namespace: str = "default",
@@ -37,41 +41,30 @@
         dimension: int = 768,
         **index_creation_kwargs,
     ):
         """
         Creates a new PineconeDocumentStore instance.
         It is meant to be connected to a Pinecone index and namespace.
 
-        :param api_key: The Pinecone API key. It can be explicitly provided or automatically read from the
-            environment variable PINECONE_API_KEY (recommended).
-        :param environment: The Pinecone environment to connect to. Defaults to "us-west1-gcp".
+        :param api_key: The Pinecone API key.
+        :param environment: The Pinecone environment to connect to.
         :param index: The Pinecone index to connect to. If the index does not exist, it will be created.
-            Defaults to "default".
         :param namespace: The Pinecone namespace to connect to. If the namespace does not exist, it will be created
-            at the first write. Defaults to "default".
-        :param batch_size: The number of documents to write in a single batch. Defaults to 100, as recommended by
-            Pinecone.
+            at the first write.
+        :param batch_size: The number of documents to write in a single batch. When setting this parameter,
+            consider [documented Pinecone limits](https://docs.pinecone.io/docs/limits).
         :param dimension: The dimension of the embeddings. This parameter is only used when creating a new index.
-            Defaults to 768.
         :param index_creation_kwargs: Additional keyword arguments to pass to the index creation method.
-            For example, you can specify `metric`, `pods`, `replicas`...
             You can find the full list of supported arguments in the
-            [API reference](https://docs.pinecone.io/reference/create_index-1).
+            [API reference](https://docs.pinecone.io/reference/create_index).
 
         """
-        resolved_api_key = api_key.resolve_value()
-        if resolved_api_key is None:
-            msg = (
-                "PineconeDocumentStore expects an API key. "
-                "Set the PINECONE_API_KEY environment variable (recommended) or pass it explicitly."
-            )
-            raise ValueError(msg)
         self.api_key = api_key
 
-        pinecone.init(api_key=resolved_api_key, environment=environment)
+        pinecone.init(api_key=api_key.resolve_value(), environment=environment)
 
         if index not in pinecone.list_indexes():
             logger.info(f"Index {index} does not exist. Creating a new index.")
             pinecone.create_index(name=index, dimension=dimension, **index_creation_kwargs)
         else:
             logger.info(f"Index {index} already exists. Connecting to it.")
 
@@ -91,18 +84,30 @@
         self.index = index
         self.namespace = namespace
         self.batch_size = batch_size
         self.index_creation_kwargs = index_creation_kwargs
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "PineconeDocumentStore":
+        """
+        Deserializes the component from a dictionary.
+        :param data:
+            Dictionary to deserialize from.
+        :returns:
+            Deserialized component.
+        """
         deserialize_secrets_inplace(data["init_parameters"], keys=["api_key"])
         return default_from_dict(cls, data)
 
     def to_dict(self) -> Dict[str, Any]:
+        """
+        Serializes the component to a dictionary.
+        :returns:
+            Dictionary with serialized data.
+        """
         return default_to_dict(
             self,
             api_key=self.api_key.to_dict(),
             environment=self.environment,
             index=self.index,
             dimension=self.dimension,
             namespace=self.namespace,
@@ -124,15 +129,15 @@
         """
         Writes Documents to Pinecone.
 
         :param documents: A list of Documents to write to the document store.
         :param policy: The duplicate policy to use when writing documents.
             PineconeDocumentStore only supports `DuplicatePolicy.OVERWRITE`.
 
-        :return: The number of documents written to the document store.
+        :returns: The number of documents written to the document store.
         """
         if len(documents) > 0 and not isinstance(documents[0], Document):
             msg = "param 'documents' must contain a list of objects of type Document"
             raise ValueError(msg)
 
         if policy not in [DuplicatePolicy.NONE, DuplicatePolicy.OVERWRITE]:
             logger.warning(
@@ -153,15 +158,15 @@
         """
         Returns the documents that match the filters provided.
 
         For a detailed specification of the filters,
         refer to the [documentation](https://docs.haystack.deepset.ai/v2.0/docs/metadata-filtering)
 
         :param filters: The filters to apply to the document list.
-        :return: A list of Documents that match the given filters.
+        :returns: A list of Documents that match the given filters.
         """
 
         # Pinecone only performs vector similarity search
         # here we are querying with a dummy vector and the max compatible top_k
         documents = self._embedding_retrieval(query_embedding=self._dummy_vector, filters=filters, top_k=TOP_K_LIMIT)
 
         # when simply filtering, we don't want to return any scores
@@ -174,15 +179,15 @@
                 f"PineconeDocumentStore can return at most {TOP_K_LIMIT} documents and the query has hit this limit. "
                 f"It is likely that there are more matching documents in the document store. "
             )
         return documents
 
     def delete_documents(self, document_ids: List[str]) -> None:
         """
-        Deletes all documents with a matching document_ids from the document store.
+        Deletes documents that match the provided `document_ids` from the document store.
 
         :param document_ids: the document ids to delete
         """
         self._index.delete(ids=document_ids, namespace=self.namespace)
 
     def _embedding_retrieval(
         self,
@@ -193,22 +198,22 @@
         top_k: int = 10,
     ) -> List[Document]:
         """
         Retrieves documents that are most similar to the query embedding using a vector similarity metric.
 
         This method is not mean to be part of the public interface of
         `PineconeDocumentStore` nor called directly.
-        `PineconeDenseRetriever` uses this method directly and is the public interface for it.
+        `PineconeEmbeddingRetriever` uses this method directly and is the public interface for it.
 
         :param query_embedding: Embedding of the query.
         :param namespace: Pinecone namespace to query. Defaults the namespace of the document store.
-        :param filters: Filters applied to the retrieved Documents. Defaults to None.
-        :param top_k: Maximum number of Documents to return, defaults to 10
+        :param filters: Filters applied to the retrieved Documents.
+        :param top_k: Maximum number of Documents to return.
 
-        :return: List of Document that are most similar to `query_embedding`
+        :returns: List of Document that are most similar to `query_embedding`
         """
 
         if not query_embedding:
             msg = "query_embedding must be a non-empty list of floats"
             raise ValueError(msg)
 
         if filters and "operator" not in filters and "conditions" not in filters:
@@ -275,10 +280,17 @@
             # currently, storing blob in Pinecone is not supported
             if document.blob is not None:
                 logger.warning(
                     f"Document {document.id} has the `blob` field set, but storing `ByteStream` "
                     "objects in Pinecone is not supported. "
                     "The content of the `blob` field will be ignored."
                 )
+            if hasattr(document, "sparse_embedding") and document.sparse_embedding is not None:
+                logger.warning(
+                    "Document %s has the `sparse_embedding` field set,"
+                    "but storing sparse embeddings in Pinecone is not currently supported."
+                    "The `sparse_embedding` field will be ignored.",
+                    document.id,
+                )
 
             documents_for_pinecone.append(doc_for_pinecone)
         return documents_for_pinecone
```

### Comparing `pinecone_haystack-0.4.0/src/haystack_integrations/document_stores/pinecone/filters.py` & `pinecone_haystack-0.4.1/src/haystack_integrations/document_stores/pinecone/filters.py`

 * *Files identical despite different names*

### Comparing `pinecone_haystack-0.4.0/tests/conftest.py` & `pinecone_haystack-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pinecone_haystack-0.4.0/tests/test_document_store.py` & `pinecone_haystack-0.4.1/tests/test_document_store.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from unittest.mock import patch
 
 import numpy as np
 import pytest
 from haystack import Document
 from haystack.testing.document_store import CountDocumentsTest, DeleteDocumentsTest, WriteDocumentsTest
 from haystack.utils import Secret
@@ -46,26 +47,27 @@
         metric="euclidean",
     )
 
     mock_pinecone.init.assert_called_with(api_key="env-api-key", environment="gcp-starter")
 
 
 @patch("haystack_integrations.document_stores.pinecone.document_store.pinecone")
-def test_to_dict(mock_pinecone, monkeypatch):
+def test_to_from_dict(mock_pinecone, monkeypatch):
     mock_pinecone.Index.return_value.describe_index_stats.return_value = {"dimension": 30}
     monkeypatch.setenv("PINECONE_API_KEY", "env-api-key")
     document_store = PineconeDocumentStore(
         environment="gcp-starter",
         index="my_index",
         namespace="test",
         batch_size=50,
         dimension=30,
         metric="euclidean",
     )
-    assert document_store.to_dict() == {
+
+    dict_output = {
         "type": "haystack_integrations.document_stores.pinecone.document_store.PineconeDocumentStore",
         "init_parameters": {
             "api_key": {
                 "env_vars": [
                     "PINECONE_API_KEY",
                 ],
                 "strict": True,
@@ -75,39 +77,55 @@
             "index": "my_index",
             "dimension": 30,
             "namespace": "test",
             "batch_size": 50,
             "metric": "euclidean",
         },
     }
+    assert document_store.to_dict() == dict_output
+
+    document_store = PineconeDocumentStore.from_dict(dict_output)
+    assert document_store.environment == "gcp-starter"
+    assert document_store.api_key == Secret.from_env_var("PINECONE_API_KEY", strict=True)
+    assert document_store.index == "my_index"
+    assert document_store.namespace == "test"
+    assert document_store.batch_size == 50
+    assert document_store.dimension == 30
+
+
+def test_init_fails_wo_api_key(monkeypatch):
+    monkeypatch.delenv("PINECONE_API_KEY", raising=False)
+    with pytest.raises(ValueError):
+        PineconeDocumentStore(
+            environment="gcp-starter",
+            index="my_index",
+        )
 
 
 @pytest.mark.integration
+@pytest.mark.skipif("PINECONE_API_KEY" not in os.environ, reason="PINECONE_API_KEY not set")
 class TestDocumentStore(CountDocumentsTest, DeleteDocumentsTest, WriteDocumentsTest):
     def test_write_documents(self, document_store: PineconeDocumentStore):
         docs = [Document(id="1")]
         assert document_store.write_documents(docs) == 1
 
+    @pytest.mark.xfail(
+        run=True, reason="Pinecone supports overwriting by default, but it takes a while for it to take effect"
+    )
+    def test_write_documents_duplicate_overwrite(self, document_store: PineconeDocumentStore): ...
+
     @pytest.mark.skip(reason="Pinecone only supports UPSERT operations")
     def test_write_documents_duplicate_fail(self, document_store: PineconeDocumentStore): ...
 
     @pytest.mark.skip(reason="Pinecone only supports UPSERT operations")
     def test_write_documents_duplicate_skip(self, document_store: PineconeDocumentStore): ...
 
     @pytest.mark.skip(reason="Pinecone creates a namespace only when the first document is written")
     def test_delete_documents_empty_document_store(self, document_store: PineconeDocumentStore): ...
 
-    def test_init_fails_wo_api_key(self, monkeypatch):
-        monkeypatch.delenv("PINECONE_API_KEY", raising=False)
-        with pytest.raises(ValueError):
-            PineconeDocumentStore(
-                environment="gcp-starter",
-                index="my_index",
-            )
-
     def test_embedding_retrieval(self, document_store: PineconeDocumentStore):
         query_embedding = [0.1] * 768
         most_similar_embedding = [0.8] * 768
         second_best_embedding = [0.8] * 700 + [0.1] * 3 + [0.2] * 65
         another_embedding = np.random.rand(768).tolist()
 
         docs = [
```

### Comparing `pinecone_haystack-0.4.0/tests/test_emebedding_retriever.py` & `pinecone_haystack-0.4.1/tests/test_emebedding_retriever.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # SPDX-FileCopyrightText: 2023-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
 from unittest.mock import Mock, patch
 
 from haystack.dataclasses import Document
+from haystack.utils import Secret
 
 from haystack_integrations.components.retrievers.pinecone import PineconeEmbeddingRetriever
 from haystack_integrations.document_stores.pinecone import PineconeDocumentStore
 
 
 def test_init_default():
     mock_store = Mock(spec=PineconeDocumentStore)
@@ -59,14 +60,21 @@
 @patch("haystack_integrations.document_stores.pinecone.document_store.pinecone")
 def test_from_dict(mock_pinecone, monkeypatch):
     data = {
         "type": "haystack_integrations.components.retrievers.pinecone.embedding_retriever.PineconeEmbeddingRetriever",
         "init_parameters": {
             "document_store": {
                 "init_parameters": {
+                    "api_key": {
+                        "env_vars": [
+                            "PINECONE_API_KEY",
+                        ],
+                        "strict": True,
+                        "type": "env_var",
+                    },
                     "environment": "gcp-starter",
                     "index": "default",
                     "namespace": "test-namespace",
                     "batch_size": 50,
                     "dimension": 512,
                 },
                 "type": "haystack_integrations.document_stores.pinecone.document_store.PineconeDocumentStore",
@@ -78,14 +86,15 @@
 
     mock_pinecone.Index.return_value.describe_index_stats.return_value = {"dimension": 512}
     monkeypatch.setenv("PINECONE_API_KEY", "test-key")
     retriever = PineconeEmbeddingRetriever.from_dict(data)
 
     document_store = retriever.document_store
     assert document_store.environment == "gcp-starter"
+    assert document_store.api_key == Secret.from_env_var("PINECONE_API_KEY", strict=True)
     assert document_store.index == "default"
     assert document_store.namespace == "test-namespace"
     assert document_store.batch_size == 50
     assert document_store.dimension == 512
 
     assert retriever.filters == {}
     assert retriever.top_k == 10
```

### Comparing `pinecone_haystack-0.4.0/.gitignore` & `pinecone_haystack-0.4.1/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -130,7 +130,8 @@
 .pyre/
 
 # IDEs
 .vscode
 
 # Docs generation artifacts
 _readme_*.md
+.idea
```

### Comparing `pinecone_haystack-0.4.0/README.md` & `pinecone_haystack-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pinecone_haystack-0.4.0/pyproject.toml` & `pinecone_haystack-0.4.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -71,20 +71,20 @@
 fmt = ["black {args:.}", "ruff --fix {args:.}", "style"]
 all = ["style", "typing"]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.black]
-target-version = ["py37"]
+target-version = ["py38"]
 line-length = 120
 skip-string-normalization = true
 
 [tool.ruff]
-target-version = "py37"
+target-version = "py38"
 line-length = 120
 select = [
   "A",
   "ARG",
   "B",
   "C",
   "DTZ",
@@ -139,25 +139,27 @@
 [tool.ruff.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 # examples can contain "print" commands
 "examples/**/*" = ["T201"]
 
 [tool.coverage.run]
-source_pkgs = ["src", "tests"]
+source = ["haystack_integrations"]
 branch = true
-parallel = true
-omit = ["examples"]
+parallel = false
 
-[tool.coverage.paths]
-pinecone_haystack = ["src/*"]
-tests = ["tests"]
 
 [tool.coverage.report]
-exclude_lines = ["no cov", "if __name__ == .__main__.:", "if TYPE_CHECKING:"]
+omit = ["*/tests/*", "*/__init__.py"]
+show_missing=true
+exclude_lines = [
+  "no cov",
+  "if __name__ == .__main__.:",
+  "if TYPE_CHECKING:",
+]
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 markers = ["unit: unit tests", "integration: integration tests"]
 
 [[tool.mypy.overrides]]
 module = ["pinecone.*", "haystack.*", "haystack_integrations.*", "pytest.*"]
```

### Comparing `pinecone_haystack-0.4.0/PKG-INFO` & `pinecone_haystack-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pinecone_haystack
-Version: 0.4.0
+Version: 0.4.1
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/pinecone#readme
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/pinecone
 Author-email: deepset GmbH <info@deepset.ai>
 License-Expression: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

