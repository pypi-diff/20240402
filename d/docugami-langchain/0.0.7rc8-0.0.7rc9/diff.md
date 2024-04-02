# Comparing `tmp/docugami_langchain-0.0.7rc8.tar.gz` & `tmp/docugami_langchain-0.0.7rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docugami_langchain-0.0.7rc8.tar", max compression
+gzip compressed data, was "docugami_langchain-0.0.7rc9.tar", max compression
```

## Comparing `docugami_langchain-0.0.7rc8.tar` & `docugami_langchain-0.0.7rc9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1072 2024-03-07 04:54:41.910235 docugami_langchain-0.0.7rc8/LICENSE
--rw-r--r--   0        0        0      351 2024-03-07 04:54:41.910235 docugami_langchain-0.0.7rc8/README.md
--rw-r--r--   0        0        0      669 2024-03-07 04:54:41.910235 docugami_langchain-0.0.7rc8/docugami_langchain/__init__.py
--rw-r--r--   0        0        0      285 2024-03-07 04:54:41.910235 docugami_langchain-0.0.7rc8/docugami_langchain/agents/__init__.py
--rw-r--r--   0        0        0     4266 2024-03-07 04:54:41.910235 docugami_langchain-0.0.7rc8/docugami_langchain/agents/base.py
--rw-r--r--   0        0        0    13350 2024-03-07 04:54:41.910235 docugami_langchain-0.0.7rc8/docugami_langchain/agents/re_act_agent.py
--rw-r--r--   0        0        0     7878 2024-03-07 04:54:41.910235 docugami_langchain-0.0.7rc8/docugami_langchain/agents/re_woo_agent.py
--rw-r--r--   0        0        0     1849 2024-03-07 04:54:41.910235 docugami_langchain-0.0.7rc8/docugami_langchain/agents/rewrite_grader_agent.py
--rw-r--r--   0        0        0     9551 2024-03-07 04:54:41.910235 docugami_langchain-0.0.7rc8/docugami_langchain/base_runnable.py
--rw-r--r--   0        0        0      914 2024-03-07 04:54:41.910235 docugami_langchain-0.0.7rc8/docugami_langchain/chains/__init__.py
--rw-r--r--   0        0        0     2009 2024-03-07 04:54:41.910235 docugami_langchain-0.0.7rc8/docugami_langchain/chains/answer_chain.py
--rw-r--r--   0        0        0     6946 2024-03-07 04:54:41.910235 docugami_langchain-0.0.7rc8/docugami_langchain/chains/base.py
--rw-r--r--   0        0        0      243 2024-03-07 04:54:41.910235 docugami_langchain-0.0.7rc8/docugami_langchain/chains/chunks/__init__.py
--rw-r--r--   0        0        0     3255 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/chains/chunks/elaborate_chunk_chain.py
--rw-r--r--   0        0        0     3849 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/chains/chunks/summarize_chunk_chain.py
--rw-r--r--   0        0        0      291 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/chains/documents/__init__.py
--rw-r--r--   0        0        0     3834 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/chains/documents/describe_document_set_chain.py
--rw-r--r--   0        0        0     3852 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/chains/documents/summarize_document_chain.py
--rw-r--r--   0        0        0     3486 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/chains/helpers.py
--rw-r--r--   0        0        0     1098 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/chains/querying/__init__.py
--rw-r--r--   0        0        0     2909 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/chains/querying/docugami_explained_sql_query_chain.py
--rw-r--r--   0        0        0     3899 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/chains/querying/sql_fixup_chain.py
--rw-r--r--   0        0        0     4360 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/chains/querying/sql_query_explainer_chain.py
--rw-r--r--   0        0        0     8191 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/chains/querying/sql_result_chain.py
--rw-r--r--   0        0        0     3522 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/chains/querying/sql_result_explainer_chain.py
--rw-r--r--   0        0        0     2426 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/chains/querying/suggested_questions_chain.py
--rw-r--r--   0        0        0     3577 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/chains/querying/suggested_report_chain.py
--rw-r--r--   0        0        0      111 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/chains/rag/__init__.py
--rw-r--r--   0        0        0     3115 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/chains/rag/simple_rag_chain.py
--rw-r--r--   0        0        0      689 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/config.py
--rw-r--r--   0        0        0      109 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/document_loaders/__init__.py
--rw-r--r--   0        0        0    13516 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/document_loaders/docugami.py
--rw-r--r--   0        0        0      674 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/output_parsers/__init__.py
--rw-r--r--   0        0        0     1075 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/output_parsers/key_finding.py
--rw-r--r--   0        0        0     1073 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/output_parsers/line_separated_list.py
--rw-r--r--   0        0        0     1992 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/output_parsers/soft_react_json_single_input.py
--rw-r--r--   0        0        0     2816 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/output_parsers/sql_finding.py
--rw-r--r--   0        0        0     4502 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/output_parsers/timespan.py
--rw-r--r--   0        0        0      781 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/params.py
--rw-r--r--   0        0        0        0 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/py.typed
--rw-r--r--   0        0        0      165 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/retrievers/__init__.py
--rw-r--r--   0        0        0     5214 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/retrievers/fused_summary.py
--rw-r--r--   0        0        0     5615 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/retrievers/mappings.py
--rw-r--r--   0        0        0     5292 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/tools/reports.py
--rw-r--r--   0        0        0     5189 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/docugami_langchain/tools/retrieval.py
--rw-r--r--   0        0        0     2606 2024-03-07 04:54:41.914235 docugami_langchain-0.0.7rc8/pyproject.toml
--rw-r--r--   0        0        0     1452 1970-01-01 00:00:00.000000 docugami_langchain-0.0.7rc8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/LICENSE
+-rw-r--r--   0        0        0      351 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/README.md
+-rw-r--r--   0        0        0      669 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/__init__.py
+-rw-r--r--   0        0        0      285 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/agents/__init__.py
+-rw-r--r--   0        0        0     4266 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/agents/base.py
+-rw-r--r--   0        0        0    13322 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/agents/re_act_agent.py
+-rw-r--r--   0        0        0     7878 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/agents/re_woo_agent.py
+-rw-r--r--   0        0        0     1849 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/agents/rewrite_grader_agent.py
+-rw-r--r--   0        0        0    11094 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/base_runnable.py
+-rw-r--r--   0        0        0      914 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/__init__.py
+-rw-r--r--   0        0        0     2009 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/answer_chain.py
+-rw-r--r--   0        0        0     6946 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/base.py
+-rw-r--r--   0        0        0      243 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/chunks/__init__.py
+-rw-r--r--   0        0        0     3255 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/chunks/elaborate_chunk_chain.py
+-rw-r--r--   0        0        0     3849 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/chunks/summarize_chunk_chain.py
+-rw-r--r--   0        0        0      291 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/documents/__init__.py
+-rw-r--r--   0        0        0     3834 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/documents/describe_document_set_chain.py
+-rw-r--r--   0        0        0     3852 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/documents/summarize_document_chain.py
+-rw-r--r--   0        0        0     3486 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/helpers.py
+-rw-r--r--   0        0        0     1098 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/__init__.py
+-rw-r--r--   0        0        0     2909 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/docugami_explained_sql_query_chain.py
+-rw-r--r--   0        0        0     3899 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/sql_fixup_chain.py
+-rw-r--r--   0        0        0     4360 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/sql_query_explainer_chain.py
+-rw-r--r--   0        0        0     8191 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/sql_result_chain.py
+-rw-r--r--   0        0        0     3522 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/sql_result_explainer_chain.py
+-rw-r--r--   0        0        0     2426 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/suggested_questions_chain.py
+-rw-r--r--   0        0        0     3577 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/suggested_report_chain.py
+-rw-r--r--   0        0        0      111 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/rag/__init__.py
+-rw-r--r--   0        0        0     3115 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/rag/simple_rag_chain.py
+-rw-r--r--   0        0        0      689 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/config.py
+-rw-r--r--   0        0        0      109 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/document_loaders/__init__.py
+-rw-r--r--   0        0        0    13516 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/document_loaders/docugami.py
+-rw-r--r--   0        0        0      674 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/output_parsers/__init__.py
+-rw-r--r--   0        0        0     1075 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/output_parsers/key_finding.py
+-rw-r--r--   0        0        0     1073 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/output_parsers/line_separated_list.py
+-rw-r--r--   0        0        0     1992 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/output_parsers/soft_react_json_single_input.py
+-rw-r--r--   0        0        0     2816 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/output_parsers/sql_finding.py
+-rw-r--r--   0        0        0     4502 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/output_parsers/timespan.py
+-rw-r--r--   0        0        0      781 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/params.py
+-rw-r--r--   0        0        0        0 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/py.typed
+-rw-r--r--   0        0        0      165 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/retrievers/__init__.py
+-rw-r--r--   0        0        0     5214 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/retrievers/fused_summary.py
+-rw-r--r--   0        0        0     5615 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/retrievers/mappings.py
+-rw-r--r--   0        0        0     5292 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/tools/reports.py
+-rw-r--r--   0        0        0     5189 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/tools/retrieval.py
+-rw-r--r--   0        0        0     2606 2024-03-17 01:01:38.636537 docugami_langchain-0.0.7rc9/pyproject.toml
+-rw-r--r--   0        0        0     1452 1970-01-01 00:00:00.000000 docugami_langchain-0.0.7rc9/PKG-INFO
```

### Comparing `docugami_langchain-0.0.7rc8/LICENSE` & `docugami_langchain-0.0.7rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/__init__.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/agents/base.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/agents/base.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/agents/re_act_agent.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/agents/re_act_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,17 +160,15 @@
         raise NotImplementedError()
 
     def runnable(self) -> Runnable:
         """
         Custom runnable for this chain.
         """
 
-        def format_chat_history(
-            chat_history: list[tuple[str, str]]
-        ) -> list[BaseMessage]:
+        def format_chat_history(chat_history: list[tuple[str, str]]) -> list[BaseMessage]:
             messages: list[BaseMessage] = []
 
             if chat_history:
                 for human, ai in chat_history:
                     messages.append(HumanMessage(content=human))
                     messages.append(AIMessage(content=ai))
             return messages
@@ -213,17 +211,15 @@
             ]
         )
 
         agent_runnable: Runnable = (
             {
                 "question": lambda x: x["question"],
                 "chat_history": lambda x: format_chat_history(x["chat_history"]),
-                "agent_scratchpad": lambda x: format_log_to_str(
-                    x["intermediate_steps"]
-                ),
+                "agent_scratchpad": lambda x: format_log_to_str(x["intermediate_steps"]),
                 "tools": lambda x: render_text_description(self.tools),
                 "tool_names": lambda x: ", ".join([t.name for t in self.tools]),
             }
             | prompt
             | self.llm.bind(stop=["\nObservation"])
             | SoftReActJsonSingleInputOutputParser()
         )
@@ -251,16 +247,16 @@
             else:
                 return "continue"
 
         # Define a new graph
         workflow = StateGraph(ReActState)
 
         # Define the two nodes we will cycle between
-        workflow.add_node("agent", run_agent)
-        workflow.add_node("action", execute_tools)
+        workflow.add_node("agent", run_agent)  # type: ignore
+        workflow.add_node("action", execute_tools)  # type: ignore
 
         # Set the entrypoint as `agent`
         # This means that this node is the first one called
         workflow.set_entry_point("agent")
 
         # We now add a conditional edge
         workflow.add_conditional_edges(
```

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/agents/re_woo_agent.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/agents/re_woo_agent.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/agents/rewrite_grader_agent.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/agents/rewrite_grader_agent.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/base_runnable.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/base_runnable.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, AsyncIterator, Generic, Optional, TypeVar
 
 import yaml
 from langchain_community.vectorstores.faiss import FAISS
@@ -55,14 +56,51 @@
     input_template_list = ""
     for input in params.inputs:
         input_template_list += f"{input.key}: {{{input.variable}}}\n"
 
     return input_template_list.strip()
 
 
+def normalize_whitespace(text: str) -> str:
+    """
+    Normalizes whitespace in given text without affecting visual formatting.
+
+    This function aims to:
+    1. Compress multiple vertical whitespace (more than two newlines) into two newlines, without affecting horizontal whitespace (indentation).
+    2. Remove leading and trailing whitespace from the text.
+
+    >>> normalize_whitespace("  Hello\\n\\n\\nWorld  ")
+    'Hello\\n\\nWorld'
+    >>> normalize_whitespace("\\n\\n\\n    Indented text\\nMore indented text\\n\\n")
+    'Indented text\\nMore indented text'
+    >>> normalize_whitespace("No extra\\nwhitespace here.")
+    'No extra\\nwhitespace here.'
+    >>> normalize_whitespace("  \\n  Leading and trailing newlines and spaces  \\n  ")
+    'Leading and trailing newlines and spaces'
+    >>> normalize_whitespace("\\n\\n\\n\\nOnly newlines here\\n\\n\\n\\nHello")
+    'Only newlines here\\n\\nHello'
+
+    Note that horizontal spaces before and after the text in a single line are not preserved if they're at the beginning or end of the text.
+
+    Args:
+        text (str): The input text to normalize.
+
+    Returns:
+        str: The normalized text with whitespace adjusted.
+    """
+
+    # compress vertical whitespace without affecting horizontal whitespace (indentation)
+    text = re.sub(r"(\s*\n){3,}", "\n\n", text)
+
+    # remove leading and trailing whitespace
+    text = text.strip()
+
+    return text
+
+
 @dataclass
 class TracedResponse(Generic[T]):
     value: T
     run_id: str = ""
 
 
 class BaseRunnable(BaseModel, Generic[T], ABC):
@@ -119,28 +157,29 @@
         if not self.embeddings:
             raise Exception("Embedding model required to use few shot examples")
 
         with open(examples_yaml, "r", encoding="utf-8") as in_f:
             self._examples = yaml.safe_load(in_f)
 
             for ex in self._examples:
-                # truncate example length to avoid overflowing context too much
                 keys = ex.keys()
                 for k in keys:
+                    # whitespace normalize
+                    ex[k] = normalize_whitespace(ex[k])
+
+                    # truncate length to avoid overflowing context too much (strip any trailing whitespace again)
                     ex[k] = ex[k][: self.few_shot_params_max_length_cutoff].strip()
 
             if self._examples and num_examples:
                 try:
-                    self._example_selector = (
-                        SemanticSimilarityExampleSelector.from_examples(
-                            examples=self._examples,
-                            embeddings=self.embeddings,
-                            vectorstore_cls=self.examples_vectorstore_cls,
-                            k=num_examples,
-                        )
+                    self._example_selector = SemanticSimilarityExampleSelector.from_examples(
+                        examples=self._examples,
+                        embeddings=self.embeddings,
+                        vectorstore_cls=self.examples_vectorstore_cls,
+                        k=num_examples,
                     )
                 except Exception as exc:
                     details = f"Exception while loading samples from YAML {examples_yaml}. Details: {exc}"
                     raise Exception(details)
 
     def runnable(self) -> Runnable:
         """
@@ -157,17 +196,15 @@
             # For chat models, we need to make sure the output is a string
             full_runnable = full_runnable | StrOutputParser()
 
         if params.key_finding_output_parse:
             # Increase accuracy for models that require very specific output, by
             # looking for the output key however adding such an output parser disables
             # streaming, so use carefully
-            full_runnable = full_runnable | KeyfindingOutputParser(
-                output_key=params.output.key
-            )
+            full_runnable = full_runnable | KeyfindingOutputParser(output_key=params.output.key)
 
         if params.additional_runnables:
             for runnable in params.additional_runnables:
                 full_runnable = full_runnable | runnable
 
         return full_runnable
 
@@ -184,19 +221,20 @@
             config = merge_configs(config, arg_config)
 
             # kwargs are used as inputs to the chain prompt, so remove the config
             # param if specified
             del kwargs_dict[CONFIG_KEY]
 
         for key in kwargs_dict:
-            # for string args, cap at max to avoid chance of prompt overflow
             if isinstance(kwargs_dict[key], str):
-                kwargs_dict[key] = kwargs_dict[key][
-                    : self.input_params_max_length_cutoff
-                ]
+                # whitespace normalize
+                kwargs_dict[key] = normalize_whitespace(kwargs_dict[key])
+
+                # truncate length to avoid overflowing context too much (strip any trailing whitespace again)
+                kwargs_dict[key] = kwargs_dict[key][: self.few_shot_params_max_length_cutoff].strip()
 
         return config, kwargs_dict
 
     @abstractmethod
     def run(self, **kwargs) -> TracedResponse[T]:  # type: ignore
         config, kwargs_dict = self._prepare_run_args(kwargs)
         with collect_runs() as cb:
@@ -219,17 +257,15 @@
         if not isinstance(inputs, list):
             raise Exception("Input for batch processing must be a List")
 
         for input_dict in inputs:
             for key in input_dict:
                 # For string args, cap at max to avoid chance of prompt overflow
                 if isinstance(input_dict[key], str):
-                    input_dict[key] = input_dict[key][
-                        : self.input_params_max_length_cutoff
-                    ]
+                    input_dict[key] = input_dict[key][: self.input_params_max_length_cutoff]
 
         return self.runnable().batch(inputs=inputs, config=config)  # type: ignore
 
     @abstractmethod
     async def run_stream(self, **kwargs: Any) -> AsyncIterator[TracedResponse[T]]: ...
 
     @abstractmethod
```

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/chains/__init__.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/chains/answer_chain.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/chains/answer_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/chains/base.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/chains/base.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/chains/chunks/elaborate_chunk_chain.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/chains/chunks/elaborate_chunk_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/chains/chunks/summarize_chunk_chain.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/chains/chunks/summarize_chunk_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/chains/documents/describe_document_set_chain.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/chains/documents/describe_document_set_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/chains/documents/summarize_document_chain.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/chains/documents/summarize_document_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/chains/helpers.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/chains/helpers.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/chains/querying/__init__.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/chains/querying/docugami_explained_sql_query_chain.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/docugami_explained_sql_query_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/chains/querying/sql_fixup_chain.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/sql_fixup_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/chains/querying/sql_query_explainer_chain.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/sql_query_explainer_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/chains/querying/sql_result_chain.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/sql_result_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/chains/querying/sql_result_explainer_chain.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/sql_result_explainer_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/chains/querying/suggested_questions_chain.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/suggested_questions_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/chains/querying/suggested_report_chain.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/suggested_report_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/chains/rag/simple_rag_chain.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/chains/rag/simple_rag_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/config.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/config.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/document_loaders/docugami.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/document_loaders/docugami.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/output_parsers/__init__.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/output_parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/output_parsers/key_finding.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/output_parsers/key_finding.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/output_parsers/line_separated_list.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/output_parsers/line_separated_list.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/output_parsers/soft_react_json_single_input.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/output_parsers/soft_react_json_single_input.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/output_parsers/sql_finding.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/output_parsers/sql_finding.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/output_parsers/timespan.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/output_parsers/timespan.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/params.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/params.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/retrievers/fused_summary.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/retrievers/fused_summary.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/retrievers/mappings.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/retrievers/mappings.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/tools/reports.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/tools/reports.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/docugami_langchain/tools/retrieval.py` & `docugami_langchain-0.0.7rc9/docugami_langchain/tools/retrieval.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc8/pyproject.toml` & `docugami_langchain-0.0.7rc9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docugami-langchain"
-version = "0.0.7rc8"
+version = "0.0.7rc9"
 description = "An integration package connecting Docugami and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/docugami/docugami-langchain"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `docugami_langchain-0.0.7rc8/PKG-INFO` & `docugami_langchain-0.0.7rc9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docugami-langchain
-Version: 0.0.7rc8
+Version: 0.0.7rc9
 Summary: An integration package connecting Docugami and LangChain
 Home-page: https://github.com/docugami/docugami-langchain
 License: MIT
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

