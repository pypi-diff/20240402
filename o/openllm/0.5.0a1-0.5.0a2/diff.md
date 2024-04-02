# Comparing `tmp/openllm-0.5.0a1.tar.gz` & `tmp/openllm-0.5.0a2.tar.gz`

## Comparing `openllm-0.5.0a1.tar` & `openllm-0.5.0a2.tar`

### file list

```diff
@@ -1,77 +1,78 @@
--rw-r--r--   0        0        0    42117 2020-02-02 00:00:00.000000 openllm-0.5.0a1/CHANGELOG.md
--rw-r--r--   0        0        0    45993 2020-02-02 00:00:00.000000 openllm-0.5.0a1/README.md
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 openllm-0.5.0a1/pyoxidizer.bzl
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/_service_vars.pyi
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/_openllm_tiny/__init__.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/_openllm_tiny/__init__.pyi
--rw-r--r--   0        0        0    19139 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/_openllm_tiny/_entrypoint.py
--rw-r--r--   0        0        0    12945 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/_openllm_tiny/_helpers.py
--rw-r--r--   0        0        0     7748 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/_openllm_tiny/_llm.py
--rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/_openllm_tiny/_service.py
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/_openllm_tiny/_service_vars.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/_openllm_tiny/bentofile.yaml
--rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/__init__.py
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/__init__.pyi
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/__main__.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/_deprecated.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/_generation.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/_generation.pyi
--rw-r--r--   0        0        0    19732 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/_llm.py
--rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/_llm.pyi
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/_quantisation.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/_quantisation.pyi
--rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/_runners.py
--rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/_runners.pyi
--rw-r--r--   0        0        0    12147 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/_strategies.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/_strategies.pyi
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/_version.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/client.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/client.pyi
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/py.typed
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/utils.py
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/utils.pyi
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/bundle/__init__.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/bundle/__init__.pyi
--rw-r--r--   0        0        0     6054 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/bundle/_package.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/bundle/_package.pyi
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/entrypoints/__init__.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/entrypoints/__init__.pyi
--rw-r--r--   0        0        0    20050 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/entrypoints/_openapi.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/entrypoints/_openapi.pyi
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/entrypoints/hf.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/entrypoints/hf.pyi
--rw-r--r--   0        0        0    17566 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/entrypoints/openai.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/entrypoints/openai.pyi
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/models/__init__.py
--rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/serialisation/__init__.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/serialisation/__init__.pyi
--rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/serialisation/_helpers.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/serialisation/constants.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/serialisation/ggml/__init__.py
--rw-r--r--   0        0        0     8324 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/serialisation/transformers/__init__.py
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/serialisation/transformers/_helpers.py
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/serialisation/transformers/weights.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm/serialisation/vllm/__init__.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm_cli/__init__.py
--rw-r--r--   0        0        0    12396 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm_cli/_factory.py
--rw-r--r--   0        0        0    12850 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm_cli/_sdk.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm_cli/termui.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm_cli/extension/__init__.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm_cli/extension/dive_bentos.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm_cli/extension/get_containerfile.py
--rw-r--r--   0        0        0     6734 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm_cli/extension/get_prompt.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm_cli/extension/list_bentos.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm_cli/extension/list_models.py
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm_cli/extension/playground.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm_cli/playground/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm_cli/playground/__init__.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm_cli/playground/_meta.yml
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm_cli/playground/falcon_tuned.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm_cli/playground/features.py
--rw-r--r--   0        0        0     8315 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm_cli/playground/llama2_qlora.py
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 openllm-0.5.0a1/src/openllm_cli/playground/opt_tuned.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 openllm-0.5.0a1/.gitignore
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.5.0a1/LICENSE.md
--rw-r--r--   0        0        0     7551 2020-02-02 00:00:00.000000 openllm-0.5.0a1/pyproject.toml
--rw-r--r--   0        0        0    52323 2020-02-02 00:00:00.000000 openllm-0.5.0a1/PKG-INFO
+-rw-r--r--   0        0        0    42218 2020-02-02 00:00:00.000000 openllm-0.5.0a2/CHANGELOG.md
+-rw-r--r--   0        0        0    45993 2020-02-02 00:00:00.000000 openllm-0.5.0a2/README.md
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 openllm-0.5.0a2/pyoxidizer.bzl
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/_service_vars.pyi
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/_openllm_tiny/Dockerfile.j2
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/_openllm_tiny/__init__.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/_openllm_tiny/__init__.pyi
+-rw-r--r--   0        0        0    19308 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/_openllm_tiny/_entrypoint.py
+-rw-r--r--   0        0        0    12945 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/_openllm_tiny/_helpers.py
+-rw-r--r--   0        0        0     7799 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/_openllm_tiny/_llm.py
+-rw-r--r--   0        0        0     5821 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/_openllm_tiny/_service.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/_openllm_tiny/_service_vars.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/_openllm_tiny/bentofile.yaml
+-rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/__init__.py
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/__init__.pyi
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/__main__.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/_deprecated.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/_generation.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/_generation.pyi
+-rw-r--r--   0        0        0    19732 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/_llm.py
+-rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/_llm.pyi
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/_quantisation.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/_quantisation.pyi
+-rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/_runners.py
+-rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/_runners.pyi
+-rw-r--r--   0        0        0    12147 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/_strategies.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/_strategies.pyi
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/_version.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/client.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/client.pyi
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/py.typed
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/utils.py
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/utils.pyi
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/bundle/__init__.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/bundle/__init__.pyi
+-rw-r--r--   0        0        0     6054 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/bundle/_package.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/bundle/_package.pyi
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/entrypoints/__init__.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/entrypoints/__init__.pyi
+-rw-r--r--   0        0        0    20050 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/entrypoints/_openapi.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/entrypoints/_openapi.pyi
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/entrypoints/hf.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/entrypoints/hf.pyi
+-rw-r--r--   0        0        0    17566 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/entrypoints/openai.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/entrypoints/openai.pyi
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/models/__init__.py
+-rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/serialisation/__init__.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/serialisation/__init__.pyi
+-rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/serialisation/_helpers.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/serialisation/constants.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/serialisation/ggml/__init__.py
+-rw-r--r--   0        0        0     8324 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/serialisation/transformers/__init__.py
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/serialisation/transformers/_helpers.py
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/serialisation/transformers/weights.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm/serialisation/vllm/__init__.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm_cli/__init__.py
+-rw-r--r--   0        0        0    12396 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm_cli/_factory.py
+-rw-r--r--   0        0        0    12850 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm_cli/_sdk.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm_cli/termui.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm_cli/extension/__init__.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm_cli/extension/dive_bentos.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm_cli/extension/get_containerfile.py
+-rw-r--r--   0        0        0     6734 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm_cli/extension/get_prompt.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm_cli/extension/list_bentos.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm_cli/extension/list_models.py
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm_cli/extension/playground.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm_cli/playground/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm_cli/playground/__init__.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm_cli/playground/_meta.yml
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm_cli/playground/falcon_tuned.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm_cli/playground/features.py
+-rw-r--r--   0        0        0     8315 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm_cli/playground/llama2_qlora.py
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 openllm-0.5.0a2/src/openllm_cli/playground/opt_tuned.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 openllm-0.5.0a2/.gitignore
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.5.0a2/LICENSE.md
+-rw-r--r--   0        0        0     7551 2020-02-02 00:00:00.000000 openllm-0.5.0a2/pyproject.toml
+-rw-r--r--   0        0        0    52323 2020-02-02 00:00:00.000000 openllm-0.5.0a2/PKG-INFO
```

### Comparing `openllm-0.5.0a1/CHANGELOG.md` & `openllm-0.5.0a2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 Do *NOT* add changelog entries here!
 
 This changelog is managed by towncrier and is compiled at release time.
 -->
 
 <!-- towncrier release notes start -->
 
+## [0.5.0-alpha.2](https://github.com/bentoml/openllm/tree/v0.5.0-alpha.2)
+No significant changes.
+
+
 ## [0.5.0-alpha.1](https://github.com/bentoml/openllm/tree/v0.5.0-alpha.1)
 No significant changes.
 
 
 ## [0.5.0-alpha](https://github.com/bentoml/openllm/tree/v0.5.0-alpha)
 
 ### Backwards-incompatible Changes
```

### Comparing `openllm-0.5.0a1/README.md` & `openllm-0.5.0a2/README.md`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/pyoxidizer.bzl` & `openllm-0.5.0a2/pyoxidizer.bzl`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/_service_vars.pyi` & `openllm-0.5.0a2/src/_service_vars.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/_openllm_tiny/__init__.pyi` & `openllm-0.5.0a2/src/_openllm_tiny/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/_openllm_tiny/_entrypoint.py` & `openllm-0.5.0a2/src/_openllm_tiny/_entrypoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import os, logging, traceback, pathlib, sys, fs, click, enum, inflection, bentoml, orjson, openllm, openllm_core, platform, typing as t
 from ._helpers import recommended_instance_type
 from openllm_core.utils import (
+  DEBUG,
   DEBUG_ENV_VAR,
   QUIET_ENV_VAR,
   SHOW_CODEGEN,
   check_bool_env,
   compose,
   first_not_none,
   dantic,
@@ -42,24 +43,18 @@
 import orjson,openllm_core.utils as coreutils
 model_id='{__model_id__}'
 model_name='{__model_name__}'
 quantise=coreutils.getenv('quantize',default='{__model_quantise__}',var=['QUANTISE'])
 serialisation=coreutils.getenv('serialization',default='{__model_serialization__}',var=['SERIALISATION'])
 dtype=coreutils.getenv('dtype', default='{__model_dtype__}', var=['TORCH_DTYPE'])
 trust_remote_code=coreutils.check_bool_env("TRUST_REMOTE_CODE",{__model_trust_remote_code__})
-max_model_len={__max_model_len__}
-gpu_memory_utilization={__gpu_memory_utilization__}
+max_model_len=orjson.loads(coreutils.getenv('max_model_len', default=orjson.dumps({__max_model_len__})))
+gpu_memory_utilization=orjson.loads(coreutils.getenv('gpu_memory_utilization', default=orjson.dumps({__gpu_memory_utilization__}), var=['GPU_MEMORY_UTILISATION']))
 services_config=orjson.loads(coreutils.getenv('services_config',"""{__services_config__}"""))
 '''
-_DOCKERFILE_TEMPLATE = """\
-{% extends bento_base_template %}
-{% block SETUP_BENTO_BASE_IMAGE %}
-{{ super() }}
-{% endblock %}
-"""
 
 
 class ItemState(enum.Enum):
   NOT_FOUND = 'NOT_FOUND'
   ADDED = 'ADDED'
   EXISTS = 'EXISTS'
   OVERWRITE = 'OVERWRITE'
@@ -265,30 +260,31 @@
     DEBUG_ENV_VAR: str(openllm.utils.get_debug_mode()),
     'MODEL_ID': model_id,
     'MODEL_NAME': model_name,
     'SERIALIZATION': serialisation,
     'OPENLLM_CONFIG': llm_config.model_dump_json(),
     'DTYPE': dtype,
     'TRUST_REMOTE_CODE': str(trust_remote_code),
-    'MAX_MODEL_LEN': orjson.dumps(max_model_len).decode(),
     'GPU_MEMORY_UTILIZATION': orjson.dumps(gpu_memory_utilization).decode(),
     'SERVICES_CONFIG': orjson.dumps(
       dict(
         resources={'gpu' if device else 'cpu': len(device) if device else 'cpu_count'}, traffic=dict(timeout=timeout)
       )
     ).decode(),
   })
+  if max_model_len is not None:
+    os.environ['MAX_MODEL_LEN'] = orjson.dumps(max_model_len)
   if quantize:
     os.environ['QUANTIZE'] = str(quantize)
 
   working_dir = os.path.abspath(os.path.dirname(__file__))
   if sys.path[0] != working_dir:
     sys.path.insert(0, working_dir)
   load('.', working_dir=working_dir).inject_config()
-  serve_http('.', working_dir=working_dir)
+  serve_http('.', working_dir=working_dir, reload=check_bool_env('RELOAD', default=False), development_mode=DEBUG)
 
 
 def construct_python_options(llm_config, llm_fs):
   from bentoml._internal.bento.build_config import PythonOptions
   from openllm.bundle._package import build_editable
 
   # TODO: Add this line back once 0.5 is out, for now depends on OPENLLM_DEV_BUILD
```

### Comparing `openllm-0.5.0a1/src/_openllm_tiny/_helpers.py` & `openllm-0.5.0a2/src/_openllm_tiny/_helpers.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/_openllm_tiny/_llm.py` & `openllm-0.5.0a2/src/_openllm_tiny/_llm.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,14 @@
     if is_vllm_available():
       num_gpus, dev = 1, openllm.utils.device_count()
       if dev >= 2:
         num_gpus = min(dev // 2 * 2, dev)
       quantise = self.quantise if self.quantise and self.quantise in {'gptq', 'awq', 'squeezellm'} else None
       dtype = 'float16' if quantise == 'gptq' else self.dtype  # NOTE: quantise GPTQ doesn't support bfloat16 yet.
 
-      self.engine_args.setdefault('gpu_memory_utilization', 0.9)
       self.engine_args.update({
         'worker_use_ray': False,
         'engine_use_ray': False,
         'tokenizer_mode': 'auto',
         'tensor_parallel_size': num_gpus,
         'model': self._path,
         'tokenizer': self._path,
@@ -77,14 +76,16 @@
         'dtype': dtype,
         'quantization': quantise,
       })
       if 'disable_log_stats' not in self.engine_args:
         self.engine_args['disable_log_stats'] = not get_debug_mode()
       if 'disable_log_requests' not in self.engine_args:
         self.engine_args['disable_log_requests'] = not get_debug_mode()
+      if 'gpu_memory_utilization' not in self.engine_args:
+        self.engine_args['gpu_memory_utilization'] = 0.9
 
       try:
         from vllm import AsyncEngineArgs, AsyncLLMEngine
 
         return AsyncLLMEngine.from_engine_args(AsyncEngineArgs(**self.engine_args))
       except Exception as err:
         traceback.print_exc()
```

### Comparing `openllm-0.5.0a1/src/_openllm_tiny/_service.py` & `openllm-0.5.0a2/src/_openllm_tiny/_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import importlib.metadata
 from http import HTTPStatus
 from starlette.requests import Request
 from starlette.responses import JSONResponse, StreamingResponse
 import openllm, bentoml, logging, openllm_core as core
 import _service_vars as svars, typing as t
 from openllm_core._typing_compat import Annotated
 from openllm_core._schemas import MessageParam, MessagesConverterInput
@@ -22,18 +23,24 @@
   model_id = bentomodel.path
 except Exception:
   bentomodel = None
   model_id = svars.model_id
 llm_config = core.AutoConfig.for_model(svars.model_name)
 GenerationInput = core.GenerationInput.from_config(llm_config)
 
-app_v1 = FastAPI(debug=True, description='OpenAI Compatible API support')
+app_v1 = FastAPI(
+  debug=True,
+  version=importlib.metadata.version('openllm'),
+  title='OpenAI',
+  description='OpenAI Compatible API support',
+  contact={'name': 'BentoML Team', 'email': 'contact@bentoml.com'},
+)
 
 
-@bentoml.mount_asgi_app(app_v1)
+@bentoml.mount_asgi_app(app_v1, path='/v1')
 @bentoml.service(name=f"llm-{llm_config['start_name']}-service", **svars.services_config)
 class LLMService:
   bentomodel = bentomodel
 
   def __init__(self):
     self.llm = openllm.LLM.from_model(
       model_id,
@@ -111,15 +118,15 @@
     ),
   ) -> str:
     return self.llm._tokenizer.apply_chat_template(
       message['messages'], add_generation_prompt=message['add_generation_prompt'], tokenize=False
     )
 
   @app_v1.post(
-    '/v1/chat/completions',
+    '/chat/completions',
     tags=['OpenAI'],
     status_code=HTTPStatus.OK,
     summary='Given a list of messages comprising a conversation, the model will return a response.',
     operation_id='openai__chat_completions',
   )
   async def chat_completions_v1(
     self,
@@ -141,26 +148,22 @@
       return JSONResponse(content=generator.model_dump(), status_code=int(t.cast(str, generator.error.code)))
     if request.stream is True:
       return StreamingResponse(generator, media_type='text/event-stream')
     return JSONResponse(content=generator.model_dump())
 
   # GET /v1/models
   @app_v1.get(
-    '/v1/models',
+    '/models',
     tags=['OpenAI'],
     status_code=HTTPStatus.OK,
     summary='Describes a model offering that can be used with the API.',
     operation_id='openai__list_models',
   )
   def list_models(self) -> ModelList:
     """
     List and describe the various models available in the API.
 
     You can refer to the available supported models with `openllm models` for more information.
     """
     return ModelList(
       data=[ModelCard(root=core.utils.normalise_model_name(model_id), id=core.utils.normalise_model_name(model_id))]
     )
-
-
-if __name__ == '__main__':
-  LLMService.serve_http(reload=core.utils.check_bool_env('RELOAD', False))
```

### Comparing `openllm-0.5.0a1/src/_openllm_tiny/_service_vars.py` & `openllm-0.5.0a2/src/_openllm_tiny/_service_vars.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import orjson, typing as t, openllm_core.utils as coreutils
+import orjson, openllm_core.utils as coreutils
 from openllm_core._typing_compat import LiteralSerialisation, LiteralQuantise
 from _openllm_tiny._llm import Dtype
 
 (
   model_id,
   model_name,
   quantise,
@@ -15,16 +15,11 @@
 ) = (
   coreutils.getenv('model_id', var=['MODEL_ID'], return_type=str),
   coreutils.getenv('model_name', return_type=str),
   coreutils.getenv('quantize', var=['QUANTISE'], return_type=LiteralQuantise),
   coreutils.getenv('serialization', default='safetensors', var=['SERIALISATION'], return_type=LiteralSerialisation),
   coreutils.getenv('dtype', default='auto', var=['TORCH_DTYPE'], return_type=Dtype),
   coreutils.check_bool_env('TRUST_REMOTE_CODE', False),
-  t.cast(t.Optional[int], orjson.loads(coreutils.getenv('max_model_len', default=orjson.dumps(None)))),
-  t.cast(
-    float,
-    orjson.loads(
-      coreutils.getenv('gpu_memory_utilization', default=orjson.dumps(0.9), var=['GPU_MEMORY_UTILISATION'])
-    ),
-  ),
-  t.cast(t.Dict[str, t.Any], orjson.loads(coreutils.getenv('services_config', orjson.dumps({})))),
+  orjson.loads(coreutils.getenv('max_model_len', default=orjson.dumps(None))),
+  orjson.loads(coreutils.getenv('gpu_memory_utilization', default=orjson.dumps(0.9), var=['GPU_MEMORY_UTILISATION'])),
+  orjson.loads(coreutils.getenv('services_config', orjson.dumps({}))),
 )
```

### Comparing `openllm-0.5.0a1/src/openllm/__init__.py` & `openllm-0.5.0a2/src/openllm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm/__init__.pyi` & `openllm-0.5.0a2/src/openllm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm/_deprecated.py` & `openllm-0.5.0a2/src/openllm/_deprecated.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm/_generation.py` & `openllm-0.5.0a2/src/openllm/_generation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm/_llm.py` & `openllm-0.5.0a2/src/openllm/_llm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm/_llm.pyi` & `openllm-0.5.0a2/src/openllm/_llm.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm/_quantisation.py` & `openllm-0.5.0a2/src/openllm/_quantisation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm/_quantisation.pyi` & `openllm-0.5.0a2/src/openllm/_quantisation.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm/_runners.py` & `openllm-0.5.0a2/src/openllm/_runners.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm/_runners.pyi` & `openllm-0.5.0a2/src/openllm/_runners.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm/_strategies.py` & `openllm-0.5.0a2/src/openllm/_strategies.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm/_strategies.pyi` & `openllm-0.5.0a2/src/openllm/_strategies.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm/utils.py` & `openllm-0.5.0a2/src/openllm/utils.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm/utils.pyi` & `openllm-0.5.0a2/src/openllm/utils.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm/bundle/__init__.py` & `openllm-0.5.0a2/src/openllm/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm/bundle/__init__.pyi` & `openllm-0.5.0a2/src/openllm/bundle/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm/bundle/_package.py` & `openllm-0.5.0a2/src/openllm/bundle/_package.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm/bundle/_package.pyi` & `openllm-0.5.0a2/src/openllm/bundle/_package.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm/entrypoints/_openapi.py` & `openllm-0.5.0a2/src/openllm/entrypoints/_openapi.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm/entrypoints/_openapi.pyi` & `openllm-0.5.0a2/src/openllm/entrypoints/_openapi.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm/entrypoints/hf.py` & `openllm-0.5.0a2/src/openllm/entrypoints/hf.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm/entrypoints/openai.py` & `openllm-0.5.0a2/src/openllm/entrypoints/openai.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm/entrypoints/openai.pyi` & `openllm-0.5.0a2/src/openllm/entrypoints/openai.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm/serialisation/__init__.py` & `openllm-0.5.0a2/src/openllm/serialisation/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm/serialisation/__init__.pyi` & `openllm-0.5.0a2/src/openllm/serialisation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm/serialisation/_helpers.py` & `openllm-0.5.0a2/src/openllm/serialisation/_helpers.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm/serialisation/transformers/__init__.py` & `openllm-0.5.0a2/src/openllm/serialisation/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm/serialisation/transformers/_helpers.py` & `openllm-0.5.0a2/src/openllm/serialisation/transformers/_helpers.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm/serialisation/transformers/weights.py` & `openllm-0.5.0a2/src/openllm/serialisation/transformers/weights.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm/serialisation/vllm/__init__.py` & `openllm-0.5.0a2/src/openllm/serialisation/vllm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm_cli/_factory.py` & `openllm-0.5.0a2/src/openllm_cli/_factory.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm_cli/_sdk.py` & `openllm-0.5.0a2/src/openllm_cli/_sdk.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm_cli/termui.py` & `openllm-0.5.0a2/src/openllm_cli/termui.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm_cli/extension/__init__.py` & `openllm-0.5.0a2/src/openllm_cli/extension/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm_cli/extension/dive_bentos.py` & `openllm-0.5.0a2/src/openllm_cli/extension/dive_bentos.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm_cli/extension/get_containerfile.py` & `openllm-0.5.0a2/src/openllm_cli/extension/get_containerfile.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm_cli/extension/get_prompt.py` & `openllm-0.5.0a2/src/openllm_cli/extension/get_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm_cli/extension/list_bentos.py` & `openllm-0.5.0a2/src/openllm_cli/extension/list_bentos.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm_cli/extension/list_models.py` & `openllm-0.5.0a2/src/openllm_cli/extension/list_models.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm_cli/extension/playground.py` & `openllm-0.5.0a2/src/openllm_cli/extension/playground.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm_cli/playground/_meta.yml` & `openllm-0.5.0a2/src/openllm_cli/playground/_meta.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm_cli/playground/falcon_tuned.py` & `openllm-0.5.0a2/src/openllm_cli/playground/falcon_tuned.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm_cli/playground/features.py` & `openllm-0.5.0a2/src/openllm_cli/playground/features.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm_cli/playground/llama2_qlora.py` & `openllm-0.5.0a2/src/openllm_cli/playground/llama2_qlora.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/src/openllm_cli/playground/opt_tuned.py` & `openllm-0.5.0a2/src/openllm_cli/playground/opt_tuned.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/.gitignore` & `openllm-0.5.0a2/.gitignore`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/LICENSE.md` & `openllm-0.5.0a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a1/pyproject.toml` & `openllm-0.5.0a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -36,16 +36,16 @@
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
     "bentoml[io]>=1.2",
     "transformers[torch,tokenizers]>=4.36.0",
-    "openllm-client>=0.5.0-alpha.1",
-    "openllm-core>=0.5.0-alpha.1",
+    "openllm-client>=0.5.0-alpha.2",
+    "openllm-core>=0.5.0-alpha.2",
     "safetensors",
     "optimum>=1.12.0",
     "accelerate",
     "ghapi",
     "einops",
     "sentencepiece",
     "scipy",
```

### Comparing `openllm-0.5.0a1/PKG-INFO` & `openllm-0.5.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openllm
-Version: 0.5.0a1
+Version: 0.5.0a2
 Summary: OpenLLM: Operating LLMs in production
 Project-URL: Blog, https://modelserving.com
 Project-URL: Chat, https://discord.gg/openllm
 Project-URL: Documentation, https://github.com/bentoml/openllm#readme
 Project-URL: GitHub, https://github.com/bentoml/OpenLLM
 Project-URL: History, https://github.com/bentoml/OpenLLM/blob/main/CHANGELOG.md
 Project-URL: Homepage, https://bentoml.com
@@ -42,16 +42,16 @@
 Requires-Dist: bentoml[io]>=1.2
 Requires-Dist: bitsandbytes<0.42
 Requires-Dist: build[virtualenv]<1
 Requires-Dist: click>=8.1.3
 Requires-Dist: cuda-python; platform_system != 'Darwin'
 Requires-Dist: einops
 Requires-Dist: ghapi
-Requires-Dist: openllm-client>=0.5.0-alpha.1
-Requires-Dist: openllm-core>=0.5.0-alpha.1
+Requires-Dist: openllm-client>=0.5.0-alpha.2
+Requires-Dist: openllm-core>=0.5.0-alpha.2
 Requires-Dist: optimum>=1.12.0
 Requires-Dist: safetensors
 Requires-Dist: scipy
 Requires-Dist: sentencepiece
 Requires-Dist: transformers[tokenizers,torch]>=4.36.0
 Provides-Extra: agents
 Requires-Dist: diffusers; extra == 'agents'
```

