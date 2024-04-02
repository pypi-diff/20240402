# Comparing `tmp/ragas-0.1.5.tar.gz` & `tmp/ragas-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragas-0.1.5.tar", last modified: Wed Mar 20 14:51:08 2024, max compression
+gzip compressed data, was "ragas-0.1.6.tar", last modified: Tue Apr  2 00:11:56 2024, max compression
```

## Comparing `ragas-0.1.5.tar` & `ragas-0.1.6.tar`

### file list

```diff
@@ -1,203 +1,211 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.089806 ragas-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-20 14:50:59.000000 ragas-0.1.5/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 14:50:59.000000 ragas-0.1.5/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.049806 ragas-0.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.057806 ragas-0.1.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-03-20 14:50:59.000000 ragas-0.1.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-20 14:50:59.000000 ragas-0.1.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-20 14:50:59.000000 ragas-0.1.5/.github/ISSUE_TEMPLATE/question.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.057806 ragas-0.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-03-20 14:50:59.000000 ragas-0.1.5/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-03-20 14:50:59.000000 ragas-0.1.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-03-20 14:50:59.000000 ragas-0.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-20 14:50:59.000000 ragas-0.1.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-03-20 14:50:59.000000 ragas-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-03-20 14:50:59.000000 ragas-0.1.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-03-20 14:51:08.089806 ragas-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-03-20 14:50:59.000000 ragas-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.057806 ragas-0.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.061806 ragas-0.1.5/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.061806 ragas-0.1.5/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/css/highlight_ipython3.css
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/css/highlight_ipython3_dark.css
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/css/highlight_ipython3_light.css
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/css/highlight_python.css
--rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/css/highlight_python_dark.css
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/css/highlight_python_light.css
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/css/ragas.css
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.065806 ragas-0.1.5/docs/_static/imgs/
--rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/imgs/bar-graph.svg
--rw-r--r--   0 runner    (1001) docker     (127)   164494 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/imgs/compare-emb-results.png
--rw-r--r--   0 runner    (1001) docker     (127)    35659 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/imgs/compare-embeddings.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)   526410 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/imgs/compare-llm-result.png
--rw-r--r--   0 runner    (1001) docker     (127)    75530 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/imgs/compare-llms-front.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)    54409 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/imgs/compare-llms-testset.png
--rw-r--r--   0 runner    (1001) docker     (127)    85475 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/imgs/component-wise-metrics.png
--rw-r--r--   0 runner    (1001) docker     (127)   166767 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/imgs/eval-evolve.png
--rw-r--r--   0 runner    (1001) docker     (127)   246223 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/imgs/langsmith-tracing-faithfullness.png
--rw-r--r--   0 runner    (1001) docker     (127)   119984 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/imgs/langsmith-tracing-overview.png
--rw-r--r--   0 runner    (1001) docker     (127)    33956 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/imgs/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/imgs/question_types.png
--rw-r--r--   0 runner    (1001) docker     (127)   251574 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/imgs/quickstart-output.png
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/imgs/ragas-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)   139460 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/imgs/testset_output.png
--rw-r--r--   0 runner    (1001) docker     (127)   734563 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/imgs/trace-langsmith.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.069806 ragas-0.1.5/docs/_static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/js/mendable_chat_bubble.js
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/js/octolane.js
--rw-r--r--   0 runner    (1001) docker     (127)    62458 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/langsmith-dataset.png
--rw-r--r--   0 runner    (1001) docker     (127)   127732 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/langsmith-evaluation.png
--rw-r--r--   0 runner    (1001) docker     (127)   100406 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/langsmith-feedback.png
--rw-r--r--   0 runner    (1001) docker     (127)   282402 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/langsmith-ragas-chain-trace.png
--rw-r--r--   0 runner    (1001) docker     (127)   209039 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/list-score-traces-ragas.png
--rw-r--r--   0 runner    (1001) docker     (127)   310073 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/_static/traces-score-ragas.png
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/alfred.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.069806 ragas-0.1.5/docs/community/
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/community/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.069806 ragas-0.1.5/docs/concepts/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/concepts/feedback.md
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/concepts/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.069806 ragas-0.1.5/docs/concepts/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/concepts/metrics/answer_correctness.md
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/concepts/metrics/answer_relevance.md
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/concepts/metrics/context_entities_recall.md
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/concepts/metrics/context_precision.md
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/concepts/metrics/context_recall.md
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/concepts/metrics/context_relevancy.md
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/concepts/metrics/critique.md
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/concepts/metrics/faithfulness.md
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/concepts/metrics/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/concepts/metrics/semantic_similarity.md
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/concepts/metrics_driven.md
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/concepts/prompt_adaptation.md
--rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/concepts/prompts.md
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/concepts/testset_generation.md
--rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.073806 ragas-0.1.5/docs/getstarted/
--rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/getstarted/evaluation.md
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/getstarted/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/getstarted/install.md
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/getstarted/monitoring.md
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/getstarted/testset_generation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.073806 ragas-0.1.5/docs/howtos/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.073806 ragas-0.1.5/docs/howtos/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/howtos/applications/compare_embeddings.md
--rw-r--r--   0 runner    (1001) docker     (127)     7548 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/howtos/applications/compare_llms.md
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/howtos/applications/custom_prompts.md
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/howtos/applications/data_preparation.md
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/howtos/applications/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/howtos/applications/tracing.md
--rw-r--r--   0 runner    (1001) docker     (127)     9610 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/howtos/applications/use_prompt_adaptation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.073806 ragas-0.1.5/docs/howtos/customisations/
--rw-r--r--   0 runner    (1001) docker     (127)    15019 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/howtos/customisations/aws-bedrock.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    16901 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/howtos/customisations/azure-openai.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8039 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/howtos/customisations/bring-your-own-llm-or-embs.md
--rw-r--r--   0 runner    (1001) docker     (127)    12023 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/howtos/customisations/gcp-vertexai.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/howtos/customisations/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/howtos/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.077806 ragas-0.1.5/docs/howtos/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/howtos/integrations/athina.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/howtos/integrations/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    15974 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/howtos/integrations/langchain.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    24965 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/howtos/integrations/langfuse.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/howtos/integrations/langsmith.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    16980 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/howtos/integrations/llamaindex.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.077806 ragas-0.1.5/docs/howtos/integrations/nyc_wikipedia/
--rw-r--r--   0 runner    (1001) docker     (127)   130296 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/howtos/integrations/nyc_wikipedia/nyc_text.txt
--rw-r--r--   0 runner    (1001) docker     (127)    23009 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/howtos/integrations/ragas-arize.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/howtos/integrations/ragas_haystack.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/howtos/integrations/tonic-validate.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/howtos/integrations/zeno.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.077806 ragas-0.1.5/docs/references/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/references/evaluation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/references/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.077806 ragas-0.1.5/docs/references/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/references/integrations/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-20 14:50:59.000000 ragas-0.1.5/docs/references/metrics.rst
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-20 14:50:59.000000 ragas-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-20 14:50:59.000000 ragas-0.1.5/references.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.077806 ragas-0.1.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-20 14:50:59.000000 ragas-0.1.5/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-20 14:50:59.000000 ragas-0.1.5/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-20 14:50:59.000000 ragas-0.1.5/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 14:51:08.089806 ragas-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.053806 ragas-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.081806 ragas-0.1.5/src/ragas/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/_analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-20 14:51:07.000000 ragas-0.1.5/src/ragas/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/adaptation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.081806 ragas-0.1.5/src/ragas/embeddings/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/embeddings/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10611 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.081806 ragas-0.1.5/src/ragas/llms/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/llms/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/llms/json_load.py
--rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/llms/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.085806 ragas-0.1.5/src/ragas/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7343 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/metrics/_answer_correctness.py
--rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/metrics/_answer_relevance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/metrics/_answer_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/metrics/_context_entities_recall.py
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/metrics/_context_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/metrics/_context_recall.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/metrics/_context_relevancy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/metrics/_faithfulness.py
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/metrics/critique.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/run_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.085806 ragas-0.1.5/src/ragas/testset/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/testset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/testset/docstore.py
--rw-r--r--   0 runner    (1001) docker     (127)    22731 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/testset/evolutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/testset/extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/testset/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    12038 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/testset/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    29009 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/testset/prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/testset/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-03-20 14:50:59.000000 ragas-0.1.5/src/ragas/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.089806 ragas-0.1.5/src/ragas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-03-20 14:51:07.000000 ragas-0.1.5/src/ragas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-03-20 14:51:08.000000 ragas-0.1.5/src/ragas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 14:51:07.000000 ragas-0.1.5/src/ragas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-20 14:51:07.000000 ragas-0.1.5/src/ragas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-20 14:51:07.000000 ragas-0.1.5/src/ragas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.085806 ragas-0.1.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.085806 ragas-0.1.5/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-20 14:50:59.000000 ragas-0.1.5/tests/benchmarks/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-03-20 14:50:59.000000 ragas-0.1.5/tests/benchmarks/benchmark_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-03-20 14:50:59.000000 ragas-0.1.5/tests/benchmarks/benchmark_testsetgen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-03-20 14:50:59.000000 ragas-0.1.5/tests/benchmarks/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-20 14:50:59.000000 ragas-0.1.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.085806 ragas-0.1.5/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-20 14:50:59.000000 ragas-0.1.5/tests/e2e/test_adaptation.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-20 14:50:59.000000 ragas-0.1.5/tests/e2e/test_fullflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.089806 ragas-0.1.5/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.089806 ragas-0.1.5/tests/unit/llms/
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-20 14:50:59.000000 ragas-0.1.5/tests/unit/llms/test_llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-03-20 14:50:59.000000 ragas-0.1.5/tests/unit/llms/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-03-20 14:50:59.000000 ragas-0.1.5/tests/unit/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-20 14:50:59.000000 ragas-0.1.5/tests/unit/test_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-20 14:50:59.000000 ragas-0.1.5/tests/unit/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-03-20 14:50:59.000000 ragas-0.1.5/tests/unit/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 14:50:59.000000 ragas-0.1.5/tests/unit/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 14:50:59.000000 ragas-0.1.5/tests/unit/test_run_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-20 14:50:59.000000 ragas-0.1.5/tests/unit/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-20 14:50:59.000000 ragas-0.1.5/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-03-20 14:50:59.000000 ragas-0.1.5/tests/unit/test_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:51:08.089806 ragas-0.1.5/tests/unit/testset_generator/
--rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-03-20 14:50:59.000000 ragas-0.1.5/tests/unit/testset_generator/test_docstore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-20 14:50:59.000000 ragas-0.1.5/tests/unit/testset_generator/test_document.py
--rw-r--r--   0 runner    (1001) docker     (127)    41535 2024-03-20 14:50:59.000000 ragas-0.1.5/tests/unit/testset_generator/test_embs.pkl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.176890 ragas-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 00:11:50.000000 ragas-0.1.6/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:50.000000 ragas-0.1.6/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.136891 ragas-0.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.140890 ragas-0.1.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-02 00:11:50.000000 ragas-0.1.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-02 00:11:50.000000 ragas-0.1.6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-02 00:11:50.000000 ragas-0.1.6/.github/ISSUE_TEMPLATE/question.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.140890 ragas-0.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-02 00:11:50.000000 ragas-0.1.6/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-02 00:11:50.000000 ragas-0.1.6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-02 00:11:50.000000 ragas-0.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-02 00:11:50.000000 ragas-0.1.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-04-02 00:11:50.000000 ragas-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-02 00:11:50.000000 ragas-0.1.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-02 00:11:56.176890 ragas-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-04-02 00:11:50.000000 ragas-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.140890 ragas-0.1.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.144890 ragas-0.1.6/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.144890 ragas-0.1.6/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/css/highlight_ipython3.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/css/highlight_ipython3_dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/css/highlight_ipython3_light.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/css/highlight_python.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/css/highlight_python_dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/css/highlight_python_light.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/css/ragas.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.152890 ragas-0.1.6/docs/_static/imgs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/bar-graph.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   164494 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/compare-emb-results.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35659 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/compare-embeddings.jpeg
+-rw-r--r--   0 runner    (1001) docker     (127)   526410 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/compare-llm-result.png
+-rw-r--r--   0 runner    (1001) docker     (127)    75530 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/compare-llms-front.jpeg
+-rw-r--r--   0 runner    (1001) docker     (127)    54409 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/compare-llms-testset.png
+-rw-r--r--   0 runner    (1001) docker     (127)    85475 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/component-wise-metrics.png
+-rw-r--r--   0 runner    (1001) docker     (127)   166767 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/eval-evolve.png
+-rw-r--r--   0 runner    (1001) docker     (127)   246223 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/langsmith-tracing-faithfullness.png
+-rw-r--r--   0 runner    (1001) docker     (127)   119984 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/langsmith-tracing-overview.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33956 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/question_types.png
+-rw-r--r--   0 runner    (1001) docker     (127)   251574 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/quickstart-output.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/ragas-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   415043 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/ragas_workflow_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)   139460 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/testset_output.png
+-rw-r--r--   0 runner    (1001) docker     (127)   734563 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/imgs/trace-langsmith.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.152890 ragas-0.1.6/docs/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/js/mendable_chat_bubble.js
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/js/octolane.js
+-rw-r--r--   0 runner    (1001) docker     (127)    62458 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/langsmith-dataset.png
+-rw-r--r--   0 runner    (1001) docker     (127)   127732 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/langsmith-evaluation.png
+-rw-r--r--   0 runner    (1001) docker     (127)   100406 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/langsmith-feedback.png
+-rw-r--r--   0 runner    (1001) docker     (127)   282402 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/langsmith-ragas-chain-trace.png
+-rw-r--r--   0 runner    (1001) docker     (127)   209039 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/list-score-traces-ragas.png
+-rw-r--r--   0 runner    (1001) docker     (127)   310073 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/_static/traces-score-ragas.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/alfred.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.152890 ragas-0.1.6/docs/community/
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/community/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.152890 ragas-0.1.6/docs/concepts/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/feedback.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.156890 ragas-0.1.6/docs/concepts/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/metrics/answer_correctness.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/metrics/answer_relevance.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/metrics/context_entities_recall.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/metrics/context_precision.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/metrics/context_recall.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/metrics/context_relevancy.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/metrics/critique.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/metrics/faithfulness.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/metrics/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/metrics/semantic_similarity.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/metrics_driven.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/prompt_adaptation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/prompts.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/concepts/testset_generation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.156890 ragas-0.1.6/docs/getstarted/
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/getstarted/evaluation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/getstarted/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/getstarted/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/getstarted/monitoring.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18719 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/getstarted/prepare_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/getstarted/testset_generation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.156890 ragas-0.1.6/docs/howtos/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.156890 ragas-0.1.6/docs/howtos/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/applications/compare_embeddings.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7548 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/applications/compare_llms.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/applications/custom_prompts.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/applications/data_preparation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/applications/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/applications/tracing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9610 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/applications/use_prompt_adaptation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.160890 ragas-0.1.6/docs/howtos/customisations/
+-rw-r--r--   0 runner    (1001) docker     (127)    15019 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/customisations/aws-bedrock.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    16912 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/customisations/azure-openai.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8039 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/customisations/bring-your-own-llm-or-embs.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12023 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/customisations/gcp-vertexai.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/customisations/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.160890 ragas-0.1.6/docs/howtos/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/integrations/athina.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/integrations/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15974 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/integrations/langchain.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    24965 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/integrations/langfuse.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/integrations/langsmith.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    16980 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/integrations/llamaindex.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.160890 ragas-0.1.6/docs/howtos/integrations/nyc_wikipedia/
+-rw-r--r--   0 runner    (1001) docker     (127)   130296 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/integrations/nyc_wikipedia/nyc_text.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8274 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/integrations/openlayer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    23009 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/integrations/ragas-arize.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9456 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/integrations/ragas_haystack.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/integrations/tonic-validate.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/howtos/integrations/zeno.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.160890 ragas-0.1.6/docs/references/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/references/evaluation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/references/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.160890 ragas-0.1.6/docs/references/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/references/integrations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-02 00:11:50.000000 ragas-0.1.6/docs/references/metrics.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 00:11:50.000000 ragas-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-02 00:11:50.000000 ragas-0.1.6/references.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.164890 ragas-0.1.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-02 00:11:50.000000 ragas-0.1.6/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-02 00:11:50.000000 ragas-0.1.6/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 00:11:50.000000 ragas-0.1.6/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 00:11:56.176890 ragas-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.136891 ragas-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.164890 ragas-0.1.6/src/ragas/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-02 00:11:56.000000 ragas-0.1.6/src/ragas/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.164890 ragas-0.1.6/src/ragas/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/embeddings/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10611 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.164890 ragas-0.1.6/src/ragas/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/integrations/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/integrations/langsmith.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.168890 ragas-0.1.6/src/ragas/llms/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/llms/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/llms/json_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/llms/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12936 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/llms/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.168890 ragas-0.1.6/src/ragas/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7842 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/metrics/_answer_correctness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/metrics/_answer_relevance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/metrics/_answer_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/metrics/_context_entities_recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8839 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/metrics/_context_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8131 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/metrics/_context_recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/metrics/_context_relevancy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10410 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/metrics/_faithfulness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/metrics/critique.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/run_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.168890 ragas-0.1.6/src/ragas/testset/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/testset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/testset/docstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22732 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/testset/evolutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/testset/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/testset/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12041 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/testset/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28992 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/testset/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/testset/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-02 00:11:50.000000 ragas-0.1.6/src/ragas/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.172890 ragas-0.1.6/src/ragas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-02 00:11:56.000000 ragas-0.1.6/src/ragas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-04-02 00:11:56.000000 ragas-0.1.6/src/ragas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 00:11:56.000000 ragas-0.1.6/src/ragas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-02 00:11:56.000000 ragas-0.1.6/src/ragas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 00:11:56.000000 ragas-0.1.6/src/ragas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.172890 ragas-0.1.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.172890 ragas-0.1.6/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/benchmarks/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/benchmarks/benchmark_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/benchmarks/benchmark_testsetgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/benchmarks/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.172890 ragas-0.1.6/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/e2e/test_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/e2e/test_fullflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.172890 ragas-0.1.6/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.172890 ragas-0.1.6/tests/unit/llms/
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/unit/llms/test_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/unit/llms/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/unit/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/unit/test_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/unit/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/unit/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/unit/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/unit/test_run_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/unit/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/unit/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:56.172890 ragas-0.1.6/tests/unit/testset_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/unit/testset_generator/test_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/unit/testset_generator/test_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41535 2024-04-02 00:11:50.000000 ragas-0.1.6/tests/unit/testset_generator/test_embs.pkl
```

### Comparing `ragas-0.1.5/.github/ISSUE_TEMPLATE/bug_report.md` & `ragas-0.1.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/.github/ISSUE_TEMPLATE/feature_request.md` & `ragas-0.1.6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/.github/workflows/ci.yaml` & `ragas-0.1.6/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/.github/workflows/python-publish.yml` & `ragas-0.1.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/.gitignore` & `ragas-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/.readthedocs.yml` & `ragas-0.1.6/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/LICENSE` & `ragas-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/Makefile` & `ragas-0.1.6/Makefile`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/PKG-INFO` & `ragas-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragas
-Version: 0.1.5
+Version: 0.1.6
 Description-Content-Type: text/plain
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: datasets
 Requires-Dist: tiktoken
 Requires-Dist: langchain
 Requires-Dist: langchain-core
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ragas Version: 0.1.5 Description-Content-Type:
+Metadata-Version: 2.1 Name: ragas Version: 0.1.6 Description-Content-Type:
 text/plain License-File: LICENSE Requires-Dist: numpy Requires-Dist: datasets
 Requires-Dist: tiktoken Requires-Dist: langchain Requires-Dist: langchain-core
 Requires-Dist: langchain-community Requires-Dist: langchain_openai Requires-
 Dist: openai>1 Requires-Dist: pysbd>=0.3.4 Requires-Dist: nest-asyncio
 Requires-Dist: appdirs Provides-Extra: all Requires-Dist: sentence-
 transformers; extra == "all"
                  ************ [[..//ddooccss//__ssttaattiicc//iimmggss//llooggoo..ppnngg]] ************
```

### Comparing `ragas-0.1.5/README.md` & `ragas-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/Makefile` & `ragas-0.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/css/highlight_ipython3.css` & `ragas-0.1.6/docs/_static/css/highlight_ipython3.css`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/css/highlight_ipython3_dark.css` & `ragas-0.1.6/docs/_static/css/highlight_ipython3_dark.css`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/css/highlight_ipython3_light.css` & `ragas-0.1.6/docs/_static/css/highlight_ipython3_light.css`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/css/highlight_python.css` & `ragas-0.1.6/docs/_static/css/highlight_python.css`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/css/highlight_python_dark.css` & `ragas-0.1.6/docs/_static/css/highlight_python_dark.css`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/css/highlight_python_light.css` & `ragas-0.1.6/docs/_static/css/highlight_python_light.css`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/css/ragas.css` & `ragas-0.1.6/docs/_static/css/ragas.css`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/favicon.ico` & `ragas-0.1.6/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/imgs/bar-graph.svg` & `ragas-0.1.6/docs/_static/imgs/bar-graph.svg`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/imgs/compare-emb-results.png` & `ragas-0.1.6/docs/_static/imgs/compare-emb-results.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/imgs/compare-embeddings.jpeg` & `ragas-0.1.6/docs/_static/imgs/compare-embeddings.jpeg`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/imgs/compare-llm-result.png` & `ragas-0.1.6/docs/_static/imgs/compare-llm-result.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/imgs/compare-llms-front.jpeg` & `ragas-0.1.6/docs/_static/imgs/compare-llms-front.jpeg`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/imgs/compare-llms-testset.png` & `ragas-0.1.6/docs/_static/imgs/compare-llms-testset.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/imgs/component-wise-metrics.png` & `ragas-0.1.6/docs/_static/imgs/component-wise-metrics.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/imgs/eval-evolve.png` & `ragas-0.1.6/docs/_static/imgs/eval-evolve.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/imgs/langsmith-tracing-faithfullness.png` & `ragas-0.1.6/docs/_static/imgs/langsmith-tracing-faithfullness.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/imgs/langsmith-tracing-overview.png` & `ragas-0.1.6/docs/_static/imgs/langsmith-tracing-overview.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/imgs/logo.png` & `ragas-0.1.6/docs/_static/imgs/logo.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/imgs/question_types.png` & `ragas-0.1.6/docs/_static/imgs/question_types.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/imgs/quickstart-output.png` & `ragas-0.1.6/docs/_static/imgs/quickstart-output.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/imgs/ragas-logo.png` & `ragas-0.1.6/docs/_static/imgs/ragas-logo.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/imgs/testset_output.png` & `ragas-0.1.6/docs/_static/imgs/testset_output.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/imgs/trace-langsmith.png` & `ragas-0.1.6/docs/_static/imgs/trace-langsmith.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/js/mendable_chat_bubble.js` & `ragas-0.1.6/docs/_static/js/mendable_chat_bubble.js`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/langsmith-dataset.png` & `ragas-0.1.6/docs/_static/langsmith-dataset.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/langsmith-evaluation.png` & `ragas-0.1.6/docs/_static/langsmith-evaluation.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/langsmith-feedback.png` & `ragas-0.1.6/docs/_static/langsmith-feedback.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/langsmith-ragas-chain-trace.png` & `ragas-0.1.6/docs/_static/langsmith-ragas-chain-trace.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/list-score-traces-ragas.png` & `ragas-0.1.6/docs/_static/list-score-traces-ragas.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/_static/traces-score-ragas.png` & `ragas-0.1.6/docs/_static/traces-score-ragas.png`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/alfred.py` & `ragas-0.1.6/docs/alfred.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/community/index.md` & `ragas-0.1.6/docs/community/index.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/concepts/feedback.md` & `ragas-0.1.6/docs/concepts/feedback.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/concepts/index.md` & `ragas-0.1.6/docs/concepts/index.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/concepts/metrics/answer_correctness.md` & `ragas-0.1.6/docs/concepts/metrics/answer_correctness.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/concepts/metrics/answer_relevance.md` & `ragas-0.1.6/docs/concepts/metrics/answer_relevance.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/concepts/metrics/context_entities_recall.md` & `ragas-0.1.6/docs/concepts/metrics/context_entities_recall.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/concepts/metrics/context_precision.md` & `ragas-0.1.6/docs/concepts/metrics/context_precision.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/concepts/metrics/context_recall.md` & `ragas-0.1.6/docs/concepts/metrics/context_recall.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/concepts/metrics/context_relevancy.md` & `ragas-0.1.6/docs/concepts/metrics/context_relevancy.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/concepts/metrics/critique.md` & `ragas-0.1.6/docs/concepts/metrics/critique.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/concepts/metrics/faithfulness.md` & `ragas-0.1.6/docs/concepts/metrics/faithfulness.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/concepts/metrics/index.md` & `ragas-0.1.6/docs/concepts/metrics/index.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/concepts/metrics/semantic_similarity.md` & `ragas-0.1.6/docs/concepts/metrics/semantic_similarity.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/concepts/metrics_driven.md` & `ragas-0.1.6/docs/concepts/metrics_driven.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/concepts/prompt_adaptation.md` & `ragas-0.1.6/docs/concepts/prompt_adaptation.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/concepts/prompts.md` & `ragas-0.1.6/docs/concepts/prompts.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Prompt Objects
 
 Prompts play a crucial role in any language model-based framework and warrant more consideration than mere strings. A well-crafted prompt should include a clear task instruction, articulated in straightforward natural language, comprehensible to any language model. The objective is to compose prompts that are generalizable and do not overly specialize to a specific state of the language model. It's widely recognized that language models exhibit higher accuracy in few-shot scenarios as opposed to zero-shot contexts. To capitalize on this advantage, it is advisable to accompany each prompt with relevant examples.
 
-Prompts in ragas are defined using the `Prompt` class. Each prompt defined using this class will contain. 
+Prompts in ragas are defined using the `Prompt` class. Each prompt defined using this class will contain.
 
 - `name`: a name given to the prompt. Used to save and identify the prompt.
 - `instruction`: The natural language description of the task to be carried out by the LLM
 - `examples`: List one or more demonstrations of the task at hand. Using demonstrations converts the task from zero-shot to few-shot which can improve accuracy in most cases.
 - `input_keys`:  List of one or more variable names that are used to identify the inputs provided to the LLM.
 - `output_key`: Variable name that is used to identify the output
 - `output_type`: Output type of the prompt. Can be JSON or string.
@@ -29,81 +29,81 @@
             "answer": "It can change its skin color based on the temperature of its environment.",
             "context": "A recent scientific study has discovered a new species of frog in the Amazon rainforest that has the unique ability to change its skin color based on the temperature of its environment.",
             "output": {"question":"What unique ability does the newly discovered species of frog have?"},
         }
     ],
     input_keys=["answer", "context"],
     output_key="output",
-    output_type="JSON",
+    output_type="json",
 )
 ```
 
 This will create a Prompt class object with the given instruction, examples, and keys. The `output_type` is given as JSON here which will process the example values as JSON strings. This object when created will undergo validations to check if the prompt class criteria are met.
 
 - `instruction` is mandatory and cannot be an empty string.
 - `input_keys` and `output_key` are mandatory fields. Multiple `input_keys` can be used but a single `output_key` is accepted.
 - `examples` are optional but if provided should contain the input_key and output_keys in the example keys. The example values should match the output_type (dict or json or str).
 
 Prompt objects have the following methods that can be used when evaluating or formatting a prompt object.
 
 - `to_string(self)`
-    
+
     This method will generate a prompt string from the given object. This string can be directly used as a formatted string with the metrics in the evaluation task.
-    
+
     ```{code-block} python
     print(qa_prompt.to_string())
     ```
-    
+
     ```
     Generate a question for the given answer
-    
+
     answer: "The last Olympics was held in Tokyo, Japan."
     context: "The last Olympics was held in Tokyo, Japan. It is held every 4 years"
     output: {{"question": "Where was the last Olympics held?"}}
-    
+
     answer: "It can change its skin color based on the temperature of its environment."
     context: "A recent scientific study has discovered a new species of frog in the Amazon rainforest that has the unique ability to change its skin color based on the temperature of its environment."
     output: {{"question": "What unique ability does the newly discovered species of frog have?"}}
-    
+
     answer: {answer}
     context: {context}
     output:
     ```
-    
+
 - `format(self, **kwargs)`
-    
+
     This method will use the parameters passed as keyword arguments to format the prompt object and return a Langchain `PromptValue` object that can be directly used in the evaluation tasks.
-    
+
     ```{code-block} python
     qa_prompt.format(answer="This is an answer", context="This is a context")
     ```
-    
+
     ```{code-block} python
     PromptValue(prompt_str='Generate a question for the given answer\n\nanswer: "The last Olympics was held in Tokyo, Japan."\ncontext: "The last Olympics was held in Tokyo, Japan. It is held every 4 years"\noutput: {"question": "Where was the last Olympics held?"}\n\nanswer: "It can change its skin color based on the temperature of its environment."\ncontext: "A recent scientific study has discovered a new species of frog in the Amazon rainforest that has the unique ability to change its skin color based on the temperature of its environment."\noutput: {"question": "What unique ability does the newly discovered species of frog have?"}\n\nanswer: This is an answer\ncontext: This is a context\noutput: \n')
-    
+
     ```
-    
+
 
 - `save(self, cache_dir)`
-    
-     This method will save the prompt to the given cache_dir (default `~/.cache`) directory using the value in the `name` variable. 
-    
+
+     This method will save the prompt to the given cache_dir (default `~/.cache`) directory using the value in the `name` variable.
+
     ```{code-block} python
     qa_prompt.save()
     ```
-    
+
     The prompts are saved in JSON format to `~/.cache/ragas` by default. One can change this by setting the `RAGAS_CACHE_HOME` environment variable to the desired path. In this example,  the prompt will be saved in `~/.cache/ragas/english/question_generation.json`
-    
+
 - `_load(self, language, name, cache_dir)`
-    
-     This method will load the appropriate prompt from the saved directory. 
-    
+
+     This method will load the appropriate prompt from the saved directory.
+
     ```{code-block} python
     from ragas.utils import RAGAS_CACHE_HOME
     Prompt._load(name="question_generation",language="english",cache_dir=RAGAS_CACHE_HOME)
     ```
-    
+
     ```{code-block} python
     Prompt(name='question_generation', instruction='Generate a question for the given answer', examples=[{'answer': 'The last Olympics was held in Tokyo, Japan.', 'context': 'The last Olympics was held in Tokyo, Japan. It is held every 4 years', 'output': {'question': 'Where was the last Olympics held?'}}, {'answer': 'It can change its skin color based on the temperature of its environment.', 'context': 'A recent scientific study has discovered a new species of frog in the Amazon rainforest that has the unique ability to change its skin color based on the temperature of its environment.', 'output': {'question': 'What unique ability does the newly discovered species of frog have?'}}], input_keys=['answer', 'context'], output_key='output', output_type='JSON')
     ```
-    
+
     The prompt was loaded from `.cache/ragas/english/question_generation.json`
```

### Comparing `ragas-0.1.5/docs/concepts/testset_generation.md` & `ragas-0.1.6/docs/concepts/testset_generation.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/conf.py` & `ragas-0.1.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/getstarted/evaluation.md` & `ragas-0.1.6/docs/getstarted/evaluation.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/getstarted/index.md` & `ragas-0.1.6/docs/getstarted/index.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/getstarted/install.md` & `ragas-0.1.6/docs/getstarted/install.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/getstarted/monitoring.md` & `ragas-0.1.6/docs/getstarted/monitoring.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/getstarted/testset_generation.md` & `ragas-0.1.6/docs/getstarted/testset_generation.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/howtos/applications/compare_embeddings.md` & `ragas-0.1.6/docs/howtos/applications/compare_embeddings.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/howtos/applications/compare_llms.md` & `ragas-0.1.6/docs/howtos/applications/compare_llms.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/howtos/applications/custom_prompts.md` & `ragas-0.1.6/docs/howtos/applications/custom_prompts.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ## Write custom prompts with ragas
 
 This is a tutorial notebook that shows how to create and use custom prompts with the metrics used in the evaluation task. This is achieved using Ragas prompt class. This tutorial will guide you to change and use different prompts with the Ragas metrics instead of the default ones used.
 
 **Dataset**
 
-Here I’m using a dataset from HuggingFace. 
+Here I’m using a dataset from HuggingFace.
 
 ```{code-block} python
 
 from datasets import load_dataset, Dataset
 
 amnesty_dataset = load_dataset("explodinggradients/amnesty_qa", "english")
 amnesty_dataset
@@ -49,15 +49,15 @@
             "statements": {
                 "statements": []
             },
         },
     ],
     input_keys=["question", "answer"],
     output_key="statements",
-    output_type="JSON",
+    output_type="json",
 )
 ```
 
 **Using the Custom Prompt in Evaluations**
 
 I will be using the **faithfulness** metric for my evaluation task. Faithfulness uses two default prompts `long_form_answer_prompt` and `nli_statements_message` for evaluations. I will be changing the default `long_form_answer_prompt` used in this metric to the newly created prompt object.
```

### Comparing `ragas-0.1.5/docs/howtos/applications/data_preparation.md` & `ragas-0.1.6/docs/howtos/applications/data_preparation.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/howtos/applications/tracing.md` & `ragas-0.1.6/docs/howtos/applications/tracing.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/howtos/applications/use_prompt_adaptation.md` & `ragas-0.1.6/docs/howtos/applications/use_prompt_adaptation.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/howtos/customisations/aws-bedrock.ipynb` & `ragas-0.1.6/docs/howtos/customisations/aws-bedrock.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/howtos/customisations/azure-openai.ipynb` & `ragas-0.1.6/docs/howtos/customisations/azure-openai.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993831953071084%*

 * *Differences: {"'cells'": "{19: {'source': {insert: [(5, 'loader = DirectoryLoader(\\n'), (6, '    "*

 * *            '"./2023-llm-papers/", use_multithreading=True, silent_errors=True, '*

 * *            'sample_size=1\\n\'), (7, \')\\n\'), (11, \'    document.metadata["filename"] = '*

 * *            'document.metadata["source"]\')], delete: [9, 5]}}, 21: {\'source\': {insert: [(0, '*

 * *            "'generator = TestsetGenerator.from_langchain(\\n'), (1, '    "*

 * *            "generator_llm=azure_model, critic_llm=azure_model, embeddings=a […]*

```diff
@@ -449,19 +449,21 @@
             "outputs": [],
             "source": [
                 "from langchain.document_loaders import DirectoryLoader\n",
                 "from ragas.testset.generator import TestsetGenerator\n",
                 "from ragas.testset.evolutions import simple, reasoning, multi_context\n",
                 "\n",
                 "\n",
-                "loader = DirectoryLoader(\"./2023-llm-papers/\", use_multithreading=True, silent_errors=True,sample_size=1)\n",
+                "loader = DirectoryLoader(\n",
+                "    \"./2023-llm-papers/\", use_multithreading=True, silent_errors=True, sample_size=1\n",
+                ")\n",
                 "documents = loader.load()\n",
                 "\n",
                 "for document in documents:\n",
-                "    document.metadata['filename'] = document.metadata['source']"
+                "    document.metadata[\"filename\"] = document.metadata[\"source\"]"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "c8f735a7",
             "metadata": {},
             "source": [
@@ -471,19 +473,25 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "04abc4b1",
             "metadata": {},
             "outputs": [],
             "source": [
-                "generator = TestsetGenerator.from_langchain(generator_llm=azure_model,critic_llm=azure_model,embeddings=azure_embeddings)\n",
+                "generator = TestsetGenerator.from_langchain(\n",
+                "    generator_llm=azure_model, critic_llm=azure_model, embeddings=azure_embeddings\n",
+                ")\n",
                 "\n",
-                "testset = generator.generate_with_langchain_docs(documents, test_size=10, \n",
-                "                                                 raise_exceptions=False, with_debugging_logs=False,\n",
-                "                                                 distributions={simple: 0.5, reasoning: 0.25, multi_context: 0.25})    "
+                "testset = generator.generate_with_langchain_docs(\n",
+                "    documents,\n",
+                "    test_size=10,\n",
+                "    raise_exceptions=False,\n",
+                "    with_debugging_logs=False,\n",
+                "    distributions={simple: 0.5, reasoning: 0.25, multi_context: 0.25},\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "d2f5a7f7",
             "metadata": {},
             "source": [
```

### Comparing `ragas-0.1.5/docs/howtos/customisations/bring-your-own-llm-or-embs.md` & `ragas-0.1.6/docs/howtos/customisations/bring-your-own-llm-or-embs.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/howtos/customisations/gcp-vertexai.ipynb` & `ragas-0.1.6/docs/howtos/customisations/gcp-vertexai.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/howtos/index.md` & `ragas-0.1.6/docs/howtos/index.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/howtos/integrations/athina.ipynb` & `ragas-0.1.6/docs/howtos/integrations/athina.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/howtos/integrations/langchain.ipynb` & `ragas-0.1.6/docs/howtos/integrations/langchain.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/howtos/integrations/langfuse.ipynb` & `ragas-0.1.6/docs/howtos/integrations/langfuse.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/howtos/integrations/langsmith.ipynb` & `ragas-0.1.6/docs/howtos/integrations/langsmith.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/howtos/integrations/llamaindex.ipynb` & `ragas-0.1.6/docs/howtos/integrations/llamaindex.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/howtos/integrations/nyc_wikipedia/nyc_text.txt` & `ragas-0.1.6/docs/howtos/integrations/nyc_wikipedia/nyc_text.txt`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/howtos/integrations/ragas-arize.ipynb` & `ragas-0.1.6/docs/howtos/integrations/ragas-arize.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/howtos/integrations/ragas_haystack.ipynb` & `ragas-0.1.6/docs/howtos/integrations/ragas_haystack.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9966097851423938%*

 * *Differences: {"'cells'": '{4: {\'source\': {insert: [(4, \'os.environ["OPENAI_API_KEY"] = getpass("enter your '*

 * *            'OpenAI API key:")\')], delete: [4]}}, 6: {\'source\': {insert: [(1, \'from '*

 * *            "haystack_integrations.components.evaluators.ragas import (\\n'), (2, '    "*

 * *            "RagasEvaluator,\\n'), (3, '    RagasMetric,\\n'), (4, ')\\n'), (12, '    "*

 * *            'metric_params={\\n\'), (13, \'        "name": "custom",\\n\'), (14, \'        '*

 * *            '"definition": "Is this answer problemati […]*

```diff
@@ -66,15 +66,15 @@
                 }
             ],
             "source": [
                 "import os\n",
                 "from getpass import getpass\n",
                 "\n",
                 "\n",
-                "os.environ[\"OPENAI_API_KEY\"] = getpass('enter your OpenAI API key:')"
+                "os.environ[\"OPENAI_API_KEY\"] = getpass(\"enter your OpenAI API key:\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "ZnJ-b0G8PPi7"
             },
@@ -94,26 +94,33 @@
             "execution_count": 6,
             "metadata": {
                 "id": "G9tzjoLpeoma"
             },
             "outputs": [],
             "source": [
                 "from haystack import Pipeline\n",
-                "from haystack_integrations.components.evaluators.ragas import RagasEvaluator, RagasMetric\n",
+                "from haystack_integrations.components.evaluators.ragas import (\n",
+                "    RagasEvaluator,\n",
+                "    RagasMetric,\n",
+                ")\n",
                 "\n",
                 "evaluation_pipeline = Pipeline()\n",
                 "evaluator_context = RagasEvaluator(\n",
                 "    metric=RagasMetric.CONTEXT_PRECISION,\n",
                 ")\n",
                 "evaluator_aspect = RagasEvaluator(\n",
                 "    metric=RagasMetric.ASPECT_CRITIQUE,\n",
-                "    metric_params={\"name\": \"custom\", \"definition\": \"Is this answer problematic for children?\", \"strictness\": 3},\n",
+                "    metric_params={\n",
+                "        \"name\": \"custom\",\n",
+                "        \"definition\": \"Is this answer problematic for children?\",\n",
+                "        \"strictness\": 3,\n",
+                "    },\n",
                 ")\n",
                 "evaluation_pipeline.add_component(\"evaluator_context\", evaluator_context)\n",
-                "evaluation_pipeline.add_component(\"evaluator_aspect\", evaluator_aspect)\n"
+                "evaluation_pipeline.add_component(\"evaluator_aspect\", evaluator_aspect)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "WRcSQBoZPnTz"
             },
@@ -125,43 +132,93 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "rfFZX87tP3IC"
             },
             "outputs": [],
             "source": [
-                "QUESTIONS = [\"Which is the most popular global sport?\", \"Who created the Python language?\"]\n",
-                "CONTEXTS = [[\"The popularity of sports can be measured in various ways, including TV viewership, social media presence, number of participants, and economic impact. Football is undoubtedly the world's most popular sport with major events like the FIFA World Cup and sports personalities like Ronaldo and Messi, drawing a followership of more than 4 billion people.\"],\n",
-                "            [\"Python, created by Guido van Rossum in the late 1980s, is a high-level general-purpose programming language. Its design philosophy emphasizes code readability, and its language constructs aim to help programmers write clear, logical code for both small and large-scale software projects.\"]]\n",
-                "RESPONSES = [\"Football is the most popular sport with around 4 billion followers worldwide\", \"Python language was created by Guido van Rossum.\"]\n",
-                "GROUND_TRUTHS = [\"Football is the most popular sport\", \"Python language was created by Guido van Rossum.\"]\n",
-                "\n",
-                "results = evaluation_pipeline.run({\n",
-                "        \"evaluator_context\": {\"questions\": QUESTIONS, \"contexts\": CONTEXTS, \"ground_truths\": GROUND_TRUTHS},\n",
-                "        \"evaluator_aspect\": {\"questions\": QUESTIONS, \"contexts\": CONTEXTS, \"responses\": RESPONSES},\n",
-                "})\n"
+                "QUESTIONS = [\n",
+                "    \"Which is the most popular global sport?\",\n",
+                "    \"Who created the Python language?\",\n",
+                "]\n",
+                "CONTEXTS = [\n",
+                "    [\n",
+                "        \"The popularity of sports can be measured in various ways, including TV viewership, social media presence, number of participants, and economic impact. Football is undoubtedly the world's most popular sport with major events like the FIFA World Cup and sports personalities like Ronaldo and Messi, drawing a followership of more than 4 billion people.\"\n",
+                "    ],\n",
+                "    [\n",
+                "        \"Python, created by Guido van Rossum in the late 1980s, is a high-level general-purpose programming language. Its design philosophy emphasizes code readability, and its language constructs aim to help programmers write clear, logical code for both small and large-scale software projects.\"\n",
+                "    ],\n",
+                "]\n",
+                "RESPONSES = [\n",
+                "    \"Football is the most popular sport with around 4 billion followers worldwide\",\n",
+                "    \"Python language was created by Guido van Rossum.\",\n",
+                "]\n",
+                "GROUND_TRUTHS = [\n",
+                "    \"Football is the most popular sport\",\n",
+                "    \"Python language was created by Guido van Rossum.\",\n",
+                "]\n",
+                "\n",
+                "results = evaluation_pipeline.run(\n",
+                "    {\n",
+                "        \"evaluator_context\": {\n",
+                "            \"questions\": QUESTIONS,\n",
+                "            \"contexts\": CONTEXTS,\n",
+                "            \"ground_truths\": GROUND_TRUTHS,\n",
+                "        },\n",
+                "        \"evaluator_aspect\": {\n",
+                "            \"questions\": QUESTIONS,\n",
+                "            \"contexts\": CONTEXTS,\n",
+                "            \"responses\": RESPONSES,\n",
+                "        },\n",
+                "    }\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "kkyUUXpyhAJt"
             },
             "outputs": [],
             "source": [
-                "QUESTIONS = [\"Which is the most popular global sport?\", \"Who created the Python language?\"]\n",
-                "CONTEXTS = [[\"The popularity of sports can be measured in various ways, including TV viewership, social media presence, number of participants, and economic impact. Football is undoubtedly the world's most popular sport with major events like the FIFA World Cup and sports personalities like Ronaldo and Messi, drawing a followership of more than 4 billion people.\"],\n",
-                "                 [\"Python, created by Guido van Rossum in the late 1980s, is a high-level general-purpose programming language. Its design philosophy emphasizes code readability, and its language constructs aim to help programmers write clear, logical code for both small and large-scale software projects.\"]]\n",
-                "RESPONSES = [\"Football is the most popular sport with around 4 billion followers worldwide\", \"Python language was created by Guido van Rossum.\"]\n",
-                "GROUND_TRUTHS = [\"Football is the most popular sport\", \"Python language was created by Guido van Rossum.\"]\n",
-                "results = evaluation_pipeline.run({\n",
-                "        \"evaluator_context\": {\"questions\": QUESTIONS, \"contexts\": CONTEXTS, \"ground_truths\": GROUND_TRUTHS},\n",
-                "        \"evaluator_aspect\": {\"questions\": QUESTIONS, \"contexts\": CONTEXTS, \"responses\": RESPONSES},\n",
-                "})"
+                "QUESTIONS = [\n",
+                "    \"Which is the most popular global sport?\",\n",
+                "    \"Who created the Python language?\",\n",
+                "]\n",
+                "CONTEXTS = [\n",
+                "    [\n",
+                "        \"The popularity of sports can be measured in various ways, including TV viewership, social media presence, number of participants, and economic impact. Football is undoubtedly the world's most popular sport with major events like the FIFA World Cup and sports personalities like Ronaldo and Messi, drawing a followership of more than 4 billion people.\"\n",
+                "    ],\n",
+                "    [\n",
+                "        \"Python, created by Guido van Rossum in the late 1980s, is a high-level general-purpose programming language. Its design philosophy emphasizes code readability, and its language constructs aim to help programmers write clear, logical code for both small and large-scale software projects.\"\n",
+                "    ],\n",
+                "]\n",
+                "RESPONSES = [\n",
+                "    \"Football is the most popular sport with around 4 billion followers worldwide\",\n",
+                "    \"Python language was created by Guido van Rossum.\",\n",
+                "]\n",
+                "GROUND_TRUTHS = [\n",
+                "    \"Football is the most popular sport\",\n",
+                "    \"Python language was created by Guido van Rossum.\",\n",
+                "]\n",
+                "results = evaluation_pipeline.run(\n",
+                "    {\n",
+                "        \"evaluator_context\": {\n",
+                "            \"questions\": QUESTIONS,\n",
+                "            \"contexts\": CONTEXTS,\n",
+                "            \"ground_truths\": GROUND_TRUTHS,\n",
+                "        },\n",
+                "        \"evaluator_aspect\": {\n",
+                "            \"questions\": QUESTIONS,\n",
+                "            \"contexts\": CONTEXTS,\n",
+                "            \"responses\": RESPONSES,\n",
+                "        },\n",
+                "    }\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 11,
             "metadata": {
                 "colab": {
@@ -179,15 +236,14 @@
                         "[{'name': 'context_precision', 'score': 0.9999999999}]\n",
                         "[{'name': 'custom', 'score': 0}]\n",
                         "[{'name': 'custom', 'score': 0}]\n"
                     ]
                 }
             ],
             "source": [
-                "\n",
                 "for component in [\"evaluator_context\", \"evaluator_aspect\"]:\n",
                 "    for output in results[component][\"results\"]:\n",
                 "        print(output)"
             ]
         },
         {
             "cell_type": "markdown",
@@ -221,15 +277,15 @@
                     ]
                 }
             ],
             "source": [
                 "import pandas as pd\n",
                 "\n",
                 "df = pd.DataFrame.from_dict(results)\n",
-                "print(df)\n"
+                "print(df)"
             ]
         }
     ],
     "metadata": {
         "colab": {
             "provenance": []
         },
```

### Comparing `ragas-0.1.5/docs/howtos/integrations/tonic-validate.ipynb` & `ragas-0.1.6/docs/howtos/integrations/tonic-validate.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/howtos/integrations/zeno.ipynb` & `ragas-0.1.6/docs/howtos/integrations/zeno.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/docs/index.md` & `ragas-0.1.6/docs/index.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 against and setting up online monitoring for your RAG apps.
 :::
 
 :::{grid-item-card} 📚 Core Concepts
 :link: core-concepts
 :link-type: ref
 
-The high-level explainations for building a better understand about the
+The high-level explanations for building a better understand about the
 important topics such how to think about metrics-driven development, how the Ragas metrics work under the hood and synthetic dataset generation.
 :::
 :::{grid-item-card} 🛠️ How-to Guides
 :link: how-to-guides
 :link-type: ref
 
 Practical guides to help you achieve a specific goals. Take a look at these
```

### Comparing `ragas-0.1.5/docs/make.bat` & `ragas-0.1.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/pyproject.toml` & `ragas-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/references.md` & `ragas-0.1.6/references.md`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/src/ragas/_analytics.py` & `ragas-0.1.6/src/ragas/_analytics.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/src/ragas/adaptation.py` & `ragas-0.1.6/src/ragas/adaptation.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/src/ragas/async_utils.py` & `ragas-0.1.6/src/ragas/async_utils.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/src/ragas/callbacks.py` & `ragas-0.1.6/src/ragas/callbacks.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/src/ragas/embeddings/base.py` & `ragas-0.1.6/src/ragas/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/src/ragas/evaluation.py` & `ragas-0.1.6/src/ragas/evaluation.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/src/ragas/exceptions.py` & `ragas-0.1.6/src/ragas/exceptions.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/src/ragas/executor.py` & `ragas-0.1.6/src/ragas/executor.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/src/ragas/llms/base.py` & `ragas-0.1.6/src/ragas/llms/base.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/src/ragas/llms/json_load.py` & `ragas-0.1.6/src/ragas/llms/json_load.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/src/ragas/llms/prompt.py` & `ragas-0.1.6/src/ragas/llms/prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,27 +32,29 @@
 class Prompt(BaseModel):
     """
     Prompt is a class that represents a prompt for the ragas metrics.
 
     Attributes:
         name (str): The name of the prompt.
         instruction (str): The instruction for the prompt.
+        output_format_instruction (str): The output format instruction for the prompt.
         examples (List[Dict[str, Any]]): List of example inputs and outputs for the prompt.
         input_keys (List[str]): List of input variable names.
         output_key (str): The output variable name.
-        output_type (str): The type of the output (default: "json").
-        language (str): The language of the prompt (default: "en").
+        output_type (Literal["json", "str"]): The type of the output (default: "json").
+        language (str): The language of the prompt (default: "english").
     """
 
     name: str
     instruction: str
+    output_format_instruction: str = ""
     examples: t.List[Example] = []
     input_keys: t.List[str]
     output_key: str
-    output_type: str = "json"
+    output_type: t.Literal["json", "str"] = "json"
     language: str = "english"
 
     @root_validator
     def validate_prompt(cls, values: t.Dict[str, t.Any]) -> t.Dict[str, t.Any]:
         """
         Validate the template string to ensure that it is in desired format.
         """
@@ -87,36 +89,45 @@
 
         return values
 
     def to_string(self) -> str:
         """
         Generate the prompt string from the variables.
         """
-        added_json_instruction = (
-            "\nOutput in only valid JSON format."
-            if self.output_type.lower() == "json"
-            else ""
-        )
-        prompt_str = self.instruction + added_json_instruction + "\n"
+        prompt_elements = [self.instruction]
+        if self.output_format_instruction:
+            prompt_elements.append(
+                "\n"
+                + self.output_format_instruction.replace("{", "{{").replace("}", "}}")
+            )
+        prompt_str = "\n".join(prompt_elements) + "\n"
 
         if self.examples:
+            prompt_str += "\nExamples:\n"
             # Format the examples to match the Langchain prompt template
             for example in self.examples:
                 for key, value in example.items():
+                    is_json = isinstance(value, (dict, list))
                     value = (
                         json.dumps(value, ensure_ascii=False).encode("utf8").decode()
                     )
                     value = (
                         value.replace("{", "{{").replace("}", "}}")
                         if self.output_type.lower() == "json"
                         else value
                     )
-                    prompt_str += f"\n{key}: {value}"
+                    prompt_str += (
+                        f"\n{key}: {value}"
+                        if not is_json
+                        else f"\n{key}: ```{value}```"
+                    )
                 prompt_str += "\n"
 
+        prompt_str += "\nYour actual task:\n"
+
         if self.input_keys:
             prompt_str += "".join(f"\n{key}: {{{key}}}" for key in self.input_keys)
         if self.output_key:
             prompt_str += f"\n{self.output_key}: \n"
 
         return prompt_str
 
@@ -132,15 +143,15 @@
             value = json.dumps(value, ensure_ascii=False).encode("utf8").decode()
             value = (
                 value.replace("{", "{{").replace("}", "}}")
                 if self.output_type.lower() == "json"
                 else value
             )
             example_str += f"\n{key}: {value}"
-        return example_str
+        return "```" + example_str + "```"
 
     def format(self, **kwargs: t.Any) -> PromptValue:
         """
         Format the Prompt object into a ChatPromptTemplate object to be used in metrics.
         """
         if set(self.input_keys) != set(kwargs.keys()):
             raise ValueError(
@@ -221,15 +232,14 @@
                 json_loader._safe_load(example[-1], llm)
                 if self.output_type.lower() == "json"
                 else example[-1]
             )
 
             if self.output_type.lower() == "json":
                 output = example_dict[self.output_key]
-                print(output)
                 if isinstance(output, dict):
                     assert (
                         set(output.keys()) == output_keys[i]
                     ), f"Adapted output keys {set(output.keys())=} do not match with the original output keys: {output_keys[i]=}"
                 elif isinstance(output, list) and all(
                     isinstance(item, dict) for item in output
                 ):
@@ -267,14 +277,19 @@
     instruction="Language translation",
     examples=[
         {
             "translate_to": "hindi",
             "input": "Who was  Albert Einstein and what is he best known for?",
             "output": "अल्बर्ट आइंस्टीन कौन थे और वे किसके लिए सबसे ज्यादा प्रसिद्ध हैं?",
         },
+        {
+            "translate_to": "dutch",
+            "input": "Who was queen Elizabeth and what is she best known for?",
+            "output": "Wie was koningin Elizabeth en waar is zij het meest bekend om?",
+        },
     ],
     input_keys=["translate_to", "input"],
     output_key="output",
     output_type="str",
 )
 
 json_translatation = Prompt(
@@ -291,13 +306,28 @@
             },
             "output": {
                 "statements": [
                     "अल्बर्ट आइंस्टीन का जन्म जर्मनी में हुआ था।",
                     "अल्बर्ट आइंस्टीन अपने सापेक्षता के सिद्धांत के लिए सबसे अधिक प्रसिद्ध थे।",
                 ]
             },
-        }
+        },
+        {
+            "translate_to": "dutch",
+            "input": {
+                "statements": [
+                    "Paris is the capital of France.",
+                    "Croissants are a popular French pastry.",
+                ]
+            },
+            "output": {
+                "statements": [
+                    "Parijs is de hoofdstad van Frankrijk.",
+                    "Croissants zijn een populair Frans gebak.",
+                ]
+            },
+        },
     ],
     input_keys=["translate_to", "input"],
     output_key="output",
-    output_type="JSON",
+    output_type="json",
 )
```

### Comparing `ragas-0.1.5/src/ragas/metrics/__init__.py` & `ragas-0.1.6/src/ragas/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/src/ragas/metrics/_answer_correctness.py` & `ragas-0.1.6/src/ragas/metrics/_answer_correctness.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,71 +1,93 @@
 from __future__ import annotations
 
 import logging
 import typing as t
 from dataclasses import dataclass, field
 
 import numpy as np
+from langchain_core.pydantic_v1 import BaseModel
 
-from ragas.llms.json_load import json_loader
+from ragas.llms.output_parser import RagasoutputParser, get_json_format_instructions
 from ragas.llms.prompt import Prompt
 from ragas.metrics._answer_similarity import AnswerSimilarity
 from ragas.metrics.base import EvaluationMode, MetricWithEmbeddings, MetricWithLLM
 from ragas.run_config import RunConfig
 
-logger = logging.getLogger(__name__)
-
 if t.TYPE_CHECKING:
     from langchain_core.callbacks import Callbacks
 
+
+logger = logging.getLogger(__name__)
+
+
+class AnswerCorrectnessClassification(BaseModel):
+    TP: t.List[str]
+    FP: t.List[str]
+    FN: t.List[str]
+
+
+_output_instructions = get_json_format_instructions(AnswerCorrectnessClassification)
+_output_parser = RagasoutputParser(pydantic_object=AnswerCorrectnessClassification)
+
+CORRECTNESS_INSTRUCTIONS = """\
+Given a ground truth and an answer, analyze each statement in the answer and classify them in one of the following categories:
+
+- TP (true positive): statements that are present in both the answer and the ground truth,
+- FP (false positive): statements present in the answer but not found in the ground truth,
+- FN (false negative): relevant statements found in the ground truth but omitted in the answer.
+
+A single statement you must classify in exactly one category. Do not try to interpret the meaning of the ground truth or the answer, just compare the presence of the statements in them."""
+
 CORRECTNESS_PROMPT = Prompt(
     name="answer_correctness",
-    instruction="""Extract following from given question and ground truth
-            "TP": statements that are present in both the answer and the ground truth,
-            "FP": statements present in the answer but not found in the ground truth,
-            "FN": relevant statements found in the ground truth but omitted in the answer, 
-        """,
+    instruction=CORRECTNESS_INSTRUCTIONS,
+    output_format_instruction=_output_instructions,
     examples=[
         {
             "question": """What powers the sun and what is its primary function?""",
             "answer": """The sun is powered by nuclear fission, similar to nuclear reactors on Earth, and its primary function is to provide light to the solar system.""",
             "ground_truth": """The sun is actually powered by nuclear fusion, not fission. In its core, hydrogen atoms fuse to form helium, releasing a tremendous amount of energy. This energy is what lights up the sun and provides heat and light, essential for life on Earth. The sun's light also plays a critical role in Earth's climate system and helps to drive the weather and ocean currents.""",
-            "Extracted statements": {
-                "TP": ["The sun's primary function is to provide light"],
-                "FP": [
-                    "The sun is powered by nuclear fission",
-                    "similar to nuclear reactors on Earth",
-                ],
-                "FN": [
-                    "The sun is powered by nuclear fusion, not fission",
-                    "In its core, hydrogen atoms fuse to form helium, releasing a tremendous amount of energy",
-                    "This energy provides heat and light, essential for life on Earth",
-                    "The sun's light plays a critical role in Earth's climate system",
-                    "The sun helps to drive the weather and ocean currents",
-                ],
-            },
+            "extracted_statements": AnswerCorrectnessClassification.parse_obj(
+                {
+                    "TP": ["The sun's primary function is to provide light"],
+                    "FP": [
+                        "The sun is powered by nuclear fission",
+                        "similar to nuclear reactors on Earth",
+                    ],
+                    "FN": [
+                        "The sun is powered by nuclear fusion, not fission",
+                        "In its core, hydrogen atoms fuse to form helium, releasing a tremendous amount of energy",
+                        "This energy provides heat and light, essential for life on Earth",
+                        "The sun's light plays a critical role in Earth's climate system",
+                        "The sun helps to drive the weather and ocean currents",
+                    ],
+                }
+            ).dict(),
         },
         {
             "question": """What is the boiling point of water?""",
             "answer": """The boiling point of water is 100 degrees Celsius at sea level.""",
             "ground_truth": """The boiling point of water is 100 degrees Celsius (212 degrees Fahrenheit) at sea level, but it can change with altitude.""",
-            "Extracted statements": {
-                "TP": [
-                    "The boiling point of water is 100 degrees Celsius at sea level"
-                ],
-                "FP": [],
-                "FN": [
-                    "The boiling point can change with altitude",
-                    "The boiling point of water is 212 degrees Fahrenheit at sea level",
-                ],
-            },
+            "extracted_statements": AnswerCorrectnessClassification.parse_obj(
+                {
+                    "TP": [
+                        "The boiling point of water is 100 degrees Celsius at sea level"
+                    ],
+                    "FP": [],
+                    "FN": [
+                        "The boiling point can change with altitude",
+                        "The boiling point of water is 212 degrees Fahrenheit at sea level",
+                    ],
+                }
+            ).dict(),
         },
     ],
     input_keys=["question", "answer", "ground_truth"],
-    output_key="Extracted statements",
+    output_key="extracted_statements",
     output_type="json",
 )
 
 
 @dataclass
 class AnswerCorrectness(MetricWithLLM, MetricWithEmbeddings):
 
@@ -85,14 +107,15 @@
     """
 
     name: str = "answer_correctness"  # type: ignore[reportIncompatibleMethodOverride]
     evaluation_mode: EvaluationMode = EvaluationMode.qga  # type: ignore[reportIncompatibleMethodOverride]
     correctness_prompt: Prompt = field(default_factory=lambda: CORRECTNESS_PROMPT)
     weights: list[float] = field(default_factory=lambda: [0.75, 0.25])
     answer_similarity: AnswerSimilarity | None = None
+    max_retries: int = 1
 
     def __post_init__(self: t.Self):
         if len(self.weights) != 2:
             raise ValueError(
                 "Expects a list of two weights. First for factuality, second for semantic similarity"
             )
         if all([w == 0 for w in self.weights]):
@@ -103,56 +126,43 @@
     def init(self, run_config: RunConfig):
         super().init(run_config)
         if self.answer_similarity is None and self.weights[1] != 0:
             self.answer_similarity = AnswerSimilarity(
                 llm=self.llm, embeddings=self.embeddings
             )
 
-    def _compute_statement_presence(self, prediction: t.Any) -> float:
-        assert self.llm is not None, "LLM must be set"
-
-        key_map = [
-            "TP",
-            "FP",
-            "FN",
-        ]
-        prediction = prediction if isinstance(prediction, dict) else {}
-        if prediction:
-            prediction = [prediction.get(k, np.nan) for k in key_map]
-            tp, fp, fn = [
-                len(item) if isinstance(item, list) else np.nan for item in prediction
-            ]
-            if any([np.isnan(i) for i in [tp, fp, fn]]):
-                score = np.nan
-                logger.warning(
-                    "Invalid prediction format. Expected a list of dictionaries with keys 'TP', 'FP', 'FN'"
-                )
-            else:
-                score = tp / (tp + 0.5 * (fp + fn)) if tp > 0 else 0
-        else:
-            score = np.nan
-
+    def _compute_statement_presence(
+        self, prediction: AnswerCorrectnessClassification
+    ) -> float:
+        tp = len(prediction.TP)
+        fp = len(prediction.FP)
+        fn = len(prediction.FN)
+        score = tp / (tp + 0.5 * (fp + fn)) if tp > 0 else 0
         return score
 
     async def _ascore(self, row: t.Dict, callbacks: Callbacks, is_async: bool) -> float:
         assert self.llm is not None, "LLM must be set"
 
         q, a, g = row["question"], row["answer"], row["ground_truth"]
         p_value = self.correctness_prompt.format(question=q, ground_truth=g, answer=a)
         is_statement_present = await self.llm.generate(
             p_value, callbacks=callbacks, is_async=is_async
         )
+        result_text = is_statement_present.generations[0][0].text
 
-        prediction = await json_loader.safe_load(
-            is_statement_present.generations[0][0].text, self.llm, is_async=is_async
+        answers = await _output_parser.aparse(
+            result_text, p_value, self.llm, self.max_retries
         )
-        f1_score = self._compute_statement_presence(prediction)
+        if answers is None:
+            return np.nan
+
+        f1_score = self._compute_statement_presence(answers)
 
         if self.weights[1] == 0:
-            similarity_score = 0
+            similarity_score = 0.0
         else:
             assert self.answer_similarity is not None, "AnswerSimilarity must be set"
 
             similarity_score = await self.answer_similarity.ascore(
                 row, callbacks=callbacks, is_async=is_async
             )
```

### Comparing `ragas-0.1.5/src/ragas/metrics/_answer_relevance.py` & `ragas-0.1.6/src/ragas/metrics/_answer_relevance.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,83 @@
 from __future__ import annotations
 
 import logging
 import typing as t
 from dataclasses import dataclass, field
 
 import numpy as np
+from langchain_core.pydantic_v1 import BaseModel
 
-from ragas.llms.json_load import json_loader
+from ragas.llms.output_parser import RagasoutputParser, get_json_format_instructions
 from ragas.llms.prompt import Prompt
 from ragas.metrics.base import EvaluationMode, MetricWithEmbeddings, MetricWithLLM
 
 logger = logging.getLogger(__name__)
 
 if t.TYPE_CHECKING:
     from langchain_core.callbacks import Callbacks
 
     from ragas.llms.prompt import PromptValue
 
+
+class AnswerRelevanceClassification(BaseModel):
+    question: str
+    noncommittal: int
+
+
+_output_instructions = get_json_format_instructions(
+    pydantic_object=AnswerRelevanceClassification
+)
+_output_parser = RagasoutputParser(pydantic_object=AnswerRelevanceClassification)
+
+
 QUESTION_GEN = Prompt(
     name="question_generation",
-    instruction="""Generate a question for the given answer and Identify if answer is noncommittal. Give noncommittal as 1 if the answer is noncommittal and 0 if the answer is committal. A noncommittal answer is one that is evasive, vague, or ambiguous. For example, "I don't know" or "I'm not sure" are noncommittal answers.""",
+    instruction="""Generate a question for the given answer and Identify if answer is noncommittal. Give noncommittal as 1 if the answer is noncommittal and 0 if the answer is committal. A noncommittal answer is one that is evasive, vague, or ambiguous. For example, "I don't know" or "I'm not sure" are noncommittal answers""",
+    output_format_instruction=_output_instructions,
     examples=[
         {
             "answer": """Albert Einstein was born in Germany.""",
             "context": """Albert Einstein was a German-born theoretical physicist who is widely held to be one of the greatest and most influential scientists of all time""",
-            "output": {
-                "question": "Where was Albert Einstein born?",
-                "noncommittal": 0,
-            },
+            "output": AnswerRelevanceClassification.parse_obj(
+                {
+                    "question": "Where was Albert Einstein born?",
+                    "noncommittal": 0,
+                }
+            ).dict(),
         },
         {
             "answer": """It can change its skin color based on the temperature of its environment.""",
             "context": """A recent scientific study has discovered a new species of frog in the Amazon rainforest that has the unique ability to change its skin color based on the temperature of its environment.""",
-            "output": {
-                "question": "What unique ability does the newly discovered species of frog have?",
-                "noncommittal": 0,
-            },
+            "output": AnswerRelevanceClassification.parse_obj(
+                {
+                    "question": "What unique ability does the newly discovered species of frog have?",
+                    "noncommittal": 0,
+                }
+            ).dict(),
         },
         {
             "answer": """Everest""",
             "context": """The tallest mountain on Earth, measured from sea level, is a renowned peak located in the Himalayas.""",
-            "output": {
-                "question": "What is the tallest mountain on Earth?",
-                "noncommittal": 0,
-            },
+            "output": AnswerRelevanceClassification.parse_obj(
+                {
+                    "question": "What is the tallest mountain on Earth?",
+                    "noncommittal": 0,
+                }
+            ).dict(),
         },
         {
             "answer": """I don't know about the  groundbreaking feature of the smartphone invented in 2023 as am unaware of information beyond 2022. """,
             "context": """In 2023, a groundbreaking invention was announced: a smartphone with a battery life of one month, revolutionizing the way people use mobile technology.""",
-            "output": {
-                "question": "What was the groundbreaking feature of the smartphone invented in 2023?",
-                "noncommittal": 1,
-            },
+            "output": AnswerRelevanceClassification.parse_obj(
+                {
+                    "question": "What was the groundbreaking feature of the smartphone invented in 2023?",
+                    "noncommittal": 1,
+                }
+            ).dict(),
         },
     ],
     input_keys=["answer", "context"],
     output_key="output",
     output_type="json",
 )
 
@@ -98,26 +120,20 @@
         return (
             np.dot(gen_question_vec, question_vec.T).reshape(
                 -1,
             )
             / norm
         )
 
-    def _calculate_score(self, response: t.Sequence[t.Any], row: t.Dict) -> float:
+    def _calculate_score(
+        self, answers: t.Sequence[AnswerRelevanceClassification], row: t.Dict
+    ) -> float:
         question = row["question"]
-        gen_questions = [
-            item.get("question", "") for item in response if isinstance(item, dict)
-        ]
-        committal = np.any(
-            [
-                bool(item.get("noncommittal", 0))
-                for item in response
-                if isinstance(item, dict)
-            ]
-        )
+        gen_questions = [answer.question for answer in answers]
+        committal = np.any([answer.noncommittal for answer in answers])
         if all(q == "" for q in gen_questions):
             logger.warning(
                 "Invalid JSON response. Expected dictionary with key 'question'"
             )
             score = np.nan
         else:
             cosine_sim = self.calculate_similarity(question, gen_questions)
@@ -135,20 +151,24 @@
         prompt = self._create_question_gen_prompt(row)
         result = await self.llm.generate(
             prompt,
             n=self.strictness,
             callbacks=callbacks,
             is_async=is_async,
         )
-        response = [
-            await json_loader.safe_load(r.text, self.llm, is_async=is_async)
-            for r in result.generations[0]
+
+        answers = [
+            await _output_parser.aparse(result.text, prompt, self.llm)
+            for result in result.generations[0]
         ]
+        if any(answer is None for answer in answers):
+            return np.nan
 
-        return self._calculate_score(response, row)
+        answers = [answer for answer in answers if answer is not None]
+        return self._calculate_score(answers, row)
 
     def adapt(self, language: str, cache_dir: str | None = None) -> None:
         assert self.llm is not None, "LLM is not set"
 
         logger.info(f"Adapting AnswerRelevancy metric to {language}")
         self.question_generation = self.question_generation.adapt(
             language, self.llm, cache_dir
```

### Comparing `ragas-0.1.5/src/ragas/metrics/_answer_similarity.py` & `ragas-0.1.6/src/ragas/metrics/_answer_similarity.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/src/ragas/metrics/_context_entities_recall.py` & `ragas-0.1.6/src/ragas/metrics/_context_entities_recall.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,110 @@
 from __future__ import annotations
 
 import logging
 import typing as t
 from dataclasses import dataclass, field
 from typing import Dict
 
-from ragas.llms.json_load import json_loader
+import numpy as np
+from langchain.pydantic_v1 import BaseModel
+
+from ragas.llms.output_parser import RagasoutputParser, get_json_format_instructions
 from ragas.llms.prompt import Prompt
 from ragas.metrics.base import EvaluationMode, MetricWithLLM
 
 if t.TYPE_CHECKING:
     from langchain.callbacks.base import Callbacks
 
 logger = logging.getLogger(__name__)
 
+
+class ContextEntitiesResponse(BaseModel):
+    entities: t.List[str]
+
+
+_output_instructions = get_json_format_instructions(
+    pydantic_object=ContextEntitiesResponse
+)
+_output_parser = RagasoutputParser(pydantic_object=ContextEntitiesResponse)
+
+
 TEXT_ENTITY_EXTRACTION = Prompt(
     name="text_entity_extraction",
     instruction="""Given a text, extract unique entities without repetition. Ensure you consider different forms or mentions of the same entity as a single entity.""",
     input_keys=["text"],
     output_key="output",
     output_type="json",
+    output_format_instruction=_output_instructions,
     examples=[
         {
-            "text": """The Eiffel Tower, located in Paris, France, is one of the most iconic landmarks globally. 
-            Millions of visitors are attracted to it each year for its breathtaking views of the city. 
+            "text": """The Eiffel Tower, located in Paris, France, is one of the most iconic landmarks globally.
+            Millions of visitors are attracted to it each year for its breathtaking views of the city.
             Completed in 1889, it was constructed in time for the 1889 World's Fair.""",
-            "output": {
-                "entities": ["Eiffel Tower", "Paris", "France", "1889", "World's Fair"],
-            },
+            "output": ContextEntitiesResponse.parse_obj(
+                {
+                    "entities": [
+                        "Eiffel Tower",
+                        "Paris",
+                        "France",
+                        "1889",
+                        "World's Fair",
+                    ],
+                }
+            ).dict(),
         },
         {
-            "text": """The Colosseum in Rome, also known as the Flavian Amphitheatre, stands as a monument to Roman architectural and engineering achievement. 
-            Construction began under Emperor Vespasian in AD 70 and was completed by his son Titus in AD 80. 
+            "text": """The Colosseum in Rome, also known as the Flavian Amphitheatre, stands as a monument to Roman architectural and engineering achievement.
+            Construction began under Emperor Vespasian in AD 70 and was completed by his son Titus in AD 80.
             It could hold between 50,000 and 80,000 spectators who watched gladiatorial contests and public spectacles.""",
-            "output": {
-                "entities": [
-                    "Colosseum",
-                    "Rome",
-                    "Flavian Amphitheatre",
-                    "Vespasian",
-                    "AD 70",
-                    "Titus",
-                    "AD 80",
-                ],
-            },
+            "output": ContextEntitiesResponse.parse_obj(
+                {
+                    "entities": [
+                        "Colosseum",
+                        "Rome",
+                        "Flavian Amphitheatre",
+                        "Vespasian",
+                        "AD 70",
+                        "Titus",
+                        "AD 80",
+                    ],
+                }
+            ).dict(),
         },
         {
-            "text": """The Great Wall of China, stretching over 21,196 kilometers from east to west, is a marvel of ancient defensive architecture. 
-            Built to protect against invasions from the north, its construction started as early as the 7th century BC. 
+            "text": """The Great Wall of China, stretching over 21,196 kilometers from east to west, is a marvel of ancient defensive architecture.
+            Built to protect against invasions from the north, its construction started as early as the 7th century BC.
             Today, it is a UNESCO World Heritage Site and a major tourist attraction.""",
-            "output": {
-                "entities": [
-                    "Great Wall of China",
-                    "21,196 kilometers",
-                    "7th century BC",
-                    "UNESCO World Heritage Site",
-                ],
-            },
+            "output": ContextEntitiesResponse.parse_obj(
+                {
+                    "entities": [
+                        "Great Wall of China",
+                        "21,196 kilometers",
+                        "7th century BC",
+                        "UNESCO World Heritage Site",
+                    ],
+                }
+            ).dict(),
         },
         {
-            "text": """The Apollo 11 mission, which launched on July 16, 1969, marked the first time humans landed on the Moon. 
-            Astronauts Neil Armstrong, Buzz Aldrin, and Michael Collins made history, with Armstrong being the first man to step on the lunar surface. 
+            "text": """The Apollo 11 mission, which launched on July 16, 1969, marked the first time humans landed on the Moon.
+            Astronauts Neil Armstrong, Buzz Aldrin, and Michael Collins made history, with Armstrong being the first man to step on the lunar surface.
             This event was a significant milestone in space exploration.""",
-            "output": {
-                "entities": [
-                    "Apollo 11 mission",
-                    "July 16, 1969",
-                    "Moon",
-                    "Neil Armstrong",
-                    "Buzz Aldrin",
-                    "Michael Collins",
-                ],
-            },
+            "output": ContextEntitiesResponse.parse_obj(
+                {
+                    "entities": [
+                        "Apollo 11 mission",
+                        "July 16, 1969",
+                        "Moon",
+                        "Neil Armstrong",
+                        "Buzz Aldrin",
+                        "Michael Collins",
+                    ],
+                }
+            ).dict(),
         },
     ],
 )
 
 
 @dataclass
 class ContextEntityRecall(MetricWithLLM):
@@ -102,59 +131,64 @@
 
     name: str = "context_entity_recall"  # type: ignore
     evaluation_mode: EvaluationMode = EvaluationMode.gc  # type: ignore
     context_entity_recall_prompt: Prompt = field(
         default_factory=lambda: TEXT_ENTITY_EXTRACTION
     )
     batch_size: int = 15
+    max_retries: int = 1
 
     def _compute_score(
-        self, ground_truth_entities: set, context_entities: set
+        self, ground_truth_entities: t.Sequence[str], context_entities: t.Sequence[str]
     ) -> float:
         num_entities_in_both = len(
             set(context_entities).intersection(set(ground_truth_entities))
         )
         return num_entities_in_both / (len(ground_truth_entities) + 1e-8)
 
     async def get_entities(
         self,
         text: str,
         callbacks: Callbacks,
         is_async: bool,
-    ) -> Dict:
+    ) -> t.Optional[ContextEntitiesResponse]:
         assert self.llm is not None, "LLM is not initialized"
-
+        p_value = self.context_entity_recall_prompt.format(
+            text=text,
+        )
         result = await self.llm.generate(
-            prompt=self.context_entity_recall_prompt.format(
-                text=text,
-            ),
+            prompt=p_value,
             callbacks=callbacks,
             is_async=is_async,
         )
-        response_dict = await json_loader.safe_load(
-            result.generations[0][0].text, self.llm, is_async=is_async
+
+        result_text = result.generations[0][0].text
+        answer = await _output_parser.aparse(
+            result_text, p_value, self.llm, self.max_retries
         )
-        response_dict = response_dict if isinstance(response_dict, dict) else {}
-        return response_dict
+        if answer is None:
+            return ContextEntitiesResponse(entities=[])
+
+        return answer
 
     async def _ascore(
         self,
         row: Dict,
         callbacks: Callbacks,
         is_async: bool,
     ) -> float:
         ground_truth, contexts = row["ground_truth"], row["contexts"]
         ground_truth = await self.get_entities(
             ground_truth, callbacks=callbacks, is_async=is_async
         )
         contexts = await self.get_entities(
             "\n".join(contexts), callbacks=callbacks, is_async=is_async
         )
-        return self._compute_score(
-            ground_truth.get("entities", []), contexts.get("entities", [])
-        )
+        if ground_truth is None or contexts is None:
+            return np.nan
+        return self._compute_score(ground_truth.entities, contexts.entities)
 
     def save(self, cache_dir: str | None = None) -> None:
         return self.context_entity_recall_prompt.save(cache_dir)
 
 
 context_entity_recall = ContextEntityRecall(batch_size=15)
```

### Comparing `ragas-0.1.5/src/ragas/metrics/_context_precision.py` & `ragas-0.1.6/src/ragas/metrics/_context_precision.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,54 +2,73 @@
 
 import logging
 import typing as t
 from dataclasses import dataclass, field
 
 import numpy as np
 from datasets import Dataset
+from langchain.pydantic_v1 import BaseModel, Field
 
-from ragas.llms.json_load import json_loader
+from ragas.llms.output_parser import RagasoutputParser, get_json_format_instructions
 from ragas.llms.prompt import Prompt, PromptValue
 from ragas.metrics.base import EvaluationMode, MetricWithLLM
 
 if t.TYPE_CHECKING:
     from langchain_core.callbacks import Callbacks
 
 logger = logging.getLogger(__name__)
 
+
+class ContextPrecisionVerification(BaseModel):
+    """Answer for the verification task wether the context was useful."""
+
+    reason: str = Field(..., description="Reason for verification")
+    verdict: int = Field(..., description="Binary (0/1) verdict of verification")
+
+
+class ContextPrecisionVerifications(BaseModel):
+    __root__: t.List[ContextPrecisionVerification]
+
+
+_verification_output_instructions = get_json_format_instructions(
+    ContextPrecisionVerification
+)
+_output_parser = RagasoutputParser(pydantic_object=ContextPrecisionVerification)
+
 CONTEXT_PRECISION = Prompt(
     name="context_precision",
-    instruction="""Given question, answer and context verify if the context was useful in arriving at the given answer. Give verdict as "1" if useful and "0" if not with json output. """,
+    instruction="""Given question, answer and context verify if the context was useful in arriving at the given answer. Give verdict as "1" if useful and "0" if not with json output.""",
+    output_format_instruction=_verification_output_instructions,
     examples=[
         {
             "question": """What can you tell me about albert Albert Einstein?""",
             "context": """Albert Einstein (14 March 1879 – 18 April 1955) was a German-born theoretical physicist, widely held to be one of the greatest and most influential scientists of all time. Best known for developing the theory of relativity, he also made important contributions to quantum mechanics, and was thus a central figure in the revolutionary reshaping of the scientific understanding of nature that modern physics accomplished in the first decades of the twentieth century. His mass–energy equivalence formula E = mc2, which arises from relativity theory, has been called "the world's most famous equation". He received the 1921 Nobel Prize in Physics "for his services to theoretical physics, and especially for his discovery of the law of the photoelectric effect", a pivotal step in the development of quantum theory. His work is also known for its influence on the philosophy of science. In a 1999 poll of 130 leading physicists worldwide by the British journal Physics World, Einstein was ranked the greatest physicist of all time. His intellectual achievements and originality have made Einstein synonymous with genius.""",
             "answer": """Albert Einstein born in 14 March 1879 was German-born theoretical physicist, widely held to be one of the greatest and most influential scientists of all time. He received the 1921 Nobel Prize in Physics for his services to theoretical physics. He published 4 papers in 1905. Einstein moved to Switzerland in 1895""",
-            "verification": {
-                "reason": "The provided context was indeed useful in arriving at the given answer. The context includes key information about Albert Einstein's life and contributions, which are reflected in the answer.",
-                "verdict": "1",
-            },
+            "verification": ContextPrecisionVerification(
+                reason="The provided context was indeed useful in arriving at the given answer. The context includes key information about Albert Einstein's life and contributions, which are reflected in the answer.",
+                verdict=1,
+            ).dict(),
         },
         {
             "question": """who won 2020 icc world cup?""",
             "context": """The 2022 ICC Men's T20 World Cup, held from October 16 to November 13, 2022, in Australia, was the eighth edition of the tournament. Originally scheduled for 2020, it was postponed due to the COVID-19 pandemic. England emerged victorious, defeating Pakistan by five wickets in the final to clinch their second ICC Men's T20 World Cup title.""",
             "answer": """England""",
-            "verification": {
-                "reason": "the context was useful in clarifying the situation regarding the 2020 ICC World Cup and indicating that England was the winner of the tournament that was intended to be held in 2020 but actually took place in 2022.",
-                "verdict": "1",
-            },
+            "verification": ContextPrecisionVerification(
+                reason="the context was useful in clarifying the situation regarding the 2020 ICC World Cup and indicating that England was the winner of the tournament that was intended to be held in 2020 but actually took place in 2022.",
+                verdict=1,
+            ).dict(),
         },
         {
             "question": """What is the tallest mountain in the world?""",
             "context": """The Andes is the longest continental mountain range in the world, located in South America. It stretches across seven countries and features many of the highest peaks in the Western Hemisphere. The range is known for its diverse ecosystems, including the high-altitude Andean Plateau and the Amazon rainforest.""",
             "answer": """Mount Everest.""",
-            "verification": {
-                "reason": "the provided context discusses the Andes mountain range, which, while impressive, does not include Mount Everest or directly relate to the question about the world's tallest mountain.",
-                "verdict": "0",
-            },
+            "verification": ContextPrecisionVerification(
+                reason="the provided context discusses the Andes mountain range, which, while impressive, does not include Mount Everest or directly relate to the question about the world's tallest mountain.",
+                verdict=0,
+            ).dict(),
         },
     ],
     input_keys=["question", "context", "answer"],
     output_key="verification",
     output_type="json",
 )
 
@@ -66,14 +85,15 @@
     evaluation_mode: EvaluationMode
     context_precision_prompt: Prompt
     """
 
     name: str = "context_precision"  # type: ignore
     evaluation_mode: EvaluationMode = EvaluationMode.qcg  # type: ignore
     context_precision_prompt: Prompt = field(default_factory=lambda: CONTEXT_PRECISION)
+    max_retries: int = 1
 
     def _get_row_attributes(self, row: t.Dict) -> t.Tuple[str, t.List[str], t.Any]:
         answer = "ground_truth"
         if answer not in row.keys():
             logger.warning(
                 "Using 'context_precision' without ground truth will be soon depreciated. Use 'context_utilization' instead"
             )
@@ -86,25 +106,20 @@
         return [
             self.context_precision_prompt.format(
                 question=question, context=c, answer=answer
             )
             for c in contexts
         ]
 
-    def _calculate_average_precision(self, json_responses: t.List[t.Dict]) -> float:
+    def _calculate_average_precision(
+        self, verifications: t.List[ContextPrecisionVerification]
+    ) -> float:
         score = np.nan
-        json_responses = [
-            item if isinstance(item, dict) else {} for item in json_responses
-        ]
-        verdict_list = [
-            int("1" == resp.get("verdict", "").strip())
-            if resp.get("verdict")
-            else np.nan
-            for resp in json_responses
-        ]
+
+        verdict_list = [1 if ver.verdict else 0 for ver in verifications]
         denominator = sum(verdict_list) + 1e-10
         numerator = sum(
             [
                 (sum(verdict_list[: i + 1]) / (i + 1)) * verdict_list[i]
                 for i in range(len(verdict_list))
             ]
         )
@@ -120,30 +135,34 @@
         row: t.Dict,
         callbacks: Callbacks,
         is_async: bool,
     ) -> float:
         assert self.llm is not None, "LLM is not set"
 
         human_prompts = self._context_precision_prompt(row)
-        responses: t.List[str] = []
+        responses = []
         for hp in human_prompts:
             result = await self.llm.generate(
                 hp,
                 n=1,
                 callbacks=callbacks,
                 is_async=is_async,
             )
-            responses.append(result.generations[0][0].text)
+            responses.append([result.generations[0][0].text, hp])
 
-        json_responses = [
-            await json_loader.safe_load(item, self.llm, is_async=is_async)
-            for item in responses
+        items = [
+            await _output_parser.aparse(item, hp, self.llm, self.max_retries)
+            for item, hp in responses
         ]
-        json_responses = t.cast(t.List[t.Dict], json_responses)
-        score = self._calculate_average_precision(json_responses)
+        if any(item is None for item in items):
+            return np.nan
+
+        items = [item for item in items if item is not None]
+        answers = ContextPrecisionVerifications(__root__=items)
+        score = self._calculate_average_precision(answers.__root__)
         return score
 
     def adapt(self, language: str, cache_dir: str | None = None) -> None:
         assert self.llm is not None, "LLM is not set"
 
         logging.info(f"Adapting Context Precision to {language}")
         self.context_precision_prompt = self.context_precision_prompt.adapt(
```

### Comparing `ragas-0.1.5/src/ragas/metrics/_context_recall.py` & `ragas-0.1.6/src/ragas/metrics/_context_recall.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,76 +1,108 @@
 from __future__ import annotations
 
 import logging
 import typing as t
 from dataclasses import dataclass, field
 
 import numpy as np
+from langchain_core.pydantic_v1 import BaseModel
 
-from ragas.llms.json_load import json_loader
+from ragas.llms.output_parser import RagasoutputParser, get_json_format_instructions
 from ragas.llms.prompt import Prompt
 from ragas.metrics.base import EvaluationMode, MetricWithLLM
 
 if t.TYPE_CHECKING:
     from langchain_core.callbacks import Callbacks
 
     from ragas.llms.prompt import PromptValue
 
 logger = logging.getLogger(__name__)
 
+
+class ContextRecallClassificationAnswer(BaseModel):
+    statement: str
+    attributed: int
+    reason: str
+
+
+class ContextRecallClassificationAnswers(BaseModel):
+    __root__: t.List[ContextRecallClassificationAnswer]
+
+    def dicts(self) -> t.List[t.Dict]:
+        return self.dict()["__root__"]
+
+
+_classification_output_instructions = get_json_format_instructions(
+    ContextRecallClassificationAnswers
+)
+_output_parser = RagasoutputParser(pydantic_object=ContextRecallClassificationAnswers)
+
+
 CONTEXT_RECALL_RA = Prompt(
     name="context_recall",
     instruction="""Given a context, and an answer, analyze each sentence in the answer and classify if the sentence can be attributed to the given context or not. Use only "Yes" (1) or "No" (0) as a binary classification. Output json with reason.""",
+    output_format_instruction=_classification_output_instructions,
     examples=[
         {
             "question": """What can you tell me about albert Albert Einstein?""",
-            "context": """Albert Einstein (14 March 1879 – 18 April 1955) was a German-born theoretical physicist, widely held to be one of the greatest and most influential scientists of all time. Best known for developing the theory of relativity, he also made important contributions to quantum mechanics, and was thus a central figure in the revolutionary reshaping of the scientific understanding of nature that modern physics accomplished in the first decades of the twentieth century. His mass–energy equivalence formula E = mc2, which arises from relativity theory, has been called 'the world's most famous equation'. He received the 1921 Nobel Prize in Physics 'for his services to theoretical physics, and especially for his discovery of the law of the photoelectric effect', a pivotal step in the development of quantum theory. His work is also known for its influence on the philosophy of science. In a 1999 poll of 130 leading physicists worldwide by the British journal Physics World, Einstein was ranked the greatest physicist of all time. His intellectual achievements and originality have made Einstein synonymous with genius.""",
+            "context": """Albert Einstein (14 March 1879 - 18 April 1955) was a German-born theoretical physicist, widely held to be one of the greatest and most influential scientists of all time. Best known for developing the theory of relativity, he also made important contributions to quantum mechanics, and was thus a central figure in the revolutionary reshaping of the scientific understanding of nature that modern physics accomplished in the first decades of the twentieth century. His mass-energy equivalence formula E = mc2, which arises from relativity theory, has been called 'the world's most famous equation'. He received the 1921 Nobel Prize in Physics 'for his services to theoretical physics, and especially for his discovery of the law of the photoelectric effect', a pivotal step in the development of quantum theory. His work is also known for its influence on the philosophy of science. In a 1999 poll of 130 leading physicists worldwide by the British journal Physics World, Einstein was ranked the greatest physicist of all time. His intellectual achievements and originality have made Einstein synonymous with genius.""",
             "answer": """Albert Einstein born in 14 March 1879 was  German-born theoretical physicist, widely held to be one of the greatest and most influential scientists of all time. He received the 1921 Nobel Prize in Physics for his services to theoretical physics. He published 4 papers in 1905.  Einstein moved to Switzerland in 1895""",
-            "classification": [
-                {
-                    "statement_1": "Albert Einstein, born on 14 March 1879, was a German-born theoretical physicist, widely held to be one of the greatest and most influential scientists of all time.",
-                    "reason": "The date of birth of Einstein is mentioned clearly in the context.",
-                    "Attributed": "1",
-                },
-                {
-                    "statement_2": "He received the 1921 Nobel Prize in Physics 'for his services to theoretical physics.",
-                    "reason": "The exact sentence is present in the given context.",
-                    "Attributed": "1",
-                },
-                {
-                    "statement_3": "He published 4 papers in 1905.",
-                    "reason": "There is no mention about papers he wrote in the given context.",
-                    "Attributed": "0",
-                },
-                {
-                    "statement_4": "Einstein moved to Switzerland in 1895.",
-                    "reason": "There is no supporting evidence for this in the given context.",
-                    "Attributed": "0",
-                },
-            ],
+            "classification": ContextRecallClassificationAnswers.parse_obj(
+                [
+                    {
+                        "statement": "Albert Einstein, born on 14 March 1879, was a German-born theoretical physicist, widely held to be one of the greatest and most influential scientists of all time.",
+                        "reason": "The date of birth of Einstein is mentioned clearly in the context.",
+                        "attributed": 1,
+                    },
+                    {
+                        "statement": "He received the 1921 Nobel Prize in Physics for his services to theoretical physics.",
+                        "reason": "The exact sentence is present in the given context.",
+                        "attributed": 1,
+                    },
+                    {
+                        "statement": "He published 4 papers in 1905.",
+                        "reason": "There is no mention about papers he wrote in the given context.",
+                        "attributed": 0,
+                    },
+                    {
+                        "statement": "Einstein moved to Switzerland in 1895.",
+                        "reason": "There is no supporting evidence for this in the given context.",
+                        "attributed": 0,
+                    },
+                ]
+            ).dicts(),
         },
         {
             "question": """who won 2020 icc world cup?""",
             "context": """The 2022 ICC Men's T20 World Cup, held from October 16 to November 13, 2022, in Australia, was the eighth edition of the tournament. Originally scheduled for 2020, it was postponed due to the COVID-19 pandemic. England emerged victorious, defeating Pakistan by five wickets in the final to clinch their second ICC Men's T20 World Cup title.""",
             "answer": """England""",
-            "classification": {
-                "statement_1": "England won the 2022 ICC Men's T20 World Cup.",
-                "reason": "From context it is clear that England defeated Pakistan to win the World Cup.",
-                "Attributed": "1",
-            },
+            "classification": ContextRecallClassificationAnswers.parse_obj(
+                [
+                    {
+                        "statement": "England won the 2022 ICC Men's T20 World Cup.",
+                        "reason": "From context it is clear that England defeated Pakistan to win the World Cup.",
+                        "attributed": 1,
+                    },
+                ]
+            ).dicts(),
         },
         {
             "question": """What is the primary fuel for the Sun?""",
             "context": """NULL""",
             "answer": """Hydrogen""",
-            "classification": {
-                "statement_1": "The Sun's primary fuel is hydrogen.",
-                "reason": "The context contains no information",
-                "Attributed": "0",
-            },
+            "classification": ContextRecallClassificationAnswers.parse_obj(
+                [
+                    {
+                        "statement": "The Sun's primary fuel is hydrogen.",
+                        "reason": "The context contains no information",
+                        "attributed": 0,
+                    },
+                ]
+            ).dicts(),
         },
     ],
     input_keys=["question", "context", "answer"],
     output_key="classification",
     output_type="json",
 )
 
@@ -86,52 +118,50 @@
     ----------
     name : str
     """
 
     name: str = "context_recall"  # type: ignore
     evaluation_mode: EvaluationMode = EvaluationMode.qcg  # type: ignore
     context_recall_prompt: Prompt = field(default_factory=lambda: CONTEXT_RECALL_RA)
+    max_retries: int = 1
 
     def _create_context_recall_prompt(self, row: t.Dict) -> PromptValue:
         qstn, ctx, gt = row["question"], row["contexts"], row["ground_truth"]
         ctx = "\n".join(ctx) if isinstance(ctx, list) else ctx
 
         return self.context_recall_prompt.format(question=qstn, context=ctx, answer=gt)
 
     def _compute_score(self, response: t.Any) -> float:
-        response = response if isinstance(response, list) else [response]
-        response = [item if isinstance(item, dict) else {} for item in response]
-        response = [
-            int(item.get("Attributed").strip() == "1")
-            if item.get("Attributed")
-            else np.nan
-            for item in response
-        ]
+        response = [1 if item.attributed else 0 for item in response.__root__]
         denom = len(response)
         numerator = sum(response)
         score = numerator / denom if denom > 0 else np.nan
 
         if np.isnan(score):
-            logger.warning(
-                "Invalid JSON response. Expected dictionary with key 'Attributed'"
-            )
+            logger.warning("The LLM did not return a valid classification.")
 
         return score
 
     async def _ascore(self, row: t.Dict, callbacks: Callbacks, is_async: bool) -> float:
         assert self.llm is not None, "set LLM before use"
-
+        p_value = self._create_context_recall_prompt(row)
         result = await self.llm.generate(
-            self._create_context_recall_prompt(row), callbacks=callbacks, is_async=is_async
+            p_value,
+            callbacks=callbacks,
+            is_async=is_async,
         )
-        response = await json_loader.safe_load(
-            result.generations[0][0].text, self.llm, is_async=is_async
+        result_text = result.generations[0][0].text
+
+        answers = await _output_parser.aparse(
+            result_text, p_value, self.llm, self.max_retries
         )
+        if answers is None:
+            return np.nan
 
-        return self._compute_score(response)
+        return self._compute_score(answers)
 
     def adapt(self, language: str, cache_dir: str | None = None) -> None:
         assert self.llm is not None, "set LLM before use"
 
         logger.info(f"Adapting Context Recall to {language}")
         self.context_recall_prompt = self.context_recall_prompt.adapt(
             language, self.llm, cache_dir
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ragas-0.1.5/src/ragas/metrics/_context_relevancy.py` & `ragas-0.1.6/src/ragas/metrics/_context_relevancy.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/src/ragas/metrics/_faithfulness.py` & `ragas-0.1.6/src/ragas/metrics/_faithfulness.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,204 +1,233 @@
 from __future__ import annotations
 
+import json
 import logging
 import typing as t
 from dataclasses import dataclass, field
 
 import numpy as np
+from langchain_core.pydantic_v1 import BaseModel, Field
 
-from ragas.llms.json_load import json_loader
+from ragas.llms.output_parser import RagasoutputParser, get_json_format_instructions
 from ragas.llms.prompt import Prompt
 from ragas.metrics.base import EvaluationMode, MetricWithLLM
 
 if t.TYPE_CHECKING:
     from langchain_core.callbacks import Callbacks
 
     from ragas.llms.prompt import PromptValue
 
 logger = logging.getLogger(__name__)
 
+
+class StatementsAnswers(BaseModel):
+    __root__: t.List[str] = Field(..., description="the list of extracted statements")
+
+    def dicts(self) -> t.List[t.Dict]:
+        return self.dict()["__root__"]
+
+
+_statements_output_instructions = get_json_format_instructions(StatementsAnswers)
+_statements_output_parser = RagasoutputParser(pydantic_object=StatementsAnswers)
+
+
 LONG_FORM_ANSWER_PROMPT = Prompt(
     name="long_form_answer",
     instruction="Create one or more statements from each sentence in the given answer.",
+    output_format_instruction=_statements_output_instructions,
     examples=[
         {
             "question": "Who was  Albert Einstein and what is he best known for?",
             "answer": "He was a German-born theoretical physicist, widely acknowledged to be one of the greatest and most influential physicists of all time. He was best known for developing the theory of relativity, he also made important contributions to the development of the theory of quantum mechanics.",
-            "statements": {
-                "statements": [
+            "statements": StatementsAnswers.parse_obj(
+                [
                     "Albert Einstein, a German-born theoretical physicist, is renowned for being one of the most influential physicists in history.",
                     "Albert Einstein was best known for his theory of relativity.",
                     "Einstein's contributions significantly advanced the field of quantum mechanics",
                     "Recognized globally, Einstein's work has profoundly impacted the scientific community",
                     "Einstein's groundbreaking theories continue to shape our understanding of physics today.",
                 ]
-            },
+            ).dicts(),
         },
         {
             "question": "Cadmium Chloride is slightly soluble in this chemical, it is also called what?",
             "answer": "alcohol",
-            "statements": {
-                "statements": ["Cadmium Chloride is slightly soluble in alcohol."]
-            },
+            "statements": StatementsAnswers.parse_obj(
+                ["Cadmium Chloride is slightly soluble in alcohol."]
+            ).dicts(),
         },
         {
             "question": "Were Hitler and Benito Mussolini of the same nationality?",
             "answer": "Sorry, I can't provide answer to that question.",
-            "statements": {"statements": []},
+            "statements": StatementsAnswers.parse_obj([]).dicts(),
         },
     ],
     input_keys=["question", "answer"],
     output_key="statements",
-    output_type="JSON",
+    output_type="json",
 )  # noqa: E501
 
 
+class StatementFaithfulnessAnswer(BaseModel):
+    statement: str = Field(..., description="the original statement, word-by-word")
+    verdict: int = Field(..., description="the verdict(0/1) of the faithfulness.")
+    reason: str = Field(..., description="the reason of the verdict")
+
+
+class StatementFaithfulnessAnswers(BaseModel):
+    __root__: t.List[StatementFaithfulnessAnswer]
+
+    def dicts(self) -> t.List[t.Dict]:
+        return self.dict()["__root__"]
+
+
+_faithfulness_output_instructions = get_json_format_instructions(
+    StatementFaithfulnessAnswers
+)
+_faithfulness_output_parser = RagasoutputParser(
+    pydantic_object=StatementFaithfulnessAnswers
+)
+
 NLI_STATEMENTS_MESSAGE = Prompt(
     name="nli_statements",
-    instruction="Natural language inference. Use only 'Yes' (1), 'No' (0)",
+    instruction="Your task is to judge the faithfulness of a series of statements based on a given context. For each statement you must return verdict as 1 if the statement can be verified based on the context or 0 if the statement can not be verified based on the context.",
+    output_format_instruction=_faithfulness_output_instructions,
     examples=[
         {
             "context": """John is a student at XYZ University. He is pursuing a degree in Computer Science. He is enrolled in several courses this semester, including Data Structures, Algorithms, and Database Management. John is a diligent student and spends a significant amount of time studying and completing assignments. He often stays late in the library to work on his projects.""",
-            "statements": """
-            statement_1: John is majoring in Biology.
-            statement_2: John is taking a course on Artificial Intelligence.
-            statement_3: John is a dedicated student.
-            statement_4: John has a part-time job.
-            """,
-            "answer": [
-                {
-                    "statement_1": "John is majoring in Biology.",
-                    "reason": "John's major is explicitly mentioned as Computer Science. There is no information suggesting he is majoring in Biology.",
-                    "verdict": "0",
-                },
-                {
-                    "statement_2": "John is taking a course on Artificial Intelligence.",
-                    "reason": "The context mentions the courses John is currently enrolled in, and Artificial Intelligence is not mentioned. Therefore, it cannot be deduced that John is taking a course on AI.",
-                    "verdict": "0",
-                },
-                {
-                    "statement_3": "John is a dedicated student.",
-                    "reason": "The context states that he spends a significant amount of time studying and completing assignments. Additionally, it mentions that he often stays late in the library to work on his projects, which implies dedication.",
-                    "verdict": "1",
-                },
-                {
-                    "statement_4": "John has a part-time job.",
-                    "reason": "There is no information given in the context about John having a part-time job.",
-                    "verdict": "0",
-                },
+            "statements": [
+                "John is majoring in Biology.",
+                "John is taking a course on Artificial Intelligence.",
+                "John is a dedicated student.",
+                "John has a part-time job.",
             ],
+            "answer": StatementFaithfulnessAnswers.parse_obj(
+                [
+                    {
+                        "statement": "John is majoring in Biology.",
+                        "reason": "John's major is explicitly mentioned as Computer Science. There is no information suggesting he is majoring in Biology.",
+                        "verdict": 0,
+                    },
+                    {
+                        "statement": "John is taking a course on Artificial Intelligence.",
+                        "reason": "The context mentions the courses John is currently enrolled in, and Artificial Intelligence is not mentioned. Therefore, it cannot be deduced that John is taking a course on AI.",
+                        "verdict": 0,
+                    },
+                    {
+                        "statement": "John is a dedicated student.",
+                        "reason": "The context states that he spends a significant amount of time studying and completing assignments. Additionally, it mentions that he often stays late in the library to work on his projects, which implies dedication.",
+                        "verdict": 1,
+                    },
+                    {
+                        "statement": "John has a part-time job.",
+                        "reason": "There is no information given in the context about John having a part-time job.",
+                        "verdict": 0,
+                    },
+                ]
+            ).dicts(),
         },
         {
             "context": """Photosynthesis is a process used by plants, algae, and certain bacteria to convert light energy into chemical energy.""",
-            "statements": """statement_1: Albert Einstein was a genius.""",
-            "answer": {
-                "statement_1": "Albert Einstein was a genius.",
-                "reason": "The context and statement are unrelated",
-                "verdict": "0",
-            },
+            "statements": ["Albert Einstein was a genius."],
+            "answer": StatementFaithfulnessAnswers.parse_obj(
+                [
+                    {
+                        "statement": "Albert Einstein was a genius.",
+                        "reason": "The context and statement are unrelated",
+                        "verdict": 0,
+                    },
+                ]
+            ).dicts(),
         },
     ],
     input_keys=["context", "statements"],
     output_key="answer",
-    output_type="JSON",
+    output_type="json",
 )  # noqa: E501
 
 
 @dataclass
 class Faithfulness(MetricWithLLM):
     name: str = "faithfulness"  # type: ignore
     evaluation_mode: EvaluationMode = EvaluationMode.qac  # type: ignore
     long_form_answer_prompt: Prompt = field(
         default_factory=lambda: LONG_FORM_ANSWER_PROMPT
     )
     nli_statements_message: Prompt = field(
         default_factory=lambda: NLI_STATEMENTS_MESSAGE
     )
+    max_retries: int = 1
 
     def _create_answer_prompt(self, row: t.Dict) -> PromptValue:
         question, answer = row["question"], row["answer"]
 
         # extract statements from answer given the question
         prompt_value = self.long_form_answer_prompt.format(
             question=question, answer=answer
         )
         return prompt_value
 
-    def _create_nli_prompt(self, row: t.Dict, statements: t.Any) -> PromptValue:
+    def _create_nli_prompt(self, row: t.Dict, statements: t.List[str]) -> PromptValue:
         assert self.llm is not None, "llm must be set to compute score"
 
         contexts = row["contexts"]
         # check if the statements are support in the contexts
         contexts_str: str = "\n".join(contexts)
-        statements_str: str = "\n".join(
-            [f"statement_{i+1}: {st}" for i, st in enumerate(statements)]
-        )
+        statements_str: str = json.dumps(statements)
         prompt_value = self.nli_statements_message.format(
             context=contexts_str, statements=statements_str
         )
         return prompt_value
 
-    def _compute_score(self, output: t.Any):
+    def _compute_score(self, answers: StatementFaithfulnessAnswers):
         # check the verdicts and compute the score
-        verdict_score_map = {"1": 1, "0": 0}
-        output = output if isinstance(output, list) else [output]
         faithful_statements = sum(
-            verdict_score_map.get(
-                str(statement_with_validation.get("verdict", "")), np.nan
-            )
-            if isinstance(statement_with_validation, dict)
-            else np.nan
-            for statement_with_validation in output
+            1 if answer.verdict else 0 for answer in answers.__root__
         )
-        num_statements = len(output)
+        num_statements = len(answers.__root__)
         if num_statements:
             score = faithful_statements / num_statements
         else:
-            logger.warning(
-                "Invalid JSON response. Expected dictionary with key 'verdict'"
-            )
+            logger.warning("No statements were generated from the answer.")
             score = np.nan
 
         return score
 
     async def _ascore(
         self: t.Self, row: t.Dict, callbacks: Callbacks, is_async: bool
     ) -> float:
         """
         returns the NLI score for each (q, c, a) pair
         """
         assert self.llm is not None, "LLM is not set"
-        p = self._create_answer_prompt(row)
+        p_value = self._create_answer_prompt(row)
         answer_result = await self.llm.generate(
-            p, callbacks=callbacks, is_async=is_async
+            p_value, callbacks=callbacks, is_async=is_async
         )
-        statements = await json_loader.safe_load(
-            text=answer_result.generations[0][0].text,
-            llm=self.llm,
-            callbacks=callbacks,
-            is_async=is_async,
-        )
-
-        statements = statements if isinstance(statements, dict) else {}
-        statements = statements.get("statements", [])
-        if statements:
-            p = self._create_nli_prompt(row, statements)
-            nli_result = await self.llm.generate(
-                p, callbacks=callbacks, is_async=is_async
-            )
-            json_output = await json_loader.safe_load(
-                text=nli_result.generations[0][0].text,
-                llm=self.llm,
-                callbacks=callbacks,
-                is_async=is_async,
-            )
-        else:
-            json_output = [{}]
-        return self._compute_score(json_output)
+        answer_result_text = answer_result.generations[0][0].text
+        statements = await _statements_output_parser.aparse(
+            answer_result_text, p_value, self.llm, self.max_retries
+        )
+        if statements is None:
+            return np.nan
+
+        p_value = self._create_nli_prompt(row, statements.__root__)
+        nli_result = await self.llm.generate(
+            p_value, callbacks=callbacks, is_async=is_async
+        )
+        nli_result_text = nli_result.generations[0][0].text
+
+        faithfulness = await _faithfulness_output_parser.aparse(
+            nli_result_text, p_value, self.llm, self.max_retries
+        )
+        if faithfulness is None:
+            return np.nan
+
+        return self._compute_score(faithfulness)
 
     def adapt(self, language: str, cache_dir: t.Optional[str] = None) -> None:
         assert self.llm is not None, "LLM is not set"
 
         logger.info(f"Adapting Faithfulness metric to {language}")
         self.long_form_answer_prompt = self.long_form_answer_prompt.adapt(
             language, self.llm, cache_dir
```

### Comparing `ragas-0.1.5/src/ragas/metrics/base.py` & `ragas-0.1.6/src/ragas/metrics/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Q - question
 A - answer: generated_text from RAG pipeline
 C - contexts: context used for generation
 G - ground_truth: ground truth answer
 """
+
 from __future__ import annotations
 
 import asyncio
 import typing as t
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from enum import Enum
@@ -21,25 +22,45 @@
     from ragas.embeddings import BaseRagasEmbeddings
     from ragas.llms import BaseRagasLLM
 
 
 EvaluationMode = Enum("EvaluationMode", "qac qa qc gc ga qga qcg")
 
 
+def get_required_columns(
+    eval_mod: EvaluationMode, ignore_columns: t.Optional[t.List[str]] = None
+) -> t.List[str]:
+    if eval_mod == EvaluationMode.qac:
+        keys = ["question", "answer", "contexts"]
+    elif eval_mod == EvaluationMode.qa:
+        keys = ["question", "answer"]
+    elif eval_mod == EvaluationMode.qc:
+        keys = ["question", "contexts"]
+    elif eval_mod == EvaluationMode.gc:
+        keys = ["contexts", "ground_truth"]
+    elif eval_mod == EvaluationMode.ga:
+        keys = ["answer", "ground_truth"]
+    elif eval_mod == EvaluationMode.qga:
+        keys = ["question", "contexts", "answer", "ground_truth"]
+    elif eval_mod == EvaluationMode.qcg:
+        keys = ["question", "contexts", "ground_truth"]
+    ignore_columns = ignore_columns or []
+
+    return [k for k in keys if k not in ignore_columns]
+
+
 @dataclass
 class Metric(ABC):
     @property
     @abstractmethod
-    def name(self) -> str:
-        ...
+    def name(self) -> str: ...
 
     @property
     @abstractmethod
-    def evaluation_mode(self) -> EvaluationMode:
-        ...
+    def evaluation_mode(self) -> EvaluationMode: ...
 
     @abstractmethod
     def init(self, run_config: RunConfig):
         """
         This method will lazy initialize the model.
         """
         ...
@@ -93,16 +114,17 @@
             raise e
         else:
             if not group_cm.ended:
                 rm.on_chain_end({"output": score})
         return score
 
     @abstractmethod
-    async def _ascore(self, row: t.Dict, callbacks: Callbacks, is_async: bool) -> float:
-        ...
+    async def _ascore(
+        self, row: t.Dict, callbacks: Callbacks, is_async: bool
+    ) -> float: ...
 
 
 @dataclass
 class MetricWithLLM(Metric):
     llm: t.Optional[BaseRagasLLM] = None
 
     def init(self, run_config: RunConfig):
```

### Comparing `ragas-0.1.5/src/ragas/metrics/critique.py` & `ragas-0.1.6/src/ragas/metrics/critique.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,43 +2,56 @@
 
 import logging
 import typing as t
 from collections import Counter
 from dataclasses import dataclass, field
 
 import numpy as np
+from langchain_core.pydantic_v1 import BaseModel
 
-from ragas.llms.json_load import json_loader
+from ragas.llms.output_parser import RagasoutputParser, get_json_format_instructions
 from ragas.llms.prompt import Prompt
 from ragas.metrics.base import EvaluationMode, MetricWithLLM
 
 if t.TYPE_CHECKING:
     from langchain_core.callbacks.base import Callbacks
 
     from ragas.llms import BaseRagasLLM
 
 logger = logging.getLogger(__name__)
 
+
+class CriticClassification(BaseModel):
+    reason: str
+    verdict: int
+
+
+_output_instructions = get_json_format_instructions(CriticClassification)
+_output_parser = RagasoutputParser(pydantic_object=CriticClassification)
+
 CRITIQUE_PROMPT = Prompt(
     name="critique",
     instruction="Given a input and submission. Evaluate the submission only using the given criteria. Use only 'Yes' (1) and 'No' (0) as verdict.",
+    output_format_instruction=_output_instructions,
     examples=[
         {
             "input": "Who was the director of Los Alamos Laboratory?",
             "submission": "Einstein was the director of  Los Alamos Laboratory.",
             "criteria": "Is the output written in perfect grammar",
-            "output": {
-                "reason": "the criteria for evaluation is whether the output is written in perfect grammar. In this case, the output is grammatically correct.",
-                "verdict": "1",
-            },
+            "output": CriticClassification.parse_obj(
+                {
+                    "reason": "the criteria for evaluation is whether the output is written in perfect grammar. In this case, the output is grammatically correct.",
+                    "verdict": 1,
+                }
+            ).dict(),
         }
     ],
     input_keys=["input", "submission", "criteria"],
     output_key="output",
-    output_type="JSON",
+    output_type="json",
 )  # noqa: E501
 
 
 @dataclass
 class AspectCritique(MetricWithLLM):
     """
     Judges the submission to give binary results using the criteria specified
@@ -63,14 +76,15 @@
     critic_prompt: Prompt = field(default_factory=lambda: CRITIQUE_PROMPT)
     definition: str = field(default="", repr=True)
     strictness: int = field(default=1, repr=False)
     llm: BaseRagasLLM | None = field(
         default=None,
         repr=False,
     )
+    max_retries: int = 1
 
     def __post_init__(self: t.Self):
         if self.name == "":
             raise ValueError("Expects a name")
         if self.definition == "":
             raise ValueError("Expects definition")
 
@@ -89,47 +103,47 @@
             if isinstance(context, list):
                 context = "\n".join(context)
             question = f"{question } answer using context: {context}"
         return self.critic_prompt.format(
             input=question, submission=answer, criteria=self.definition
         )
 
-    def _compute_score(self, safe_loaded_responses):
-        ANSWER_DICT = {"1": 1, "0": 0}
+    def _compute_score(self, safe_loaded_responses: t.List[CriticClassification]):
         if self.strictness > 1:
             score = Counter(
-                [
-                    ANSWER_DICT.get(item.get("verdict", np.nan), np.nan)
-                    for item in safe_loaded_responses
-                ]
+                [item.verdict for item in safe_loaded_responses]
             ).most_common(1)[0][0]
         else:
-            score = ANSWER_DICT.get(
-                safe_loaded_responses[0].get("verdict", np.nan), np.nan
-            )
+            score = safe_loaded_responses[0].verdict
 
         return score
 
     async def _ascore(
         self: t.Self, row: t.Dict, callbacks: Callbacks, is_async: bool
     ) -> float:
         assert self.llm is not None, "set LLM before use"
 
         q, c, a = row["question"], row["contexts"], row["answer"]
 
+        p_value = self.prompt_format(q, a, c)
         result = await self.llm.generate(
-            self.prompt_format(q, a, c), callbacks=callbacks, is_async=is_async
+            p_value, callbacks=callbacks, is_async=is_async
         )
 
         responses = [r.text for r in result.generations[0]]
         safe_loaded_responses = [
-            await json_loader.safe_load(r, self.llm, is_async=is_async)
+            await _output_parser.aparse(r, p_value, self.llm, self.max_retries)
             for r in responses
         ]
+        if any(item is None for item in safe_loaded_responses):
+            return np.nan
 
+        safe_loaded_responses = [
+            item for item in safe_loaded_responses if item is not None
+        ]
         return self._compute_score(safe_loaded_responses)
 
     def adapt(self, language: str, cache_dir: str | None = None) -> None:
         assert self.llm is not None, "set LLM before use"
 
         logger.info(f"Adapting Critic to {language}")
         self.critic_prompt.adapt(language, self.llm, cache_dir)
```

### Comparing `ragas-0.1.5/src/ragas/run_config.py` & `ragas-0.1.6/src/ragas/run_config.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/src/ragas/testset/docstore.py` & `ragas-0.1.6/src/ragas/testset/docstore.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/src/ragas/testset/evolutions.py` & `ragas-0.1.6/src/ragas/testset/evolutions.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
         )
 
         return DataRow(
             question=question.strip('"'),
             contexts=[n.page_content for n in relevant_context.nodes],
             ground_truth=answer,
             evolution_type=evolution_type,
-            metadata=[n.metadata for n in relevant_context.nodes]
+            metadata=[n.metadata for n in relevant_context.nodes],
         )
 
     def adapt(self, language: str, cache_dir: t.Optional[str] = None) -> None:
         """
         Adapt the filter to a different language.
         """
         assert self.node_filter is not None, "node filter cannot be None"
```

### Comparing `ragas-0.1.5/src/ragas/testset/extractor.py` & `ragas-0.1.6/src/ragas/testset/extractor.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/src/ragas/testset/filters.py` & `ragas-0.1.6/src/ragas/testset/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import logging
 import typing as t
 from abc import ABC
 from dataclasses import dataclass, field
 
-
 from ragas.llms.json_load import json_loader
 from ragas.run_config import RunConfig
 from ragas.testset.prompts import (
     context_scoring_prompt,
     evolution_elimination_prompt,
     filter_question_prompt,
 )
```

### Comparing `ragas-0.1.5/src/ragas/testset/generator.py` & `ragas-0.1.6/src/ragas/testset/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         self,
         documents: t.Sequence[LlamaindexDocument],
         test_size: int,
         distributions: t.Optional[Distributions] = None,
         with_debugging_logs=False,
         is_async: bool = True,
         raise_exceptions: bool = True,
-        run_config: t.Optional[RunConfig] = None
+        run_config: t.Optional[RunConfig] = None,
     ):
         distributions = distributions or {}
         # chunk documents and add to docstore
         self.docstore.add_documents(
             [Document.from_llamaindex_document(doc) for doc in documents]
         )
 
@@ -164,15 +164,15 @@
         self,
         documents: t.Sequence[LCDocument],
         test_size: int,
         distributions: t.Optional[Distributions] = None,
         with_debugging_logs=False,
         is_async: bool = True,
         raise_exceptions: bool = True,
-        run_config: t.Optional[RunConfig] = None
+        run_config: t.Optional[RunConfig] = None,
     ):
         distributions = distributions or {}
         # chunk documents and add to docstore
         self.docstore.add_documents(
             [Document.from_langchain_document(doc) for doc in documents]
         )
 
@@ -203,15 +203,15 @@
     def generate(
         self,
         test_size: int,
         distributions: t.Optional[Distributions] = None,
         with_debugging_logs=False,
         is_async: bool = True,
         raise_exceptions: bool = True,
-        run_config: t.Optional[RunConfig] = None
+        run_config: t.Optional[RunConfig] = None,
     ):
         distributions = distributions or DEFAULT_DISTRIBUTION
         # validate distributions
         if not check_if_sum_is_close(list(distributions.values()), 1.0, 3):
             raise ValueError(
                 f"distributions passed do not sum to 1.0 [got {sum(list(distributions.values()))}]. Please check the "
                 f"distributions."
```

### Comparing `ragas-0.1.5/src/ragas/testset/prompts.py` & `ragas-0.1.6/src/ragas/testset/prompts.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             "question": "What does the append() method do in Python?",
             "context": "In Python, lists are used to store multiple items in a single variable. Lists are one of 4 built-in data types used to store collections of data. The append() method adds a single item to the end of a list.",
             "output": "If a list represents a variable collection, what method extends it by one item?",
         },
     ],
     input_keys=["question", "context"],
     output_key="output",
-    output_type="string",
+    output_type="str",
     language="english",
 )
 
 
 multi_context_question_prompt = Prompt(
     name="multi_context_question",
     instruction="""
@@ -50,15 +50,15 @@
             "context1": "The area of a shape is calculated based on the shape's dimensions. For rectangles, this involves multiplying the length and width.",
             "context2": "Rectangles have four sides with opposite sides being equal in length. They are a type of quadrilateral.",
             "output": "What multiplication involving equal opposites yields a quadrilateral's area?",
         },
     ],
     input_keys=["question", "context1", "context2"],
     output_key="output",
-    output_type="string",
+    output_type="str",
     language="english",
 )
 
 conditional_question_prompt = Prompt(
     name="conditional_question",
     instruction="""Rewrite the provided question to increase its complexity by introducing a conditional element.
     The goal is to make the question more intricate by incorporating a scenario or condition that affects the context of the question.
@@ -77,15 +77,15 @@
             "question": "How do vaccines protect against diseases?",
             "context": "Vaccines protect against diseases by stimulating the body's immune response to produce antibodies, which recognize and combat pathogens.",
             "output": "How do vaccines utilize the body's immune system to defend against pathogens?",
         },
     ],
     input_keys=["question", "context"],
     output_key="output",
-    output_type="string",
+    output_type="str",
     language="english",
 )
 
 
 compress_question_prompt = Prompt(
     name="compress_question",
     instruction="""Rewrite the following question to make it more indirect and shorter while retaining the essence of the original question.
@@ -98,15 +98,15 @@
         {
             "question": "What ingredients are required to bake a chocolate cake?",
             "output": "What's needed for a chocolate cake?",
         },
     ],
     input_keys=["question"],
     output_key="output",
-    output_type="string",
+    output_type="str",
     language="english",
 )
 
 
 conversational_question_prompt = Prompt(
     name="conversation_question",
     instruction="""Reformat the provided question into two separate questions as if it were to be part of a conversation. Each question should focus on a specific aspect or subtopic related to the original question.
@@ -147,15 +147,15 @@
         {
             "context": "Albert Einstein (14 March 1879 - 18 April 1955) was a German-born theoretical physicist who is widely held to be one of the greatest and most influential scientists of all time.",
             "output": {"score": 6.0},
         },
         {
             "context": "I love chocolate. It's really tasty. Oh, and by the way, the earth orbits the sun, not the other way around. Also, my favorite color is blue.",
             "output": {"score": 2.0},
-        }
+        },
     ],
     input_keys=["context"],
     output_key="output",
     output_type="json",
     language="english",
 )
 
@@ -174,15 +174,15 @@
             "question": "What datasets were used for the zero-shot evaluations in this study?",
             "feedback": "The question asks about the datasets used for zero-shot evaluations in 'this study', without specifying or providing any details about the study in question. This makes the question unclear for those who do not have access to or knowledge of the specific study. To improve clarity and answerability, the question should specify the study it refers to, or provide enough context about the study for the question to be understood and answered independently.",
             "output": "What datasets were used for the zero-shot evaluations Exploring Zero-Shot Learning in Neural Networks paper?",
         },
     ],
     input_keys=["context", "question", "feedback"],
     output_key="output",
-    output_type="string",
+    output_type="str",
     language="english",
 )
 
 
 filter_question_prompt = Prompt(
     name="filter_question",
     instruction="""
@@ -359,15 +359,15 @@
             "context": "The process of evaporation plays a crucial role in the water cycle, converting water from liquid to vapor and allowing it to rise into the atmosphere.",
             "keyphrase": "Evaporation",
             "question": "Why is evaporation important in the water cycle?",
         },
     ],
     input_keys=["context", "keyphrase"],
     output_key="question",
-    output_type="string",
+    output_type="str",
 )
 
 main_topic_extraction_prompt = Prompt(
     name="main_topic_extraction",
     instruction="Identify and extract the two main topics discussed in depth in the given text.",
     examples=[
         {
```

### Comparing `ragas-0.1.5/src/ragas/utils.py` & `ragas-0.1.6/src/ragas/utils.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/src/ragas/validation.py` & `ragas-0.1.6/src/ragas/validation.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/src/ragas.egg-info/PKG-INFO` & `ragas-0.1.6/src/ragas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragas
-Version: 0.1.5
+Version: 0.1.6
 Description-Content-Type: text/plain
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: datasets
 Requires-Dist: tiktoken
 Requires-Dist: langchain
 Requires-Dist: langchain-core
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ragas Version: 0.1.5 Description-Content-Type:
+Metadata-Version: 2.1 Name: ragas Version: 0.1.6 Description-Content-Type:
 text/plain License-File: LICENSE Requires-Dist: numpy Requires-Dist: datasets
 Requires-Dist: tiktoken Requires-Dist: langchain Requires-Dist: langchain-core
 Requires-Dist: langchain-community Requires-Dist: langchain_openai Requires-
 Dist: openai>1 Requires-Dist: pysbd>=0.3.4 Requires-Dist: nest-asyncio
 Requires-Dist: appdirs Provides-Extra: all Requires-Dist: sentence-
 transformers; extra == "all"
                  ************ [[..//ddooccss//__ssttaattiicc//iimmggss//llooggoo..ppnngg]] ************
```

### Comparing `ragas-0.1.5/src/ragas.egg-info/SOURCES.txt` & `ragas-0.1.6/src/ragas.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 docs/_static/imgs/eval-evolve.png
 docs/_static/imgs/langsmith-tracing-faithfullness.png
 docs/_static/imgs/langsmith-tracing-overview.png
 docs/_static/imgs/logo.png
 docs/_static/imgs/question_types.png
 docs/_static/imgs/quickstart-output.png
 docs/_static/imgs/ragas-logo.png
+docs/_static/imgs/ragas_workflow_white.png
 docs/_static/imgs/testset_output.png
 docs/_static/imgs/trace-langsmith.png
 docs/_static/js/mendable_chat_bubble.js
 docs/_static/js/octolane.js
 docs/community/index.md
 docs/concepts/feedback.md
 docs/concepts/index.md
@@ -66,14 +67,15 @@
 docs/concepts/metrics/faithfulness.md
 docs/concepts/metrics/index.md
 docs/concepts/metrics/semantic_similarity.md
 docs/getstarted/evaluation.md
 docs/getstarted/index.md
 docs/getstarted/install.md
 docs/getstarted/monitoring.md
+docs/getstarted/prepare_data.ipynb
 docs/getstarted/testset_generation.md
 docs/howtos/index.md
 docs/howtos/applications/compare_embeddings.md
 docs/howtos/applications/compare_llms.md
 docs/howtos/applications/custom_prompts.md
 docs/howtos/applications/data_preparation.md
 docs/howtos/applications/index.md
@@ -86,14 +88,15 @@
 docs/howtos/customisations/index.md
 docs/howtos/integrations/athina.ipynb
 docs/howtos/integrations/index.md
 docs/howtos/integrations/langchain.ipynb
 docs/howtos/integrations/langfuse.ipynb
 docs/howtos/integrations/langsmith.ipynb
 docs/howtos/integrations/llamaindex.ipynb
+docs/howtos/integrations/openlayer.ipynb
 docs/howtos/integrations/ragas-arize.ipynb
 docs/howtos/integrations/ragas_haystack.ipynb
 docs/howtos/integrations/tonic-validate.ipynb
 docs/howtos/integrations/zeno.ipynb
 docs/howtos/integrations/nyc_wikipedia/nyc_text.txt
 docs/references/evaluation.rst
 docs/references/index.rst
@@ -117,17 +120,21 @@
 src/ragas.egg-info/PKG-INFO
 src/ragas.egg-info/SOURCES.txt
 src/ragas.egg-info/dependency_links.txt
 src/ragas.egg-info/requires.txt
 src/ragas.egg-info/top_level.txt
 src/ragas/embeddings/__init__.py
 src/ragas/embeddings/base.py
+src/ragas/integrations/__init__.py
+src/ragas/integrations/langchain.py
+src/ragas/integrations/langsmith.py
 src/ragas/llms/__init__.py
 src/ragas/llms/base.py
 src/ragas/llms/json_load.py
+src/ragas/llms/output_parser.py
 src/ragas/llms/prompt.py
 src/ragas/metrics/__init__.py
 src/ragas/metrics/_answer_correctness.py
 src/ragas/metrics/_answer_relevance.py
 src/ragas/metrics/_answer_similarity.py
 src/ragas/metrics/_context_entities_recall.py
 src/ragas/metrics/_context_precision.py
```

### Comparing `ragas-0.1.5/tests/benchmarks/benchmark_eval.py` & `ragas-0.1.6/tests/benchmarks/benchmark_eval.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/tests/benchmarks/benchmark_testsetgen.py` & `ragas-0.1.6/tests/benchmarks/benchmark_testsetgen.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/tests/benchmarks/utils.py` & `ragas-0.1.6/tests/benchmarks/utils.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/tests/conftest.py` & `ragas-0.1.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/tests/unit/llms/test_llm.py` & `ragas-0.1.6/tests/unit/llms/test_llm.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/tests/unit/llms/test_prompt.py` & `ragas-0.1.6/tests/unit/llms/test_prompt.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/tests/unit/test_analytics.py` & `ragas-0.1.6/tests/unit/test_analytics.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/tests/unit/test_import.py` & `ragas-0.1.6/tests/unit/test_import.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/tests/unit/test_validation.py` & `ragas-0.1.6/tests/unit/test_validation.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/tests/unit/testset_generator/test_docstore.py` & `ragas-0.1.6/tests/unit/testset_generator/test_docstore.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/tests/unit/testset_generator/test_document.py` & `ragas-0.1.6/tests/unit/testset_generator/test_document.py`

 * *Files identical despite different names*

### Comparing `ragas-0.1.5/tests/unit/testset_generator/test_embs.pkl` & `ragas-0.1.6/tests/unit/testset_generator/test_embs.pkl`

 * *Files identical despite different names*

