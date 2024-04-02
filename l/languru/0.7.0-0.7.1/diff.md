# Comparing `tmp/languru-0.7.0.tar.gz` & `tmp/languru-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "languru-0.7.0.tar", max compression
+gzip compressed data, was "languru-0.7.1.tar", max compression
```

## Comparing `languru-0.7.0.tar` & `languru-0.7.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0    11357 2024-01-29 14:01:08.176794 languru-0.7.0/LICENSE
--rw-r--r--   0        0        0    10071 2024-03-17 14:45:00.663595 languru-0.7.0/README.md
--rw-r--r--   0        0        0        0 2024-01-29 14:05:50.312326 languru-0.7.0/languru/__init__.py
--rw-r--r--   0        0        0        0 2024-02-05 13:57:47.271478 languru-0.7.0/languru/action/__init__.py
--rw-r--r--   0        0        0     4891 2024-03-16 09:35:43.286010 languru-0.7.0/languru/action/base.py
--rw-r--r--   0        0        0     7655 2024-03-15 13:40:33.034768 languru-0.7.0/languru/action/google.py
--rw-r--r--   0        0        0     2816 2024-03-22 14:23:05.037171 languru-0.7.0/languru/action/groq.py
--rw-r--r--   0        0        0    18777 2024-03-15 13:47:24.662973 languru-0.7.0/languru/action/hf.py
--rw-r--r--   0        0        0     7339 2024-03-22 14:32:54.575174 languru-0.7.0/languru/action/openai.py
--rw-r--r--   0        0        0     2999 2024-03-22 14:32:25.897966 languru-0.7.0/languru/action/pplx.py
--rw-r--r--   0        0        0     1105 2024-03-22 13:37:34.206504 languru-0.7.0/languru/action/utils.py
--rw-r--r--   0        0        0        0 2024-01-30 14:23:22.088837 languru-0.7.0/languru/cli/__init__.py
--rw-r--r--   0        0        0     3327 2024-03-22 13:37:34.206678 languru-0.7.0/languru/cli/main.py
--rw-r--r--   0        0        0      221 2024-03-03 04:51:38.853780 languru-0.7.0/languru/config.py
--rw-r--r--   0        0        0        0 2024-03-16 05:09:45.252330 languru-0.7.0/languru/examples/__init__.py
--rw-r--r--   0        0        0        0 2024-03-16 05:10:17.853192 languru-0.7.0/languru/examples/return_values/__init__.py
--rw-r--r--   0        0        0     9704 2024-03-16 14:45:25.427960 languru-0.7.0/languru/examples/return_values/_openai.py
--rw-r--r--   0        0        0       41 2024-02-10 12:12:53.654103 languru-0.7.0/languru/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-03 10:10:03.421778 languru-0.7.0/languru/resources/__init__.py
--rw-r--r--   0        0        0        0 2024-02-03 10:19:09.963208 languru-0.7.0/languru/resources/llm/__init__.py
--rw-r--r--   0        0        0        0 2024-02-03 10:18:35.609130 languru-0.7.0/languru/resources/model/__init__.py
--rw-r--r--   0        0        0     4394 2024-03-10 02:36:17.112445 languru-0.7.0/languru/resources/model/discovery.py
--rw-r--r--   0        0        0        0 2024-01-29 14:28:54.637050 languru-0.7.0/languru/server/__init__.py
--rw-r--r--   0        0        0        0 2024-02-01 14:35:12.034189 languru-0.7.0/languru/server/api/__init__.py
--rw-r--r--   0        0        0      729 2024-02-10 12:03:18.878712 languru-0.7.0/languru/server/api/v1/__init__.py
--rw-r--r--   0        0        0     7533 2024-03-22 14:27:23.583494 languru-0.7.0/languru/server/api/v1/chat.py
--rw-r--r--   0        0        0     5796 2024-03-19 17:27:51.666346 languru-0.7.0/languru/server/api/v1/completions.py
--rw-r--r--   0        0        0     4423 2024-03-19 17:27:51.669771 languru-0.7.0/languru/server/api/v1/embeddings.py
--rw-r--r--   0        0        0     9679 2024-03-16 14:36:10.708408 languru-0.7.0/languru/server/api/v1/model.py
--rw-r--r--   0        0        0     4353 2024-03-19 17:27:51.659208 languru-0.7.0/languru/server/api/v1/moderations.py
--rw-r--r--   0        0        0     5020 2024-03-16 14:34:11.926368 languru-0.7.0/languru/server/api/v1/test_chat.py
--rw-r--r--   0        0        0     4807 2024-03-16 14:34:11.928032 languru-0.7.0/languru/server/api/v1/test_completions.py
--rw-r--r--   0        0        0     2475 2024-03-16 14:32:42.163888 languru-0.7.0/languru/server/api/v1/test_embeddings.py
--rw-r--r--   0        0        0     3501 2024-03-16 14:28:37.515008 languru-0.7.0/languru/server/api/v1/test_model.py
--rw-r--r--   0        0        0     2263 2024-03-16 14:49:26.337338 languru-0.7.0/languru/server/api/v1/test_moderations.py
--rw-r--r--   0        0        0     6958 2024-03-22 14:40:36.646870 languru-0.7.0/languru/server/config.py
--rw-r--r--   0        0        0        0 2024-03-15 13:29:27.116472 languru-0.7.0/languru/server/deps/__init__.py
--rw-r--r--   0        0        0      429 2024-03-15 15:57:27.107390 languru-0.7.0/languru/server/deps/common.py
--rw-r--r--   0        0        0     5166 2024-03-16 14:19:31.491484 languru-0.7.0/languru/server/main.py
--rw-r--r--   0        0        0        0 2024-03-14 16:10:30.874646 languru-0.7.0/languru/server/utils/__init__.py
--rw-r--r--   0        0        0     1270 2024-03-16 04:51:06.133387 languru-0.7.0/languru/server/utils/common.py
--rw-r--r--   0        0        0        0 2024-02-03 08:58:36.094265 languru-0.7.0/languru/types/__init__.py
--rw-r--r--   0        0        0        0 2024-02-03 08:59:16.654501 languru-0.7.0/languru/types/chat/__init__.py
--rw-r--r--   0        0        0     2777 2024-02-07 11:22:07.653278 languru-0.7.0/languru/types/chat/completions.py
--rw-r--r--   0        0        0     2895 2024-03-16 09:41:38.471425 languru-0.7.0/languru/types/completions.py
--rw-r--r--   0        0        0      603 2024-02-09 09:22:56.989013 languru-0.7.0/languru/types/embeddings.py
--rw-r--r--   0        0        0      158 2024-02-07 11:22:07.653430 languru-0.7.0/languru/types/model/__init__.py
--rw-r--r--   0        0        0      454 2024-02-07 11:22:07.653586 languru-0.7.0/languru/types/model/orm.py
--rw-r--r--   0        0        0      403 2024-02-10 12:09:30.949805 languru-0.7.0/languru/types/moderations.py
--rw-r--r--   0        0        0        0 2024-02-13 08:54:51.563321 languru-0.7.0/languru/utils/__init__.py
--rw-r--r--   0        0        0     1622 2024-02-18 07:12:00.382248 languru-0.7.0/languru/utils/calculation.py
--rw-r--r--   0        0        0     2405 2024-03-10 03:24:03.516300 languru-0.7.0/languru/utils/common.py
--rw-r--r--   0        0        0     2328 2024-03-06 14:06:53.434085 languru-0.7.0/languru/utils/device.py
--rw-r--r--   0        0        0     3213 2024-03-10 05:05:15.323391 languru-0.7.0/languru/utils/hf.py
--rw-r--r--   0        0        0     1666 2024-03-16 04:57:10.612817 languru-0.7.0/languru/utils/http.py
--rw-r--r--   0        0        0     1163 2024-02-13 12:38:09.199703 languru-0.7.0/languru/utils/socket.py
--rw-r--r--   0        0        0       63 2024-03-24 13:24:45.659155 languru-0.7.0/languru/version.py
--rw-r--r--   0        0        0     3823 2024-03-24 13:24:34.085064 languru-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    12732 1970-01-01 00:00:00.000000 languru-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-01 11:42:52.861485 languru-0.7.1/LICENSE
+-rw-r--r--   0        0        0    10182 2024-04-02 11:20:24.107511 languru-0.7.1/README.md
+-rw-r--r--   0        0        0        0 2024-02-01 11:42:52.861665 languru-0.7.1/languru/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-07 02:51:29.580590 languru-0.7.1/languru/action/__init__.py
+-rw-r--r--   0        0        0     4891 2024-03-11 03:18:17.774427 languru-0.7.1/languru/action/base.py
+-rw-r--r--   0        0        0     7655 2024-03-19 05:31:55.754602 languru-0.7.1/languru/action/google.py
+-rw-r--r--   0        0        0     2816 2024-03-27 09:02:07.247643 languru-0.7.1/languru/action/groq.py
+-rw-r--r--   0        0        0    18777 2024-03-19 05:31:55.754961 languru-0.7.1/languru/action/hf.py
+-rw-r--r--   0        0        0     7339 2024-03-27 09:02:07.248837 languru-0.7.1/languru/action/openai.py
+-rw-r--r--   0        0        0     2999 2024-03-27 09:02:07.249387 languru-0.7.1/languru/action/pplx.py
+-rw-r--r--   0        0        0     1105 2024-03-22 10:50:29.684729 languru-0.7.1/languru/action/utils.py
+-rw-r--r--   0        0        0        0 2024-02-01 11:42:52.861745 languru-0.7.1/languru/cli/__init__.py
+-rw-r--r--   0        0        0     3327 2024-03-22 10:21:59.204779 languru-0.7.1/languru/cli/main.py
+-rw-r--r--   0        0        0      221 2024-02-07 08:19:21.426236 languru-0.7.1/languru/config.py
+-rw-r--r--   0        0        0        0 2024-03-19 05:31:55.755531 languru-0.7.1/languru/examples/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 05:31:55.755648 languru-0.7.1/languru/examples/return_values/__init__.py
+-rw-r--r--   0        0        0     9704 2024-03-19 05:31:55.755827 languru-0.7.1/languru/examples/return_values/_openai.py
+-rw-r--r--   0        0        0       41 2024-02-15 01:55:28.093981 languru-0.7.1/languru/exceptions.py
+-rw-r--r--   0        0        0        0 2024-02-07 02:51:29.582508 languru-0.7.1/languru/resources/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-07 02:51:29.582657 languru-0.7.1/languru/resources/llm/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-07 02:51:29.582788 languru-0.7.1/languru/resources/model/__init__.py
+-rw-r--r--   0        0        0     4394 2024-03-09 09:50:32.758650 languru-0.7.1/languru/resources/model/discovery.py
+-rw-r--r--   0        0        0        0 2024-02-01 11:42:52.861878 languru-0.7.1/languru/server/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-02 02:00:42.777707 languru-0.7.1/languru/server/api/__init__.py
+-rw-r--r--   0        0        0      729 2024-02-15 01:55:28.095262 languru-0.7.1/languru/server/api/v1/__init__.py
+-rw-r--r--   0        0        0     7533 2024-03-27 09:02:07.250510 languru-0.7.1/languru/server/api/v1/chat.py
+-rw-r--r--   0        0        0     5796 2024-03-22 10:07:39.202848 languru-0.7.1/languru/server/api/v1/completions.py
+-rw-r--r--   0        0        0     4423 2024-03-22 10:07:39.203160 languru-0.7.1/languru/server/api/v1/embeddings.py
+-rw-r--r--   0        0        0     9679 2024-03-19 05:31:55.756461 languru-0.7.1/languru/server/api/v1/model.py
+-rw-r--r--   0        0        0     4353 2024-03-22 10:07:39.203389 languru-0.7.1/languru/server/api/v1/moderations.py
+-rw-r--r--   0        0        0     5020 2024-03-19 05:31:55.756725 languru-0.7.1/languru/server/api/v1/test_chat.py
+-rw-r--r--   0        0        0     4807 2024-03-19 05:31:55.756818 languru-0.7.1/languru/server/api/v1/test_completions.py
+-rw-r--r--   0        0        0     2475 2024-03-19 05:31:55.756905 languru-0.7.1/languru/server/api/v1/test_embeddings.py
+-rw-r--r--   0        0        0     3501 2024-03-19 05:31:55.757121 languru-0.7.1/languru/server/api/v1/test_model.py
+-rw-r--r--   0        0        0     2263 2024-03-19 05:31:55.757219 languru-0.7.1/languru/server/api/v1/test_moderations.py
+-rw-r--r--   0        0        0     6958 2024-03-27 09:02:07.250950 languru-0.7.1/languru/server/config.py
+-rw-r--r--   0        0        0        0 2024-03-19 05:31:55.757554 languru-0.7.1/languru/server/deps/__init__.py
+-rw-r--r--   0        0        0      429 2024-03-19 05:31:55.757647 languru-0.7.1/languru/server/deps/common.py
+-rw-r--r--   0        0        0     5166 2024-03-19 05:31:55.757727 languru-0.7.1/languru/server/main.py
+-rw-r--r--   0        0        0        0 2024-03-19 05:31:55.757760 languru-0.7.1/languru/server/utils/__init__.py
+-rw-r--r--   0        0        0     1270 2024-03-19 05:31:55.758226 languru-0.7.1/languru/server/utils/common.py
+-rw-r--r--   0        0        0        0 2024-02-07 02:51:29.585801 languru-0.7.1/languru/types/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-07 02:51:29.585941 languru-0.7.1/languru/types/chat/__init__.py
+-rw-r--r--   0        0        0     2777 2024-02-07 07:57:15.543854 languru-0.7.1/languru/types/chat/completions.py
+-rw-r--r--   0        0        0     2895 2024-03-19 05:31:55.758398 languru-0.7.1/languru/types/completions.py
+-rw-r--r--   0        0        0      603 2024-02-15 01:55:28.096416 languru-0.7.1/languru/types/embeddings.py
+-rw-r--r--   0        0        0      158 2024-02-07 06:54:11.803747 languru-0.7.1/languru/types/model/__init__.py
+-rw-r--r--   0        0        0      454 2024-02-07 07:01:30.525620 languru-0.7.1/languru/types/model/orm.py
+-rw-r--r--   0        0        0      403 2024-02-15 01:55:28.096482 languru-0.7.1/languru/types/moderations.py
+-rw-r--r--   0        0        0        0 2024-02-15 01:55:28.096547 languru-0.7.1/languru/utils/__init__.py
+-rw-r--r--   0        0        0     1622 2024-02-18 04:18:45.843584 languru-0.7.1/languru/utils/calculation.py
+-rw-r--r--   0        0        0     2405 2024-03-11 03:18:17.778514 languru-0.7.1/languru/utils/common.py
+-rw-r--r--   0        0        0     2328 2024-03-08 08:14:03.711878 languru-0.7.1/languru/utils/device.py
+-rw-r--r--   0        0        0     3213 2024-03-11 03:18:17.779132 languru-0.7.1/languru/utils/hf.py
+-rw-r--r--   0        0        0     1666 2024-03-19 05:31:55.758527 languru-0.7.1/languru/utils/http.py
+-rw-r--r--   0        0        0     1163 2024-02-15 01:55:28.096890 languru-0.7.1/languru/utils/socket.py
+-rw-r--r--   0        0        0       63 2024-04-02 11:48:22.742986 languru-0.7.1/languru/version.py
+-rw-r--r--   0        0        0     4296 2024-04-02 11:48:13.512193 languru-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0    13024 1970-01-01 00:00:00.000000 languru-0.7.1/PKG-INFO
```

### Comparing `languru-0.7.0/LICENSE` & `languru-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/README.md` & `languru-0.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,31 +4,32 @@
 
 [![image](https://img.shields.io/pypi/v/languru.svg)](https://pypi.python.org/pypi/languru)
 [![image](https://img.shields.io/pypi/l/languru.svg)](https://pypi.python.org/pypi/languru)
 [![image](https://img.shields.io/pypi/pyversions/languru.svg)](https://pypi.python.org/pypi/languru)
 [![PytestCI](https://github.com/dockhardman/languru/actions/workflows/python-pytest.yml/badge.svg)](https://github.com/dockhardman/languru/actions/workflows/python-pytest.yml)
 [![codecov](https://codecov.io/gh/dockhardman/languru/graph/badge.svg?token=OFX6C8Z31C)](https://codecov.io/gh/dockhardman/languru)
 
+Documentation: [Github Pages](https://dockhardman.github.io/languru/)
+
 ## Getting Started
 
 Install Languru:
 
 ```shell
 pip install languru[server]
 pip install languru[all]  # Or install all dependencies (include `torch`, `transformers`, ...)
 ```
 
 Run llm action server:
 
 ```shell
-echo OPENAI_API_KEY=<YOUR_API_KEY> >>.env  # Replace <YOUR_API_KEY> with your key
-languru llm run
+OPENAI_API_KEY=$OPENAI_API_KEY languru llm run  # Remember set OPENAI_API_KEY before you run.
 ```
 
-Query llm service.
+Query LLM service, which is fully compatible with OpenAI APIs.
 
 ```python
 from openai import OpenAI
 
 client = OpenAI(base_url="http://localhost:8682/v1")
 res = client.chat.completions.create(
     model="gpt-3.5-turbo",
```

### Comparing `languru-0.7.0/languru/action/base.py` & `languru-0.7.1/languru/action/base.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/action/google.py` & `languru-0.7.1/languru/action/google.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/action/groq.py` & `languru-0.7.1/languru/action/groq.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/action/hf.py` & `languru-0.7.1/languru/action/hf.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/action/openai.py` & `languru-0.7.1/languru/action/openai.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/action/pplx.py` & `languru-0.7.1/languru/action/pplx.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/action/utils.py` & `languru-0.7.1/languru/action/utils.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/cli/main.py` & `languru-0.7.1/languru/cli/main.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/examples/return_values/_openai.py` & `languru-0.7.1/languru/examples/return_values/_openai.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/resources/model/discovery.py` & `languru-0.7.1/languru/resources/model/discovery.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/server/api/v1/__init__.py` & `languru-0.7.1/languru/server/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/server/api/v1/chat.py` & `languru-0.7.1/languru/server/api/v1/chat.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/server/api/v1/completions.py` & `languru-0.7.1/languru/server/api/v1/completions.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/server/api/v1/embeddings.py` & `languru-0.7.1/languru/server/api/v1/embeddings.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/server/api/v1/model.py` & `languru-0.7.1/languru/server/api/v1/model.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/server/api/v1/moderations.py` & `languru-0.7.1/languru/server/api/v1/moderations.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/server/api/v1/test_chat.py` & `languru-0.7.1/languru/server/api/v1/test_chat.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/server/api/v1/test_completions.py` & `languru-0.7.1/languru/server/api/v1/test_completions.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/server/api/v1/test_embeddings.py` & `languru-0.7.1/languru/server/api/v1/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/server/api/v1/test_model.py` & `languru-0.7.1/languru/server/api/v1/test_model.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/server/api/v1/test_moderations.py` & `languru-0.7.1/languru/server/api/v1/test_moderations.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/server/config.py` & `languru-0.7.1/languru/server/config.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/server/main.py` & `languru-0.7.1/languru/server/main.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/server/utils/common.py` & `languru-0.7.1/languru/server/utils/common.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/types/chat/completions.py` & `languru-0.7.1/languru/types/chat/completions.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/types/completions.py` & `languru-0.7.1/languru/types/completions.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/types/embeddings.py` & `languru-0.7.1/languru/types/embeddings.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/utils/calculation.py` & `languru-0.7.1/languru/utils/calculation.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/utils/common.py` & `languru-0.7.1/languru/utils/common.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/utils/device.py` & `languru-0.7.1/languru/utils/device.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/utils/hf.py` & `languru-0.7.1/languru/utils/hf.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/utils/http.py` & `languru-0.7.1/languru/utils/http.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/languru/utils/socket.py` & `languru-0.7.1/languru/utils/socket.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.0/pyproject.toml` & `languru-0.7.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [tool.poetry]
 authors = ["Allen Chou <f1470891079@gmail.com>"]
 description = "The general purpose LLM app stacks."
+documentation = "https://dockhardman.github.io/languru/"
+homepage = "https://github.com/dockhardman/languru"
 license = "Apache-2.0 license"
 name = "languru"
 readme = "README.md"
-version = "0.7.0"
+repository = "https://github.com/dockhardman/languru"
+version = "0.7.1"
 
 [tool.poetry.dependencies]
 accelerate = { version = "^0.27.2", optional = true, markers = "sys_platform == 'linux'" }
 aiohttp = "^3.9.3"
 bitsandbytes = { version = "^0.42", optional = true, markers = "sys_platform == 'linux'" }
 click = "^8.1.7"
 colorama = "^0.4.6"
@@ -70,14 +73,25 @@
 
 [tool.poetry.group.cuda.dependencies]
 accelerate = { version = "^0.27.2", optional = true, markers = "sys_platform == 'linux'" }
 bitsandbytes = { version = "^0.42", optional = true, markers = "sys_platform == 'linux'" }
 flash-attn = { version = "^2", optional = true, markers = "sys_platform == 'linux'" }
 nvgpu = { version = "^0.10.0", optional = true, markers = "sys_platform == 'linux'" }
 
+[tool.poetry.group.docs.dependencies]
+mkdocs-git-authors-plugin = "*"
+mkdocs-git-committers-plugin-2 = "*"
+mkdocs-git-revision-date-localized-plugin = "*"
+mkdocs-material = "^9"
+mkdocs-minify-plugin = "*"
+mkdocs-nav-weight = "*"
+mkdocs-redirects = "*"
+mkdocs-render-swagger-plugin = "*"
+neoteroi-mkdocs = "*"
+
 [tool.poetry.group.dev.dependencies]
 black = "*"
 isort = "*"
 mkdocs-material = "^9"
 poetry-plugin-export = "^1.6.0"
 pytest = "^8"
 pytest-asyncio = "*"
```

### Comparing `languru-0.7.0/PKG-INFO` & `languru-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: languru
-Version: 0.7.0
+Version: 0.7.1
 Summary: The general purpose LLM app stacks.
+Home-page: https://github.com/dockhardman/languru
 License: Apache-2.0 license
 Author: Allen Chou
 Author-email: f1470891079@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -43,43 +44,46 @@
 Requires-Dist: sentencepiece (>=0.1.99,<0.2.0) ; extra == "all" or extra == "huggingface"
 Requires-Dist: sqlalchemy (>=2.0.25,<3.0.0)
 Requires-Dist: torch (>=2.2.0,<3.0.0) ; extra == "all" or extra == "huggingface" or extra == "torch"
 Requires-Dist: torchaudio (>=2.2.0,<3.0.0) ; extra == "all" or extra == "huggingface" or extra == "torch"
 Requires-Dist: torchvision (>=0.17.0,<0.18.0) ; extra == "all" or extra == "huggingface" or extra == "torch"
 Requires-Dist: transformers[torch] (>=4.37.2,<5.0.0) ; extra == "all" or extra == "huggingface" or extra == "huggingface-cpu"
 Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
+Project-URL: Documentation, https://dockhardman.github.io/languru/
+Project-URL: Repository, https://github.com/dockhardman/languru
 Description-Content-Type: text/markdown
 
 # Languru
 
 The general-purpose LLM app stacks deploy AI services quickly and (stupidly) simply.
 
 [![image](https://img.shields.io/pypi/v/languru.svg)](https://pypi.python.org/pypi/languru)
 [![image](https://img.shields.io/pypi/l/languru.svg)](https://pypi.python.org/pypi/languru)
 [![image](https://img.shields.io/pypi/pyversions/languru.svg)](https://pypi.python.org/pypi/languru)
 [![PytestCI](https://github.com/dockhardman/languru/actions/workflows/python-pytest.yml/badge.svg)](https://github.com/dockhardman/languru/actions/workflows/python-pytest.yml)
 [![codecov](https://codecov.io/gh/dockhardman/languru/graph/badge.svg?token=OFX6C8Z31C)](https://codecov.io/gh/dockhardman/languru)
 
+Documentation: [Github Pages](https://dockhardman.github.io/languru/)
+
 ## Getting Started
 
 Install Languru:
 
 ```shell
 pip install languru[server]
 pip install languru[all]  # Or install all dependencies (include `torch`, `transformers`, ...)
 ```
 
 Run llm action server:
 
 ```shell
-echo OPENAI_API_KEY=<YOUR_API_KEY> >>.env  # Replace <YOUR_API_KEY> with your key
-languru llm run
+OPENAI_API_KEY=$OPENAI_API_KEY languru llm run  # Remember set OPENAI_API_KEY before you run.
 ```
 
-Query llm service.
+Query LLM service, which is fully compatible with OpenAI APIs.
 
 ```python
 from openai import OpenAI
 
 client = OpenAI(base_url="http://localhost:8682/v1")
 res = client.chat.completions.create(
     model="gpt-3.5-turbo",
```

