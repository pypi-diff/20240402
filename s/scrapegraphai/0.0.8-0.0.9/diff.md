# Comparing `tmp/scrapegraphai-0.0.8.tar.gz` & `tmp/scrapegraphai-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapegraphai-0.0.8.tar", max compression
+gzip compressed data, was "scrapegraphai-0.0.9.tar", max compression
```

## Comparing `scrapegraphai-0.0.8.tar` & `scrapegraphai-0.0.9.tar`

### file list

```diff
@@ -1,38 +1,77 @@
--rw-r--r--   0        0        0     1065 2024-03-03 14:00:51.183606 scrapegraphai-0.0.8/LICENSE
--rw-r--r--   0        0        0     5248 2024-03-12 12:08:32.404636 scrapegraphai-0.0.8/README.md
--rw-r--r--   0        0        0     1669 2024-03-12 12:51:06.511393 scrapegraphai-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       54 2024-03-03 14:00:51.196394 scrapegraphai-0.0.8/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2024-03-03 14:00:51.196546 scrapegraphai-0.0.8/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6225 2024-03-03 14:00:51.196717 scrapegraphai-0.0.8/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0       95 2024-03-03 14:00:51.196864 scrapegraphai-0.0.8/scrapegraphai/evaluators/__init__.py
--rw-r--r--   0        0        0     2850 2024-03-03 14:00:51.196981 scrapegraphai-0.0.8/scrapegraphai/evaluators/trulens_evaluator.py
--rw-r--r--   0        0        0      182 2024-03-03 14:00:51.197129 scrapegraphai-0.0.8/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0     3041 2024-03-03 14:00:51.197243 scrapegraphai-0.0.8/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     4033 2024-03-12 12:08:32.406048 scrapegraphai-0.0.8/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     4615 2024-03-12 12:08:32.408204 scrapegraphai-0.0.8/scrapegraphai/graphs/speech_summary_graph.py
--rw-r--r--   0        0        0      164 2024-03-03 14:00:51.197634 scrapegraphai-0.0.8/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0      406 2024-03-03 14:00:51.197724 scrapegraphai-0.0.8/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3446 2024-03-12 12:08:32.408444 scrapegraphai-0.0.8/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0     2363 2024-03-03 14:00:51.197887 scrapegraphai-0.0.8/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      160 2024-03-03 14:00:51.198004 scrapegraphai-0.0.8/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      575 2024-03-03 14:00:51.198085 scrapegraphai-0.0.8/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1721 2024-03-03 14:00:51.198164 scrapegraphai-0.0.8/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1647 2024-03-03 14:00:51.198245 scrapegraphai-0.0.8/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      445 2024-03-12 12:08:32.408767 scrapegraphai-0.0.8/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     2666 2024-03-03 14:00:51.198470 scrapegraphai-0.0.8/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2914 2024-03-03 14:00:51.198557 scrapegraphai-0.0.8/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     3498 2024-03-12 12:08:32.408975 scrapegraphai-0.0.8/scrapegraphai/nodes/fetch_html_node.py
--rw-r--r--   0        0        0     1798 2024-03-12 12:08:32.409163 scrapegraphai-0.0.8/scrapegraphai/nodes/fetch_text_node.py
--rw-r--r--   0        0        0     5624 2024-03-12 12:08:32.409470 scrapegraphai-0.0.8/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     3770 2024-03-03 14:00:51.198885 scrapegraphai-0.0.8/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     1243 2024-03-03 14:00:51.198966 scrapegraphai-0.0.8/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     3395 2024-03-12 12:08:32.409631 scrapegraphai-0.0.8/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     4130 2024-03-12 12:08:32.411047 scrapegraphai-0.0.8/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     1258 2024-03-03 14:00:51.199293 scrapegraphai-0.0.8/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      191 2024-03-03 14:00:51.199414 scrapegraphai-0.0.8/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     1271 2024-03-03 14:00:51.199500 scrapegraphai-0.0.8/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1268 2024-03-03 14:00:51.199592 scrapegraphai-0.0.8/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0      877 2024-03-12 12:08:32.411492 scrapegraphai-0.0.8/scrapegraphai/utils/remover.py
--rw-r--r--   0        0        0      574 2024-03-03 14:00:51.199769 scrapegraphai-0.0.8/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0      990 2024-03-03 14:00:51.199840 scrapegraphai-0.0.8/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0     6925 1970-01-01 00:00:00.000000 scrapegraphai-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-03-03 14:00:51.183606 scrapegraphai-0.0.9/LICENSE
+-rw-r--r--   0        0        0     5204 2024-03-14 19:54:25.107262 scrapegraphai-0.0.9/README.md
+-rw-r--r--   0        0        0     1669 2024-03-14 20:02:12.175652 scrapegraphai-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-03-03 14:00:51.196394 scrapegraphai-0.0.9/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2024-03-03 14:00:51.196546 scrapegraphai-0.0.9/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0      322 2024-03-07 12:18:05.846696 scrapegraphai-0.0.9/scrapegraphai/builders/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     8164 2024-03-07 12:18:05.847612 scrapegraphai-0.0.9/scrapegraphai/builders/__pycache__/graph_builder.cpython-311.pyc
+-rw-r--r--   0        0        0     6476 2024-03-14 19:54:25.108991 scrapegraphai-0.0.9/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0       95 2024-03-03 14:00:51.196864 scrapegraphai-0.0.9/scrapegraphai/evaluators/__init__.py
+-rw-r--r--   0        0        0      330 2024-03-07 12:16:19.339413 scrapegraphai-0.0.9/scrapegraphai/evaluators/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4763 2024-03-07 12:16:19.340112 scrapegraphai-0.0.9/scrapegraphai/evaluators/__pycache__/trulens_evaluator.cpython-311.pyc
+-rw-r--r--   0        0        0     2850 2024-03-03 14:00:51.196981 scrapegraphai-0.0.9/scrapegraphai/evaluators/trulens_evaluator.py
+-rw-r--r--   0        0        0      182 2024-03-03 14:00:51.197129 scrapegraphai-0.0.9/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0      465 2024-03-03 14:05:13.267158 scrapegraphai-0.0.9/scrapegraphai/graphs/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3938 2024-03-03 14:05:13.268442 scrapegraphai-0.0.9/scrapegraphai/graphs/__pycache__/base_graph.cpython-311.pyc
+-rw-r--r--   0        0        0     4878 2024-03-14 19:59:46.286501 scrapegraphai-0.0.9/scrapegraphai/graphs/__pycache__/smart_scraper_graph.cpython-311.pyc
+-rw-r--r--   0        0        0     5595 2024-03-14 19:59:47.193195 scrapegraphai-0.0.9/scrapegraphai/graphs/__pycache__/speech_summary_graph.cpython-311.pyc
+-rw-r--r--   0        0        0     3041 2024-03-03 14:00:51.197243 scrapegraphai-0.0.9/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     4047 2024-03-14 19:54:25.109163 scrapegraphai-0.0.9/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     4629 2024-03-14 19:54:25.109531 scrapegraphai-0.0.9/scrapegraphai/graphs/speech_summary_graph.py
+-rw-r--r--   0        0        0      164 2024-03-03 14:00:51.197634 scrapegraphai-0.0.9/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0      417 2024-03-07 12:18:06.972641 scrapegraphai-0.0.9/scrapegraphai/helpers/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      554 2024-03-07 12:18:06.974033 scrapegraphai-0.0.9/scrapegraphai/helpers/__pycache__/models_tokens.cpython-311.pyc
+-rw-r--r--   0        0        0     2990 2024-03-12 12:09:21.919273 scrapegraphai-0.0.9/scrapegraphai/helpers/__pycache__/nodes_metadata.cpython-311.pyc
+-rw-r--r--   0        0        0     1555 2024-03-07 12:18:06.973681 scrapegraphai-0.0.9/scrapegraphai/helpers/__pycache__/schemas.cpython-311.pyc
+-rw-r--r--   0        0        0      406 2024-03-03 14:00:51.197724 scrapegraphai-0.0.9/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3446 2024-03-12 12:08:32.408444 scrapegraphai-0.0.9/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0     2363 2024-03-03 14:00:51.197887 scrapegraphai-0.0.9/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      187 2024-03-14 19:54:25.109790 scrapegraphai-0.0.9/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      495 2024-03-14 19:58:41.591208 scrapegraphai-0.0.9/scrapegraphai/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1245 2024-03-14 19:58:42.338097 scrapegraphai-0.0.9/scrapegraphai/models/__pycache__/gemini.cpython-311.pyc
+-rw-r--r--   0        0        0     1173 2024-03-03 14:05:12.611162 scrapegraphai-0.0.9/scrapegraphai/models/__pycache__/openai.cpython-311.pyc
+-rw-r--r--   0        0        0     2415 2024-03-03 14:05:13.261218 scrapegraphai-0.0.9/scrapegraphai/models/__pycache__/openai_itt.cpython-311.pyc
+-rw-r--r--   0        0        0     2478 2024-03-03 14:05:13.265915 scrapegraphai-0.0.9/scrapegraphai/models/__pycache__/openai_tts.cpython-311.pyc
+-rw-r--r--   0        0        0      715 2024-03-14 19:54:25.109898 scrapegraphai-0.0.9/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      575 2024-03-03 14:00:51.198085 scrapegraphai-0.0.9/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1721 2024-03-03 14:00:51.198164 scrapegraphai-0.0.9/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1647 2024-03-03 14:00:51.198245 scrapegraphai-0.0.9/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      529 2024-03-14 19:54:25.110074 scrapegraphai-0.0.9/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0      994 2024-03-14 19:59:46.287147 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3390 2024-03-03 14:05:13.451022 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/base_node.cpython-311.pyc
+-rw-r--r--   0        0        0     3903 2024-03-12 20:22:37.637898 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/conditional_node.cpython-311.pyc
+-rw-r--r--   0        0        0     4815 2024-03-12 12:08:54.597343 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/fetch_html_node.cpython-311.pyc
+-rw-r--r--   0        0        0     2756 2024-03-12 20:22:38.139360 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/fetch_text_node.cpython-311.pyc
+-rw-r--r--   0        0        0     6336 2024-03-12 12:08:54.998583 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/generate_answer_node.cpython-311.pyc
+-rw-r--r--   0        0        0     6366 2024-03-14 19:59:46.670743 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/generate_answer_node_from_rag.cpython-311.pyc
+-rw-r--r--   0        0        0     4946 2024-03-14 19:59:47.192498 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/generate_answer_node_vanilla.cpython-311.pyc
+-rw-r--r--   0        0        0     4783 2024-03-03 14:05:13.451945 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/get_probable_tags_node.cpython-311.pyc
+-rw-r--r--   0        0        0     2219 2024-03-03 14:05:14.086097 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/image_to_text_node.cpython-311.pyc
+-rw-r--r--   0        0        0     4151 2024-03-03 14:05:13.500976 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/parse_html_node.cpython-311.pyc
+-rw-r--r--   0        0        0     4476 2024-03-12 12:08:55.003121 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/parse_node.cpython-311.pyc
+-rw-r--r--   0        0        0     3625 2024-03-05 12:13:18.777801 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/parse_text_node.cpython-311.pyc
+-rw-r--r--   0        0        0     5068 2024-03-12 12:08:55.011225 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/rag_node.cpython-311.pyc
+-rw-r--r--   0        0        0     2276 2024-03-03 14:05:14.085608 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/text_to_speech_node.cpython-311.pyc
+-rw-r--r--   0        0        0     2666 2024-03-03 14:00:51.198470 scrapegraphai-0.0.9/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2914 2024-03-12 20:22:34.352630 scrapegraphai-0.0.9/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     3498 2024-03-12 12:08:32.408975 scrapegraphai-0.0.9/scrapegraphai/nodes/fetch_html_node.py
+-rw-r--r--   0        0        0     1799 2024-03-12 20:17:38.519456 scrapegraphai-0.0.9/scrapegraphai/nodes/fetch_text_node.py
+-rw-r--r--   0        0        0     5631 2024-03-14 19:54:25.110224 scrapegraphai-0.0.9/scrapegraphai/nodes/generate_answer_node_from_rag.py
+-rw-r--r--   0        0        0     3938 2024-03-14 19:54:25.110334 scrapegraphai-0.0.9/scrapegraphai/nodes/generate_answer_node_vanilla.py
+-rw-r--r--   0        0        0     3770 2024-03-03 14:00:51.198885 scrapegraphai-0.0.9/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     1243 2024-03-03 14:00:51.198966 scrapegraphai-0.0.9/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     3395 2024-03-12 12:08:32.409631 scrapegraphai-0.0.9/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     4130 2024-03-12 12:08:32.411047 scrapegraphai-0.0.9/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     1258 2024-03-03 14:00:51.199293 scrapegraphai-0.0.9/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      191 2024-03-03 14:00:51.199414 scrapegraphai-0.0.9/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0      417 2024-03-03 14:05:14.087703 scrapegraphai-0.0.9/scrapegraphai/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2134 2024-03-03 14:05:14.088401 scrapegraphai-0.0.9/scrapegraphai/utils/__pycache__/convert_to_csv.cpython-311.pyc
+-rw-r--r--   0        0        0     2291 2024-03-03 14:05:14.674154 scrapegraphai-0.0.9/scrapegraphai/utils/__pycache__/convert_to_json.cpython-311.pyc
+-rw-r--r--   0        0        0     1559 2024-03-12 12:08:54.888761 scrapegraphai-0.0.9/scrapegraphai/utils/__pycache__/remover.cpython-311.pyc
+-rw-r--r--   0        0        0     1159 2024-03-03 14:05:14.088008 scrapegraphai-0.0.9/scrapegraphai/utils/__pycache__/save_audio_from_bytes.cpython-311.pyc
+-rw-r--r--   0        0        0     1271 2024-03-03 14:00:51.199500 scrapegraphai-0.0.9/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1268 2024-03-03 14:00:51.199592 scrapegraphai-0.0.9/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0      877 2024-03-12 12:08:32.411492 scrapegraphai-0.0.9/scrapegraphai/utils/remover.py
+-rw-r--r--   0        0        0      574 2024-03-03 14:00:51.199769 scrapegraphai-0.0.9/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0      990 2024-03-03 14:00:51.199840 scrapegraphai-0.0.9/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0     6881 1970-01-01 00:00:00.000000 scrapegraphai-0.0.9/PKG-INFO
```

### Comparing `scrapegraphai-0.0.8/LICENSE` & `scrapegraphai-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.0.8/README.md` & `scrapegraphai-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 
 
 # 🕷️ ScrapeGraphAI: You Only Scrape Once
 [![Downloads](https://static.pepy.tech/badge/scrapegraphai)](https://pepy.tech/project/scrapegraphai)
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
+[![Pylint](https://github.com/VinciGit00/Scrapegraph-ai/actions/workflows/pylint.yml/badge.svg)](https://github.com/VinciGit00/Scrapegraph-ai/actions/workflows/pylint.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 
 ScrapeGraphAI is a *web scraping* python library based on LangChain which uses LLM and direct graph logic to create scraping pipelines for websites and documents.
 Just say which information you want to extract and the library will do it for you!
 
 <p align="center">
@@ -23,24 +24,26 @@
 pip install scrapegraphai
 ```
 ## 🔍 Demo
 Official streamlit demo:
 
 [![My Skills](https://skillicons.dev/icons?i=react)](https://scrapegraph-ai-demo.streamlit.app/)
 
-Is it possible to try also the colab version
+Try it directly on the web using Google Colab:
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1sEZBonBMGP44CtO6GQTwAlL0BGJXjtfd?usp=sharing)
 
 Follow the procedure on the following link to setup your OpenAI API key: [link](https://scrapegraph-ai.readthedocs.io/en/latest/index.html).
 
 ## 📖 Documentation
 
 The documentation for ScrapeGraphAI can be found [here](https://scrapegraph-ai.readthedocs.io/en/latest/).
-Behind this there is also the docusaurus documentation [here](https://scrapegraph-doc.onrender.com/).
+
+Check out also the docusaurus [documentation](https://scrapegraph-doc.onrender.com/).
+
 ## 💻 Usage
 
 ### Case 1: Extracting information using a prompt
 
 You can use the `SmartScraper` class to extract information from a website using a prompt.
 
 The `SmartScraper` class is a direct graph implementation that uses the most common nodes present in a web scraping pipeline. For more information, please see the [documentation](https://scrapegraph-ai.readthedocs.io/en/latest/).
@@ -73,33 +76,26 @@
         'Open Source project aimed at controlling a real life rotary pendulum using RL algorithms'
         ]
 }
 ```
 
 ## 🤝 Contributing
 
-Scrapegraph-ai is [MIT LICENSED](https://github.com/VinciGit00/Scrapegraph-ai/blob/main/LICENSE).
-
-Contributions are welcome! Please check out the todos below, and feel free to open a pull request.
+Fell free to contribute and join our Discord server to discuss with us improvements and give us suggestions!
 
 For more information, please see the [contributing guidelines](https://github.com/VinciGit00/Scrapegraph-ai/blob/main/CONTRIBUTING.md).
 
-Join our Discord server to discuss with us improvements and give us suggestions!
-
 [![My Skills](https://skillicons.dev/icons?i=discord)](https://discord.gg/DujC7HG8)
-
-
-You can also follow all the updates on linkedin!
-
 [![My Skills](https://skillicons.dev/icons?i=linkedin)](https://www.linkedin.com/company/scrapegraphai/)
 
+## ❤️ Contributors
 [![Contributors](https://contrib.rocks/image?repo=VinciGit00/Scrapegraph-ai)](https://github.com/VinciGit00/Scrapegraph-ai/graphs/contributors)
 
-### Citations
-If you want to use our library for research purposes please quote us with the following reference
+## 🎓 Citations
+If you have used our library for research purposes please quote us with the following reference:
 ```text
   @misc{scrapegraph-ai,
     author = {Marco Perini, Lorenzo Padoan, Marco Vinciguerra},
     title = {Scrapegraph-ai},
     year = {2024},
     url = {https://github.com/VinciGit00/Scrapegraph-ai},
     note = {A Python library for scraping data from graphs}
@@ -116,13 +112,13 @@
 |--------------------|----------------------|
 | Marco Vinciguerra  | [![Linkedin Badge](https://img.shields.io/badge/-Linkedin-blue?style=flat&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/marco-vinciguerra-7ba365242/)    |
 | Marco Perini       | [![Linkedin Badge](https://img.shields.io/badge/-Linkedin-blue?style=flat&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/perinim/)   |
 | Lorenzo Padoan     | [![Linkedin Badge](https://img.shields.io/badge/-Linkedin-blue?style=flat&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/lorenzo-padoan-4521a2154/)  |
 
 ## 📜 License
 
-ScrapeGraphAI is licensed under the Apache 2.0 License. See the [LICENSE](https://github.com/VinciGit00/Scrapegraph-ai/blob/main/LICENSE) file for more information.
+ScrapeGraphAI is licensed under the MIT License. See the [LICENSE](https://github.com/VinciGit00/Scrapegraph-ai/blob/main/LICENSE) file for more information.
 
 ## Acknowledgements
 
 - We would like to thank all the contributors to the project and the open-source community for their support.
 - ScrapeGraphAI is meant to be used for data exploration and research purposes only. We are not responsible for any misuse of the library.
```

### Comparing `scrapegraphai-0.0.8/pyproject.toml` & `scrapegraphai-0.0.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scrapegraphai"
-version = "0.0.8"
+version = "0.0.9"
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     "Marco Vinciguerra <mvincig11@gmail.com>",
     "Marco Perini <perinim.98@gmail.com>",
     "Lorenzo Padoan <lorenzo.padoan977@gmail.com>"
 ]
 license = "MIT"
```

### Comparing `scrapegraphai-0.0.8/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-0.0.9/scrapegraphai/builders/graph_builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ 
 Module for making the graph building
 """
 import graphviz
 from langchain_core.prompts import ChatPromptTemplate
 from langchain.chains import create_extraction_chain
-from ..models import OpenAI
+from ..models import OpenAI, Gemini
 from ..helpers import nodes_metadata, graph_schema
 
 
 class GraphBuilder:
     """
     GraphBuilder is a dynamic tool for constructing web scraping graphs based on user prompts. 
     It utilizes a natural language understanding model to interpret user prompts and 
@@ -64,14 +64,21 @@
             "temperature": 0,
             "streaming": True
         }
         # Update defaults with any LLM parameters that were provided
         llm_params = {**llm_defaults, **self.llm_config}
         if "api_key" not in llm_params:
             raise ValueError("LLM configuration must include an 'api_key'.")
+        
+        # select the model based on the model name
+        if "gpt-" in llm_params["model_name"]:
+            return OpenAI(llm_params)
+        elif "gemini" in llm_params["model_name"]:
+            return Gemini(llm_params)
+        
         return OpenAI(llm_params)
 
     def _generate_nodes_description(self):
         """
         Generates a string description of all available nodes and their arguments.
 
         Returns:
```

### Comparing `scrapegraphai-0.0.8/scrapegraphai/evaluators/trulens_evaluator.py` & `scrapegraphai-0.0.9/scrapegraphai/evaluators/trulens_evaluator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.0.8/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-0.0.9/scrapegraphai/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.0.8/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-0.0.9/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 from ..models import OpenAI
 from .base_graph import BaseGraph
 from ..nodes import (
     FetchHTMLNode,
     ParseNode,
     RAGNode,
-    GenerateAnswerNode
+    GenerateAnswerNodeFromRag
     )
 
 class SmartScraperGraph:
     """
     SmartScraper is a comprehensive web scraping tool that automates the process of extracting
     information from web pages using a natural language model to interpret and answer prompts.
 
@@ -74,15 +74,15 @@
         Returns:
             BaseGraph: An instance of the BaseGraph class.
         """
         # define the nodes for the graph
         fetch_html_node = FetchHTMLNode("fetch_html")
         parse_document_node = ParseNode(doc_type="html", chunks_size=4000, node_name="parse_document")
         rag_node = RAGNode(self.llm, "rag")
-        generate_answer_node = GenerateAnswerNode(self.llm, "generate_answer")
+        generate_answer_node = GenerateAnswerNodeFromRag(self.llm, "generate_answer")
 
         return BaseGraph(
             nodes={
                 fetch_html_node,
                 parse_document_node,
                 rag_node,
                 generate_answer_node,
```

### Comparing `scrapegraphai-0.0.8/scrapegraphai/graphs/speech_summary_graph.py` & `scrapegraphai-0.0.9/scrapegraphai/graphs/speech_summary_graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from scrapegraphai.utils.save_audio_from_bytes import save_audio_from_bytes
 from ..models import OpenAI, OpenAITextToSpeech
 from .base_graph import BaseGraph
 from ..nodes import (
     FetchHTMLNode,
     ParseNode,
     RAGNode,
-    GenerateAnswerNode,
+    GenerateAnswerNodeFromRag,
     TextToSpeechNode,
 )
 
 
 class SpeechSummaryGraph:
     """
     SpeechSummaryGraph is a tool that automates the process of extracting and summarizing
@@ -78,15 +78,15 @@
 
         Returns:
             BaseGraph: An instance of the BaseGraph class.
         """
         fetch_html_node = FetchHTMLNode("fetch_html")
         parse_document_node = ParseNode(doc_type="html", chunks_size=4000, node_name="parse_document")
         rag_node = RAGNode(self.llm, "rag")
-        generate_answer_node = GenerateAnswerNode(self.llm, "generate_answer")
+        generate_answer_node = GenerateAnswerNodeFromRag(self.llm, "generate_answer")
         text_to_speech_node = TextToSpeechNode(
             self.text_to_speech_model, "text_to_speech")
 
         return BaseGraph(
             nodes={
                 fetch_html_node,
                 parse_document_node,
```

### Comparing `scrapegraphai-0.0.8/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-0.0.9/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.0.8/scrapegraphai/helpers/schemas.py` & `scrapegraphai-0.0.9/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.0.8/scrapegraphai/models/openai.py` & `scrapegraphai-0.0.9/scrapegraphai/models/openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.0.8/scrapegraphai/models/openai_itt.py` & `scrapegraphai-0.0.9/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.0.8/scrapegraphai/models/openai_tts.py` & `scrapegraphai-0.0.9/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.0.8/scrapegraphai/nodes/base_node.py` & `scrapegraphai-0.0.9/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.0.8/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-0.0.9/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.0.8/scrapegraphai/nodes/fetch_html_node.py` & `scrapegraphai-0.0.9/scrapegraphai/nodes/fetch_html_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.0.8/scrapegraphai/nodes/fetch_text_node.py` & `scrapegraphai-0.0.9/scrapegraphai/nodes/fetch_text_node.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ 
 Module for FetchTextNode
 """
-from .base_node import BaseNode
 from langchain_core.documents import Document
+from .base_node import BaseNode
+
 
 class FetchTextNode(BaseNode):
     """
     A node for loading raw text into the state.
 
     Primarily used in scraping workflows, this node prepares the state by directly 
     loading raw text content from a specified source, making it available for
```

### Comparing `scrapegraphai-0.0.8/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-0.0.9/scrapegraphai/nodes/generate_answer_node_from_rag.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from langchain_core.output_parsers import JsonOutputParser
 from langchain_core.runnables import RunnableParallel
 
 # Imports from the library
 from .base_node import BaseNode
 
 
-class GenerateAnswerNode(BaseNode):
+class GenerateAnswerNodeFromRag(BaseNode):
     """
     A node that generates an answer using a language model (LLM) based on the user's input
     and the content extracted from a webpage. It constructs a prompt from the user's input
     and the scraped content, feeds it to the LLM, and parses the LLM's response to produce
     an answer.
 
     Attributes:
```

### Comparing `scrapegraphai-0.0.8/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-0.0.9/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.0.8/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-0.0.9/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.0.8/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-0.0.9/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.0.8/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-0.0.9/scrapegraphai/nodes/rag_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.0.8/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-0.0.9/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.0.8/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-0.0.9/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.0.8/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-0.0.9/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.0.8/scrapegraphai/utils/remover.py` & `scrapegraphai-0.0.9/scrapegraphai/utils/remover.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.0.8/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-0.0.9/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.0.8/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-0.0.9/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.0.8/PKG-INFO` & `scrapegraphai-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapegraphai
-Version: 0.0.8
+Version: 0.0.9
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Home-page: https://scrapegraph-ai.readthedocs.io/
 License: MIT
 Keywords: scrapegraph,scrapegraphai,langchain,ai,artificial intelligence,gpt,machine learning,rag,nlp,natural language processing,openai,scraping,web scraping,web scraping library,web scraping tool,webscraping,graph
 Author: Marco Vinciguerra
 Author-email: mvincig11@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*, !=3.12.*
@@ -34,14 +34,15 @@
 
 
 
 
 # 🕷️ ScrapeGraphAI: You Only Scrape Once
 [![Downloads](https://static.pepy.tech/badge/scrapegraphai)](https://pepy.tech/project/scrapegraphai)
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
+[![Pylint](https://github.com/VinciGit00/Scrapegraph-ai/actions/workflows/pylint.yml/badge.svg)](https://github.com/VinciGit00/Scrapegraph-ai/actions/workflows/pylint.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 
 ScrapeGraphAI is a *web scraping* python library based on LangChain which uses LLM and direct graph logic to create scraping pipelines for websites and documents.
 Just say which information you want to extract and the library will do it for you!
 
 <p align="center">
@@ -57,24 +58,26 @@
 pip install scrapegraphai
 ```
 ## 🔍 Demo
 Official streamlit demo:
 
 [![My Skills](https://skillicons.dev/icons?i=react)](https://scrapegraph-ai-demo.streamlit.app/)
 
-Is it possible to try also the colab version
+Try it directly on the web using Google Colab:
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1sEZBonBMGP44CtO6GQTwAlL0BGJXjtfd?usp=sharing)
 
 Follow the procedure on the following link to setup your OpenAI API key: [link](https://scrapegraph-ai.readthedocs.io/en/latest/index.html).
 
 ## 📖 Documentation
 
 The documentation for ScrapeGraphAI can be found [here](https://scrapegraph-ai.readthedocs.io/en/latest/).
-Behind this there is also the docusaurus documentation [here](https://scrapegraph-doc.onrender.com/).
+
+Check out also the docusaurus [documentation](https://scrapegraph-doc.onrender.com/).
+
 ## 💻 Usage
 
 ### Case 1: Extracting information using a prompt
 
 You can use the `SmartScraper` class to extract information from a website using a prompt.
 
 The `SmartScraper` class is a direct graph implementation that uses the most common nodes present in a web scraping pipeline. For more information, please see the [documentation](https://scrapegraph-ai.readthedocs.io/en/latest/).
@@ -107,33 +110,26 @@
         'Open Source project aimed at controlling a real life rotary pendulum using RL algorithms'
         ]
 }
 ```
 
 ## 🤝 Contributing
 
-Scrapegraph-ai is [MIT LICENSED](https://github.com/VinciGit00/Scrapegraph-ai/blob/main/LICENSE).
-
-Contributions are welcome! Please check out the todos below, and feel free to open a pull request.
+Fell free to contribute and join our Discord server to discuss with us improvements and give us suggestions!
 
 For more information, please see the [contributing guidelines](https://github.com/VinciGit00/Scrapegraph-ai/blob/main/CONTRIBUTING.md).
 
-Join our Discord server to discuss with us improvements and give us suggestions!
-
 [![My Skills](https://skillicons.dev/icons?i=discord)](https://discord.gg/DujC7HG8)
-
-
-You can also follow all the updates on linkedin!
-
 [![My Skills](https://skillicons.dev/icons?i=linkedin)](https://www.linkedin.com/company/scrapegraphai/)
 
+## ❤️ Contributors
 [![Contributors](https://contrib.rocks/image?repo=VinciGit00/Scrapegraph-ai)](https://github.com/VinciGit00/Scrapegraph-ai/graphs/contributors)
 
-### Citations
-If you want to use our library for research purposes please quote us with the following reference
+## 🎓 Citations
+If you have used our library for research purposes please quote us with the following reference:
 ```text
   @misc{scrapegraph-ai,
     author = {Marco Perini, Lorenzo Padoan, Marco Vinciguerra},
     title = {Scrapegraph-ai},
     year = {2024},
     url = {https://github.com/VinciGit00/Scrapegraph-ai},
     note = {A Python library for scraping data from graphs}
@@ -150,14 +146,14 @@
 |--------------------|----------------------|
 | Marco Vinciguerra  | [![Linkedin Badge](https://img.shields.io/badge/-Linkedin-blue?style=flat&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/marco-vinciguerra-7ba365242/)    |
 | Marco Perini       | [![Linkedin Badge](https://img.shields.io/badge/-Linkedin-blue?style=flat&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/perinim/)   |
 | Lorenzo Padoan     | [![Linkedin Badge](https://img.shields.io/badge/-Linkedin-blue?style=flat&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/lorenzo-padoan-4521a2154/)  |
 
 ## 📜 License
 
-ScrapeGraphAI is licensed under the Apache 2.0 License. See the [LICENSE](https://github.com/VinciGit00/Scrapegraph-ai/blob/main/LICENSE) file for more information.
+ScrapeGraphAI is licensed under the MIT License. See the [LICENSE](https://github.com/VinciGit00/Scrapegraph-ai/blob/main/LICENSE) file for more information.
 
 ## Acknowledgements
 
 - We would like to thank all the contributors to the project and the open-source community for their support.
 - ScrapeGraphAI is meant to be used for data exploration and research purposes only. We are not responsible for any misuse of the library.
```

