# Comparing `tmp/langchain_cohere-0.1.0rc0.tar.gz` & `tmp/langchain_cohere-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_cohere-0.1.0rc0.tar", max compression
+gzip compressed data, was "langchain_cohere-0.1.0rc1.tar", max compression
```

## Comparing `langchain_cohere-0.1.0rc0.tar` & `langchain_cohere-0.1.0rc1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1072 2024-03-25 20:47:01.840585 langchain_cohere-0.1.0rc0/LICENSE
--rw-r--r--   0        0        0       19 2024-03-25 20:47:01.840585 langchain_cohere-0.1.0rc0/README.md
--rw-r--r--   0        0        0      349 2024-03-25 20:47:01.840585 langchain_cohere-0.1.0rc0/langchain_cohere/__init__.py
--rw-r--r--   0        0        0     8088 2024-03-25 20:47:01.840585 langchain_cohere-0.1.0rc0/langchain_cohere/chat_models.py
--rw-r--r--   0        0        0     5193 2024-03-25 20:47:01.840585 langchain_cohere-0.1.0rc0/langchain_cohere/embeddings.py
--rw-r--r--   0        0        0     7654 2024-03-25 20:47:01.840585 langchain_cohere-0.1.0rc0/langchain_cohere/llms.py
--rw-r--r--   0        0        0        0 2024-03-25 20:47:01.840585 langchain_cohere-0.1.0rc0/langchain_cohere/py.typed
--rw-r--r--   0        0        0     2915 2024-03-25 20:47:01.840585 langchain_cohere-0.1.0rc0/langchain_cohere/rag_retrievers.py
--rw-r--r--   0        0        0     3916 2024-03-25 20:47:01.840585 langchain_cohere-0.1.0rc0/langchain_cohere/rerank.py
--rw-r--r--   0        0        0      975 2024-03-25 20:47:01.840585 langchain_cohere-0.1.0rc0/langchain_cohere/utils.py
--rw-r--r--   0        0        0     2471 2024-03-25 20:47:01.840585 langchain_cohere-0.1.0rc0/pyproject.toml
--rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 langchain_cohere-0.1.0rc0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-03-28 19:12:51.649709 langchain_cohere-0.1.0rc1/LICENSE
+-rw-r--r--   0        0        0       19 2024-03-28 19:12:51.649709 langchain_cohere-0.1.0rc1/README.md
+-rw-r--r--   0        0        0      450 2024-03-28 19:12:51.649709 langchain_cohere-0.1.0rc1/langchain_cohere/__init__.py
+-rw-r--r--   0        0        0    12664 2024-03-28 19:12:51.649709 langchain_cohere-0.1.0rc1/langchain_cohere/chat_models.py
+-rw-r--r--   0        0        0     7496 2024-03-28 19:12:51.649709 langchain_cohere-0.1.0rc1/langchain_cohere/cohere_agent.py
+-rw-r--r--   0        0        0     5193 2024-03-28 19:12:51.649709 langchain_cohere-0.1.0rc1/langchain_cohere/embeddings.py
+-rw-r--r--   0        0        0     7654 2024-03-28 19:12:51.649709 langchain_cohere-0.1.0rc1/langchain_cohere/llms.py
+-rw-r--r--   0        0        0        0 2024-03-28 19:12:51.649709 langchain_cohere-0.1.0rc1/langchain_cohere/py.typed
+-rw-r--r--   0        0        0     2974 2024-03-28 19:12:51.649709 langchain_cohere-0.1.0rc1/langchain_cohere/rag_retrievers.py
+-rw-r--r--   0        0        0     3995 2024-03-28 19:12:51.649709 langchain_cohere-0.1.0rc1/langchain_cohere/rerank.py
+-rw-r--r--   0        0        0      975 2024-03-28 19:12:51.649709 langchain_cohere-0.1.0rc1/langchain_cohere/utils.py
+-rw-r--r--   0        0        0     2471 2024-03-28 19:12:51.649709 langchain_cohere-0.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 langchain_cohere-0.1.0rc1/PKG-INFO
```

### Comparing `langchain_cohere-0.1.0rc0/LICENSE` & `langchain_cohere-0.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.0rc0/langchain_cohere/embeddings.py` & `langchain_cohere-0.1.0rc1/langchain_cohere/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.0rc0/langchain_cohere/llms.py` & `langchain_cohere-0.1.0rc1/langchain_cohere/llms.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.0rc0/langchain_cohere/rag_retrievers.py` & `langchain_cohere-0.1.0rc1/langchain_cohere/rag_retrievers.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     from langchain_core.messages import BaseMessage
 
 
 def _get_docs(response: Any) -> List[Document]:
     docs = (
         []
         if "documents" not in response.generation_info
+        or len(response.generation_info["documents"]) == 0
         else [
             Document(page_content=doc["snippet"], metadata=doc)
             for doc in response.generation_info["documents"]
         ]
     )
     docs.append(
         Document(
```

### Comparing `langchain_cohere-0.1.0rc0/langchain_cohere/rerank.py` & `langchain_cohere-0.1.0rc1/langchain_cohere/rerank.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,18 +65,22 @@
             return []
         docs = [
             doc.page_content if isinstance(doc, Document) else doc for doc in documents
         ]
         model = model or self.model
         top_n = top_n if (top_n is None or top_n > 0) else self.top_n
         results = self.client.rerank(
-            query, docs, model, top_n=top_n, max_chunks_per_doc=max_chunks_per_doc
+            query=query,
+            documents=docs,
+            model=model,
+            top_n=top_n,
+            max_chunks_per_doc=max_chunks_per_doc,
         )
         result_dicts = []
-        for res in results:
+        for res in results.results:
             result_dicts.append(
                 {"index": res.index, "relevance_score": res.relevance_score}
             )
         return result_dicts
 
     def compress_documents(
         self,
```

### Comparing `langchain_cohere-0.1.0rc0/langchain_cohere/utils.py` & `langchain_cohere-0.1.0rc1/langchain_cohere/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.0rc0/pyproject.toml` & `langchain_cohere-0.1.0rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "langchain-cohere"
-version = "0.1.0rc0"
+version = "0.1.0rc1"
 description = "An integration package connecting Cohere and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/cohere"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 langchain-core = "^0.1.32"
-cohere = "^5.1.1"
+cohere = "^5.1.4"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
 freezegun = "^1.2.2"
```

### Comparing `langchain_cohere-0.1.0rc0/PKG-INFO` & `langchain_cohere-0.1.0rc1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: langchain-cohere
-Version: 0.1.0rc0
+Version: 0.1.0rc1
 Summary: An integration package connecting Cohere and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: cohere (>=5.1.1,<6.0.0)
+Requires-Dist: cohere (>=5.1.4,<6.0.0)
 Requires-Dist: langchain-core (>=0.1.32,<0.2.0)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/cohere
 Description-Content-Type: text/markdown
 
 # langchain-cohere
```

