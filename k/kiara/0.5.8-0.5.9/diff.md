# Comparing `tmp/kiara-0.5.8.tar.gz` & `tmp/kiara-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara-0.5.8.tar", last modified: Wed Dec 27 14:19:37 2023, max compression
+gzip compressed data, was "kiara-0.5.9.tar", last modified: Fri Dec 29 09:34:24 2023, max compression
```

## Comparing `kiara-0.5.8.tar` & `kiara-0.5.9.tar`

### file list

```diff
@@ -1,515 +1,515 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.311592 kiara-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-27 14:19:22.000000 kiara-0.5.8/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)      127 2023-12-27 14:19:22.000000 kiara-0.5.8/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-27 14:19:22.000000 kiara-0.5.8/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-27 14:19:22.000000 kiara-0.5.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.243592 kiara-0.5.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.243592 kiara-0.5.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2023-12-27 14:19:22.000000 kiara-0.5.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2023-12-27 14:19:22.000000 kiara-0.5.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      501 2023-12-27 14:19:22.000000 kiara-0.5.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.243592 kiara-0.5.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2023-12-27 14:19:22.000000 kiara-0.5.8/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9102 2023-12-27 14:19:22.000000 kiara-0.5.8/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-12-27 14:19:22.000000 kiara-0.5.8/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      831 2023-12-27 14:19:22.000000 kiara-0.5.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      934 2023-12-27 14:19:22.000000 kiara-0.5.8/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-12-27 14:19:22.000000 kiara-0.5.8/.kiara_complete.zsh
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2023-12-27 14:19:22.000000 kiara-0.5.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       77 2023-12-27 14:19:22.000000 kiara-0.5.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11182 2023-12-27 14:19:22.000000 kiara-0.5.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    16756 2023-12-27 14:19:22.000000 kiara-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      337 2023-12-27 14:19:22.000000 kiara-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2023-12-27 14:19:22.000000 kiara-0.5.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     9994 2023-12-27 14:19:37.311592 kiara-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2023-12-27 14:19:22.000000 kiara-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.223592 kiara-0.5.8/ci/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.243592 kiara-0.5.8/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2023-12-27 14:19:22.000000 kiara-0.5.8/ci/conda/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.243592 kiara-0.5.8/ci/conda/airium/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-27 14:19:22.000000 kiara-0.5.8/ci/conda/airium/conda-pkg-patch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.243592 kiara-0.5.8/ci/conda/bases/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-27 14:19:22.000000 kiara-0.5.8/ci/conda/bases/conda-pkg-patch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      537 2023-12-27 14:19:22.000000 kiara-0.5.8/ci/conda/conda-pkg-patch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.243592 kiara-0.5.8/ci/conda/dag-cbor/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-27 14:19:22.000000 kiara-0.5.8/ci/conda/dag-cbor/conda-pkg-patch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.243592 kiara-0.5.8/ci/conda/email-validator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:22.000000 kiara-0.5.8/ci/conda/email-validator/conda-pkg-patch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.243592 kiara-0.5.8/ci/conda/fasteners/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:22.000000 kiara-0.5.8/ci/conda/fasteners/conda-pkg-patch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.247592 kiara-0.5.8/ci/conda/jupyter-client/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-12-27 14:19:22.000000 kiara-0.5.8/ci/conda/jupyter-client/conda-pkg-patch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.247592 kiara-0.5.8/ci/conda/jupyter-core/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-27 14:19:22.000000 kiara-0.5.8/ci/conda/jupyter-core/conda-pkg-patch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.247592 kiara-0.5.8/ci/conda/makkus.bases/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-27 14:19:22.000000 kiara-0.5.8/ci/conda/makkus.bases/conda-pkg-patch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.247592 kiara-0.5.8/ci/conda/makkus.dag-cbor/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-27 14:19:22.000000 kiara-0.5.8/ci/conda/makkus.dag-cbor/conda-pkg-patch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.247592 kiara-0.5.8/ci/conda/makkus.multiformats/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-27 14:19:22.000000 kiara-0.5.8/ci/conda/makkus.multiformats/multiformats.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.247592 kiara-0.5.8/ci/conda/makkus.multiformats-config/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-27 14:19:22.000000 kiara-0.5.8/ci/conda/makkus.multiformats-config/multiformats-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.247592 kiara-0.5.8/ci/conda/mknotebooks/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-27 14:19:22.000000 kiara-0.5.8/ci/conda/mknotebooks/conda-pkg-patch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.247592 kiara-0.5.8/ci/conda/multiformats/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-12-27 14:19:22.000000 kiara-0.5.8/ci/conda/multiformats/multiformats.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.247592 kiara-0.5.8/ci/conda/multiformats-config/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-27 14:19:22.000000 kiara-0.5.8/ci/conda/multiformats-config/multiformats-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.247592 kiara-0.5.8/ci/conda/pp-ez/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:22.000000 kiara-0.5.8/ci/conda/pp-ez/conda-pkg-patch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.247592 kiara-0.5.8/ci/conda/puremagic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:22.000000 kiara-0.5.8/ci/conda/puremagic/conda-pkg-patch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.247592 kiara-0.5.8/ci/conda/pydantic-to-typescript/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:22.000000 kiara-0.5.8/ci/conda/pydantic-to-typescript/conda-pkg-patch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.247592 kiara-0.5.8/ci/conda/typing-validation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:22.000000 kiara-0.5.8/ci/conda/typing-validation/conda-pkg-patch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-12-27 14:19:22.000000 kiara-0.5.8/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.247592 kiara-0.5.8/dev/
--rw-r--r--   0 runner    (1001) docker     (127)   134752 2023-12-27 14:19:22.000000 kiara-0.5.8/dev/dev.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:22.000000 kiara-0.5.8/dev/network_analysis.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2023-12-27 14:19:22.000000 kiara-0.5.8/dev/script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.247592 kiara-0.5.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/SUMMARY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.247592 kiara-0.5.8/docs/design_docs/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/design_docs/SUMMARY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.251592 kiara-0.5.8/docs/design_docs/architecture/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/design_docs/architecture/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/design_docs/architecture/assumptions.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.251592 kiara-0.5.8/docs/design_docs/architecture/data/
--rw-r--r--   0 runner    (1001) docker     (127)      878 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/design_docs/architecture/data/data_centric_approach.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    67993 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/design_docs/architecture/data/data_formats.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      592 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/design_docs/architecture/data/dev.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6152 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/design_docs/architecture/data/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    20616 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/design_docs/architecture/data/persistence.md
--rw-r--r--   0 runner    (1001) docker     (127)   105120 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/design_docs/architecture/data/requirements.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    17509 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/design_docs/architecture/data/result_tree.png
--rw-r--r--   0 runner    (1001) docker     (127)     5724 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/design_docs/architecture/decisions.md
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/design_docs/architecture/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/design_docs/architecture/metadata.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.251592 kiara-0.5.8/docs/design_docs/architecture/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)    18476 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/design_docs/architecture/workflows/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.251592 kiara-0.5.8/docs/design_docs/architecture/workflows/modularity/
--rw-r--r--   0 runner    (1001) docker     (127)    63106 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/design_docs/architecture/workflows/modularity/modularity.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    53370 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/design_docs/architecture/workflows/modularity/modularity_2.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.251592 kiara-0.5.8/docs/design_docs/architecture/workflows/modularity/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/design_docs/architecture/workflows/modularity/workflows/corpus_processing.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      293 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/design_docs/architecture/workflows/modularity/workflows/corpus_processing_simple.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      597 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/design_docs/architecture/workflows/modularity/workflows/input_files_processing.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/design_docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.251592 kiara-0.5.8/docs/development/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/development/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (127)      776 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/development/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      900 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/development/install.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.251592 kiara-0.5.8/docs/development/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/development/modules/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/development/modules/render_value.md
--rw-r--r--   0 runner    (1001) docker     (127)      718 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/development/rendering.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.255592 kiara-0.5.8/docs/included_components/
--rw-r--r--   0 runner    (1001) docker     (127)      466 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/included_components/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.255592 kiara-0.5.8/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-27 14:19:22.000000 kiara-0.5.8/docs/stylesheets/extra.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.227592 kiara-0.5.8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.255592 kiara-0.5.8/examples/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:22.000000 kiara-0.5.8/examples/data/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.255592 kiara-0.5.8/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2023-12-27 14:19:22.000000 kiara-0.5.8/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (127)    33398 2023-12-27 14:19:22.000000 kiara-0.5.8/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-12-27 14:19:22.000000 kiara-0.5.8/examples/data/journals/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-12-27 14:19:22.000000 kiara-0.5.8/examples/data/journals/query.graphql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.255592 kiara-0.5.8/examples/data/text_corpus/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.255592 kiara-0.5.8/examples/data/text_corpus/La_Ragione/
--rw-r--r--   0 runner    (1001) docker     (127)    16613 2023-12-27 14:19:22.000000 kiara-0.5.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16679 2023-12-27 14:19:22.000000 kiara-0.5.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-2_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16793 2023-12-27 14:19:22.000000 kiara-0.5.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-3_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16235 2023-12-27 14:19:22.000000 kiara-0.5.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-4_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18346 2023-12-27 14:19:22.000000 kiara-0.5.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18474 2023-12-27 14:19:22.000000 kiara-0.5.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-2_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18280 2023-12-27 14:19:22.000000 kiara-0.5.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-3_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18481 2023-12-27 14:19:22.000000 kiara-0.5.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-4_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18620 2023-12-27 14:19:22.000000 kiara-0.5.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-16_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18698 2023-12-27 14:19:22.000000 kiara-0.5.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-16_ed-2_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18540 2023-12-27 14:19:22.000000 kiara-0.5.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-16_ed-3_seq-1_ocr.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.259592 kiara-0.5.8/examples/data/text_corpus/La_Rassegna/
--rw-r--r--   0 runner    (1001) docker     (127)    19397 2023-12-27 14:19:22.000000 kiara-0.5.8/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-07_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    20647 2023-12-27 14:19:22.000000 kiara-0.5.8/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-14_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    20650 2023-12-27 14:19:22.000000 kiara-0.5.8/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-14_ed-2_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21017 2023-12-27 14:19:22.000000 kiara-0.5.8/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-21_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    20982 2023-12-27 14:19:22.000000 kiara-0.5.8/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-21_ed-2_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-12-27 14:19:22.000000 kiara-0.5.8/examples/data/text_corpus/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.259592 kiara-0.5.8/examples/jupyter/
--rw-r--r--   0 runner    (1001) docker     (127)   256513 2023-12-27 14:19:22.000000 kiara-0.5.8/examples/jupyter/install_example.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.259592 kiara-0.5.8/examples/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2023-12-27 14:19:22.000000 kiara-0.5.8/examples/pipelines/mock_pipeline_1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.259592 kiara-0.5.8/examples/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-12-27 14:19:22.000000 kiara-0.5.8/examples/scripts/import_df.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2023-12-27 14:19:22.000000 kiara-0.5.8/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      251 2023-12-27 14:19:22.000000 kiara-0.5.8/onboarding.folder_to_table.json
--rw-r--r--   0 runner    (1001) docker     (127)    14311 2023-12-27 14:19:22.000000 kiara-0.5.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.227592 kiara-0.5.8/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.259592 kiara-0.5.8/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2023-12-27 14:19:22.000000 kiara-0.5.8/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2023-12-27 14:19:22.000000 kiara-0.5.8/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2023-12-27 14:19:22.000000 kiara-0.5.8/scripts/documentation/gen_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-27 14:19:37.311592 kiara-0.5.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.235592 kiara-0.5.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.259592 kiara-0.5.8/src/kiara/
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.259592 kiara-0.5.8/src/kiara/context/
--rw-r--r--   0 runner    (1001) docker     (127)    22449 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28345 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/context/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6414 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/context/orm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/context/runtime_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.259592 kiara-0.5.8/src/kiara/data_types/
--rw-r--r--   0 runner    (1001) docker     (127)    19178 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/data_types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.263592 kiara-0.5.8/src/kiara/data_types/included_core_types/
--rw-r--r--   0 runner    (1001) docker     (127)    17897 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/data_types/included_core_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10220 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/data_types/included_core_types/filesystem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.263592 kiara-0.5.8/src/kiara/data_types/included_core_types/internal/
--rw-r--r--   0 runner    (1001) docker     (127)     8444 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/data_types/included_core_types/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/data_types/included_core_types/internal/render_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/data_types/included_core_types/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/data_types/included_core_types/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8196 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.263592 kiara-0.5.8/src/kiara/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/doc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/doc/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/doc/generate_api_doc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/doc/mkdocs_macros_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6035 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/doc/mkdocs_macros_kiara.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.263592 kiara-0.5.8/src/kiara/doc/mkdocstrings/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/doc/mkdocstrings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/doc/mkdocstrings/collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/doc/mkdocstrings/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/doc/mkdocstrings/renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15721 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.263592 kiara-0.5.8/src/kiara/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)    10824 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.263592 kiara-0.5.8/src/kiara/interfaces/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.263592 kiara-0.5.8/src/kiara/interfaces/cli/context/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/cli/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16472 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/cli/context/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.263592 kiara-0.5.8/src/kiara/interfaces/cli/data/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/cli/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15186 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/cli/data/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.263592 kiara-0.5.8/src/kiara/interfaces/cli/info/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/cli/info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/cli/info/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.267592 kiara-0.5.8/src/kiara/interfaces/cli/module/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/cli/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/cli/module/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.267592 kiara-0.5.8/src/kiara/interfaces/cli/operation/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/cli/operation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/cli/operation/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.267592 kiara-0.5.8/src/kiara/interfaces/cli/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/cli/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10182 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/cli/pipeline/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/cli/proxy_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.267592 kiara-0.5.8/src/kiara/interfaces/cli/render/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/cli/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6662 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/cli/render/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     8237 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/cli/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.267592 kiara-0.5.8/src/kiara/interfaces/cli/type/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/cli/type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/cli/type/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.267592 kiara-0.5.8/src/kiara/interfaces/cli/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/cli/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/cli/workflow/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.267592 kiara-0.5.8/src/kiara/interfaces/python_api/
--rw-r--r--   0 runner    (1001) docker     (127)   100497 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/python_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5860 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/python_api/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.271592 kiara-0.5.8/src/kiara/interfaces/python_api/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/python_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/python_api/models/doc.py
--rw-r--r--   0 runner    (1001) docker     (127)    70434 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/python_api/models/info.py
--rw-r--r--   0 runner    (1001) docker     (127)    11238 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/python_api/models/job.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/python_api/models/workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    10325 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/python_api/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9810 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/python_api/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/python_api/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/python_api/value.py
--rw-r--r--   0 runner    (1001) docker     (127)    52348 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/interfaces/python_api/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.271592 kiara-0.5.8/src/kiara/models/
--rw-r--r--   0 runner    (1001) docker     (127)    12174 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.271592 kiara-0.5.8/src/kiara/models/aliases/
--rw-r--r--   0 runner    (1001) docker     (127)    13433 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/aliases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8016 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/archives.py
--rw-r--r--   0 runner    (1001) docker     (127)    10258 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8233 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/documentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.271592 kiara-0.5.8/src/kiara/models/events/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/events/alias_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/events/data_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/events/destiny_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/events/job_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     8184 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/events/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/events/workflow_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    19299 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/filesystem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.271592 kiara-0.5.8/src/kiara/models/module/
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/module/destiny.py
--rw-r--r--   0 runner    (1001) docker     (127)     9406 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/module/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6669 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/module/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    16327 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/module/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/module/persistence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.275592 kiara-0.5.8/src/kiara/models/module/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)    29161 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/module/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8662 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/module/pipeline/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    32647 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/module/pipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    10441 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/module/pipeline/stages.py
--rw-r--r--   0 runner    (1001) docker     (127)    30954 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/module/pipeline/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/module/pipeline/value_refs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/python_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.275592 kiara-0.5.8/src/kiara/models/rendering/
--rw-r--r--   0 runner    (1001) docker     (127)     4836 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/rendering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/rendering/values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.275592 kiara-0.5.8/src/kiara/models/runtime_environment/
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/runtime_environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/runtime_environment/kiara.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/runtime_environment/operating_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     5697 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/runtime_environment/python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.275592 kiara-0.5.8/src/kiara/models/values/
--rw-r--r--   0 runner    (1001) docker     (127)      895 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/values/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/values/data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    10669 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/values/lineage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/values/matchers.py
--rw-r--r--   0 runner    (1001) docker     (127)    55108 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/values/value.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.275592 kiara-0.5.8/src/kiara/models/values/value_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/values/value_metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.275592 kiara-0.5.8/src/kiara/models/values/value_metadata/included_metadata_types/
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/values/value_metadata/included_metadata_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/values/value_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    12771 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/models/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.275592 kiara-0.5.8/src/kiara/modules/
--rw-r--r--   0 runner    (1001) docker     (127)    20300 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.279592 kiara-0.5.8/src/kiara/modules/included_core_modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/modules/included_core_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/modules/included_core_modules/create_from.py
--rw-r--r--   0 runner    (1001) docker     (127)     6837 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/modules/included_core_modules/export_as.py
--rw-r--r--   0 runner    (1001) docker     (127)     9970 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/modules/included_core_modules/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     5268 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/modules/included_core_modules/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/modules/included_core_modules/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4220 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/modules/included_core_modules/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/modules/included_core_modules/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6360 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/modules/included_core_modules/pretty_print.py
--rw-r--r--   0 runner    (1001) docker     (127)     7996 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/modules/included_core_modules/render_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     8470 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/modules/included_core_modules/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.279592 kiara-0.5.8/src/kiara/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/operations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.279592 kiara-0.5.8/src/kiara/operations/included_core_operations/
--rw-r--r--   0 runner    (1001) docker     (127)     7001 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/operations/included_core_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7312 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/operations/included_core_operations/create_from.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/operations/included_core_operations/export_as.py
--rw-r--r--   0 runner    (1001) docker     (127)    16716 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/operations/included_core_operations/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7155 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/operations/included_core_operations/import_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/operations/included_core_operations/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/operations/included_core_operations/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     8900 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/operations/included_core_operations/pretty_print.py
--rw-r--r--   0 runner    (1001) docker     (127)     8458 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/operations/included_core_operations/render_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8899 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/operations/included_core_operations/render_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    10168 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/operations/included_core_operations/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.279592 kiara-0.5.8/src/kiara/processing/
--rw-r--r--   0 runner    (1001) docker     (127)    13652 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/processing/synchronous.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.279592 kiara-0.5.8/src/kiara/registries/
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/registries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.279592 kiara-0.5.8/src/kiara/registries/aliases/
--rw-r--r--   0 runner    (1001) docker     (127)    13096 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/registries/aliases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4835 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/registries/aliases/archives.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.283592 kiara-0.5.8/src/kiara/registries/data/
--rw-r--r--   0 runner    (1001) docker     (127)    39525 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/registries/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.283592 kiara-0.5.8/src/kiara/registries/data/data_store/
--rw-r--r--   0 runner    (1001) docker     (127)    17793 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/registries/data/data_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16968 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/registries/data/data_store/filesystem_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.283592 kiara-0.5.8/src/kiara/registries/destinies/
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/registries/destinies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6165 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/registries/destinies/filesystem_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    10243 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/registries/destinies/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.283592 kiara-0.5.8/src/kiara/registries/environment/
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/registries/environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.283592 kiara-0.5.8/src/kiara/registries/events/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/registries/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/registries/events/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/registries/events/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.283592 kiara-0.5.8/src/kiara/registries/ids/
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/registries/ids/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.283592 kiara-0.5.8/src/kiara/registries/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)    19254 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/registries/jobs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.283592 kiara-0.5.8/src/kiara/registries/jobs/job_store/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/registries/jobs/job_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6819 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/registries/jobs/job_store/filesystem_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.283592 kiara-0.5.8/src/kiara/registries/models/
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/registries/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.283592 kiara-0.5.8/src/kiara/registries/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/registries/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.283592 kiara-0.5.8/src/kiara/registries/operations/
--rw-r--r--   0 runner    (1001) docker     (127)    24894 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/registries/operations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.283592 kiara-0.5.8/src/kiara/registries/rendering/
--rw-r--r--   0 runner    (1001) docker     (127)    13328 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/registries/rendering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.283592 kiara-0.5.8/src/kiara/registries/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     6261 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/registries/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.283592 kiara-0.5.8/src/kiara/registries/types/
--rw-r--r--   0 runner    (1001) docker     (127)    10465 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/registries/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.283592 kiara-0.5.8/src/kiara/registries/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)    17272 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/registries/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7073 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/registries/workflows/archives.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.283592 kiara-0.5.8/src/kiara/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)     6953 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/renderers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.287592 kiara-0.5.8/src/kiara/renderers/included_renderers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/renderers/included_renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/renderers/included_renderers/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12237 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/renderers/included_renderers/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/renderers/included_renderers/value.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/renderers/jinja.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.287592 kiara-0.5.8/src/kiara/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.235592 kiara-0.5.8/src/kiara/resources/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.287592 kiara-0.5.8/src/kiara/resources/templates/doc_gen/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/resources/templates/doc_gen/info_listing.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.235592 kiara-0.5.8/src/kiara/resources/templates/render/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.287592 kiara-0.5.8/src/kiara/resources/templates/render/kiara_api/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/resources/templates/render/kiara_api/api_doc.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.287592 kiara-0.5.8/src/kiara/resources/templates/render/models/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/resources/templates/render/models/generic_model_info.html
--rw-r--r--   0 runner    (1001) docker     (127)      458 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/resources/templates/render/models/info.operation.html
--rw-r--r--   0 runner    (1001) docker     (127)      346 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/resources/templates/render/models/info.value.html
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/resources/templates/render/models/macros.html
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/resources/templates/render/models/metadata.authors.html
--rw-r--r--   0 runner    (1001) docker     (127)      649 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/resources/templates/render/models/metadata.context.html
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/resources/templates/render/models/metadata.documentation.html
--rw-r--r--   0 runner    (1001) docker     (127)      359 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/resources/templates/render/models/model_data.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.287592 kiara-0.5.8/src/kiara/resources/templates/render/pipeline/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.287592 kiara-0.5.8/src/kiara/resources/templates/render/pipeline/markdown/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/resources/templates/render/pipeline/markdown/pipeline.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/resources/templates/render/pipeline/pipeline_info.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/resources/templates/render/pipeline/python_script.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.287592 kiara-0.5.8/src/kiara/resources/templates/render/pipeline/static_page/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/resources/templates/render/pipeline/static_page/page.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/resources/templates/render/pipeline/static_page/step.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.287592 kiara-0.5.8/src/kiara/resources/tui/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/resources/tui/pager_app.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.295592 kiara-0.5.8/src/kiara/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25554 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/class_loading.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.295592 kiara-0.5.8/src/kiara/utils/cli/
--rw-r--r--   0 runner    (1001) docker     (127)    12544 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16498 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/cli/rich_click.py
--rw-r--r--   0 runner    (1001) docker     (127)    13553 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     8167 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.295592 kiara-0.5.8/src/kiara/utils/develop/
--rw-r--r--   0 runner    (1001) docker     (127)     7856 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/develop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/doc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/downloads.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/global_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.295592 kiara-0.5.8/src/kiara/utils/hashfs/
--rw-r--r--   0 runner    (1001) docker     (127)    16790 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/hashfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/html.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     9491 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)    30147 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    11262 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/reflection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/rendering.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/string_vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.295592 kiara-0.5.8/src/kiara/utils/testing/
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6206 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/values.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/windows.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.295592 kiara-0.5.8/src/kiara/zmq/
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/zmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/zmq/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.295592 kiara-0.5.8/src/kiara/zmq/messages/
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/zmq/messages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.295592 kiara-0.5.8/src/kiara/zmq/service/
--rw-r--r--   0 runner    (1001) docker     (127)     8250 2023-12-27 14:19:22.000000 kiara-0.5.8/src/kiara/zmq/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.303592 kiara-0.5.8/src/kiara.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9994 2023-12-27 14:19:37.000000 kiara-0.5.8/src/kiara.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15457 2023-12-27 14:19:37.000000 kiara-0.5.8/src/kiara.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 14:19:37.000000 kiara-0.5.8/src/kiara.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5695 2023-12-27 14:19:37.000000 kiara-0.5.8/src/kiara.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-12-27 14:19:37.000000 kiara-0.5.8/src/kiara.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-27 14:19:37.000000 kiara-0.5.8/src/kiara.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.239592 kiara-0.5.8/src/mkdocstrings_handlers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.295592 kiara-0.5.8/src/mkdocstrings_handlers/kiara/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2023-12-27 14:19:22.000000 kiara-0.5.8/src/mkdocstrings_handlers/kiara/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.239592 kiara-0.5.8/src/mkdocstrings_handlers/kiara/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.295592 kiara-0.5.8/src/mkdocstrings_handlers/kiara/templates/material/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:22.000000 kiara-0.5.8/src/mkdocstrings_handlers/kiara/templates/material/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.295592 kiara-0.5.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.239592 kiara-0.5.8/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.299592 kiara-0.5.8/tests/resources/invalid_pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/resources/invalid_pipelines/logic_4.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.299592 kiara-0.5.8/tests/resources/module_configs/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/resources/module_configs/and.json
--rw-r--r--   0 runner    (1001) docker     (127)      229 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/resources/module_configs/and_wrapped.json
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/resources/module_configs/table_load.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.299592 kiara-0.5.8/tests/resources/pipelines/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.299592 kiara-0.5.8/tests/resources/pipelines/dummy/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/resources/pipelines/dummy/dummy_1.json
--rw-r--r--   0 runner    (1001) docker     (127)      506 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/resources/pipelines/dummy/dummy_1_delay.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.299592 kiara-0.5.8/tests/resources/pipelines/logic/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/resources/pipelines/logic/logic_1.json
--rw-r--r--   0 runner    (1001) docker     (127)      419 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/resources/pipelines/logic/logic_2.json
--rw-r--r--   0 runner    (1001) docker     (127)      383 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/resources/pipelines/logic/logic_3.json
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/resources/pipelines/logic/logic_4.json
--rw-r--r--   0 runner    (1001) docker     (127)      308 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/resources/pipelines/table_import.json
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/resources/pipelines/test_preseed_1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.299592 kiara-0.5.8/tests/test_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_api/test_data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_api/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_api/test_module_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_api/test_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.303592 kiara-0.5.8/tests/test_cli/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_cli/test_context_subcommands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_cli/test_data_subcommands.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_cli/test_metadata_subcommands.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_cli/test_misc_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_cli/test_module_subcommands.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_cli/test_operation_subcommands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_cli/test_pipeline_subcommands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_cli/test_run_subcommand.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.303592 kiara-0.5.8/tests/test_included_data_types/
--rw-r--r--   0 runner    (1001) docker     (127)      702 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_included_data_types/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_kiara_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_module_instances.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_module_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.303592 kiara-0.5.8/tests/test_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_modules/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_modules/test_simple_module_exec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.303592 kiara-0.5.8/tests/test_operation_types/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_operation_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_operation_types/test_extract_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_operation_types/test_persist_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_operation_types/test_render_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_pipeline_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.303592 kiara-0.5.8/tests/test_pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_pipelines/test_pipeline_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_pipelines/test_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_rendering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:19:37.303592 kiara-0.5.8/tests/test_values/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_values/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/test_values/test_values.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2023-12-27 14:19:22.000000 kiara-0.5.8/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.255943 kiara-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-29 09:34:13.000000 kiara-0.5.9/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2023-12-29 09:34:13.000000 kiara-0.5.9/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-29 09:34:13.000000 kiara-0.5.9/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-29 09:34:13.000000 kiara-0.5.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.187944 kiara-0.5.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.187944 kiara-0.5.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2023-12-29 09:34:13.000000 kiara-0.5.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2023-12-29 09:34:13.000000 kiara-0.5.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2023-12-29 09:34:13.000000 kiara-0.5.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.187944 kiara-0.5.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2023-12-29 09:34:13.000000 kiara-0.5.9/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9572 2023-12-29 09:34:13.000000 kiara-0.5.9/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-12-29 09:34:13.000000 kiara-0.5.9/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2023-12-29 09:34:13.000000 kiara-0.5.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2023-12-29 09:34:13.000000 kiara-0.5.9/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2023-12-29 09:34:13.000000 kiara-0.5.9/.kiara_complete.zsh
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2023-12-29 09:34:13.000000 kiara-0.5.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2023-12-29 09:34:13.000000 kiara-0.5.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11182 2023-12-29 09:34:13.000000 kiara-0.5.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16756 2023-12-29 09:34:13.000000 kiara-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2023-12-29 09:34:13.000000 kiara-0.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2023-12-29 09:34:13.000000 kiara-0.5.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     9995 2023-12-29 09:34:24.251943 kiara-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2023-12-29 09:34:13.000000 kiara-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.167943 kiara-0.5.9/ci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.187944 kiara-0.5.9/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2023-12-29 09:34:13.000000 kiara-0.5.9/ci/conda/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.187944 kiara-0.5.9/ci/conda/airium/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-29 09:34:13.000000 kiara-0.5.9/ci/conda/airium/conda-pkg-patch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.187944 kiara-0.5.9/ci/conda/bases/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-29 09:34:13.000000 kiara-0.5.9/ci/conda/bases/conda-pkg-patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2023-12-29 09:34:13.000000 kiara-0.5.9/ci/conda/conda-pkg-patch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.187944 kiara-0.5.9/ci/conda/dag-cbor/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-29 09:34:13.000000 kiara-0.5.9/ci/conda/dag-cbor/conda-pkg-patch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.187944 kiara-0.5.9/ci/conda/email-validator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:13.000000 kiara-0.5.9/ci/conda/email-validator/conda-pkg-patch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.187944 kiara-0.5.9/ci/conda/fasteners/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:13.000000 kiara-0.5.9/ci/conda/fasteners/conda-pkg-patch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.187944 kiara-0.5.9/ci/conda/jupyter-client/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2023-12-29 09:34:13.000000 kiara-0.5.9/ci/conda/jupyter-client/conda-pkg-patch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.187944 kiara-0.5.9/ci/conda/jupyter-core/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-29 09:34:13.000000 kiara-0.5.9/ci/conda/jupyter-core/conda-pkg-patch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.187944 kiara-0.5.9/ci/conda/makkus.bases/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-29 09:34:13.000000 kiara-0.5.9/ci/conda/makkus.bases/conda-pkg-patch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.187944 kiara-0.5.9/ci/conda/makkus.dag-cbor/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-29 09:34:13.000000 kiara-0.5.9/ci/conda/makkus.dag-cbor/conda-pkg-patch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.187944 kiara-0.5.9/ci/conda/makkus.multiformats/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-29 09:34:13.000000 kiara-0.5.9/ci/conda/makkus.multiformats/multiformats.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.187944 kiara-0.5.9/ci/conda/makkus.multiformats-config/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-29 09:34:13.000000 kiara-0.5.9/ci/conda/makkus.multiformats-config/multiformats-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.187944 kiara-0.5.9/ci/conda/mknotebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-29 09:34:13.000000 kiara-0.5.9/ci/conda/mknotebooks/conda-pkg-patch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.187944 kiara-0.5.9/ci/conda/multiformats/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2023-12-29 09:34:13.000000 kiara-0.5.9/ci/conda/multiformats/multiformats.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.187944 kiara-0.5.9/ci/conda/multiformats-config/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-29 09:34:13.000000 kiara-0.5.9/ci/conda/multiformats-config/multiformats-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.187944 kiara-0.5.9/ci/conda/pp-ez/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:13.000000 kiara-0.5.9/ci/conda/pp-ez/conda-pkg-patch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.191944 kiara-0.5.9/ci/conda/puremagic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:13.000000 kiara-0.5.9/ci/conda/puremagic/conda-pkg-patch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.191944 kiara-0.5.9/ci/conda/pydantic-to-typescript/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:13.000000 kiara-0.5.9/ci/conda/pydantic-to-typescript/conda-pkg-patch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.191944 kiara-0.5.9/ci/conda/typing-validation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:13.000000 kiara-0.5.9/ci/conda/typing-validation/conda-pkg-patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2023-12-29 09:34:13.000000 kiara-0.5.9/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.191944 kiara-0.5.9/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)   134752 2023-12-29 09:34:13.000000 kiara-0.5.9/dev/dev.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:13.000000 kiara-0.5.9/dev/network_analysis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2023-12-29 09:34:13.000000 kiara-0.5.9/dev/script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.191944 kiara-0.5.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/SUMMARY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.191944 kiara-0.5.9/docs/design_docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/design_docs/SUMMARY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.191944 kiara-0.5.9/docs/design_docs/architecture/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/design_docs/architecture/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/design_docs/architecture/assumptions.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.191944 kiara-0.5.9/docs/design_docs/architecture/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/design_docs/architecture/data/data_centric_approach.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    67993 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/design_docs/architecture/data/data_formats.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/design_docs/architecture/data/dev.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6152 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/design_docs/architecture/data/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    20616 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/design_docs/architecture/data/persistence.md
+-rw-r--r--   0 runner    (1001) docker     (127)   105120 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/design_docs/architecture/data/requirements.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    17509 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/design_docs/architecture/data/result_tree.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/design_docs/architecture/decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/design_docs/architecture/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/design_docs/architecture/metadata.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.191944 kiara-0.5.9/docs/design_docs/architecture/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)    18476 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/design_docs/architecture/workflows/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.195943 kiara-0.5.9/docs/design_docs/architecture/workflows/modularity/
+-rw-r--r--   0 runner    (1001) docker     (127)    63106 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/design_docs/architecture/workflows/modularity/modularity.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    53370 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/design_docs/architecture/workflows/modularity/modularity_2.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.195943 kiara-0.5.9/docs/design_docs/architecture/workflows/modularity/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/design_docs/architecture/workflows/modularity/workflows/corpus_processing.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/design_docs/architecture/workflows/modularity/workflows/corpus_processing_simple.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/design_docs/architecture/workflows/modularity/workflows/input_files_processing.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/design_docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.195943 kiara-0.5.9/docs/development/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/development/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/development/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/development/install.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.195943 kiara-0.5.9/docs/development/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/development/modules/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/development/modules/render_value.md
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/development/rendering.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.195943 kiara-0.5.9/docs/included_components/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/included_components/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.195943 kiara-0.5.9/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-29 09:34:13.000000 kiara-0.5.9/docs/stylesheets/extra.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.171944 kiara-0.5.9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.195943 kiara-0.5.9/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:13.000000 kiara-0.5.9/examples/data/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.195943 kiara-0.5.9/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2023-12-29 09:34:13.000000 kiara-0.5.9/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    33398 2023-12-29 09:34:13.000000 kiara-0.5.9/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2023-12-29 09:34:13.000000 kiara-0.5.9/examples/data/journals/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2023-12-29 09:34:13.000000 kiara-0.5.9/examples/data/journals/query.graphql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.195943 kiara-0.5.9/examples/data/text_corpus/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.199943 kiara-0.5.9/examples/data/text_corpus/La_Ragione/
+-rw-r--r--   0 runner    (1001) docker     (127)    16613 2023-12-29 09:34:13.000000 kiara-0.5.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16679 2023-12-29 09:34:13.000000 kiara-0.5.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-2_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16793 2023-12-29 09:34:13.000000 kiara-0.5.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-3_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16235 2023-12-29 09:34:13.000000 kiara-0.5.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-4_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18346 2023-12-29 09:34:13.000000 kiara-0.5.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18474 2023-12-29 09:34:13.000000 kiara-0.5.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-2_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18280 2023-12-29 09:34:13.000000 kiara-0.5.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-3_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18481 2023-12-29 09:34:13.000000 kiara-0.5.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-4_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18620 2023-12-29 09:34:13.000000 kiara-0.5.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-16_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18698 2023-12-29 09:34:13.000000 kiara-0.5.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-16_ed-2_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18540 2023-12-29 09:34:13.000000 kiara-0.5.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-16_ed-3_seq-1_ocr.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.199943 kiara-0.5.9/examples/data/text_corpus/La_Rassegna/
+-rw-r--r--   0 runner    (1001) docker     (127)    19397 2023-12-29 09:34:13.000000 kiara-0.5.9/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-07_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    20647 2023-12-29 09:34:13.000000 kiara-0.5.9/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-14_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    20650 2023-12-29 09:34:13.000000 kiara-0.5.9/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-14_ed-2_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21017 2023-12-29 09:34:13.000000 kiara-0.5.9/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-21_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    20982 2023-12-29 09:34:13.000000 kiara-0.5.9/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-21_ed-2_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2023-12-29 09:34:13.000000 kiara-0.5.9/examples/data/text_corpus/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.199943 kiara-0.5.9/examples/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (127)   256513 2023-12-29 09:34:13.000000 kiara-0.5.9/examples/jupyter/install_example.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.199943 kiara-0.5.9/examples/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2023-12-29 09:34:13.000000 kiara-0.5.9/examples/pipelines/mock_pipeline_1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.199943 kiara-0.5.9/examples/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2023-12-29 09:34:13.000000 kiara-0.5.9/examples/scripts/import_df.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2023-12-29 09:34:13.000000 kiara-0.5.9/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2023-12-29 09:34:13.000000 kiara-0.5.9/onboarding.folder_to_table.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14312 2023-12-29 09:34:13.000000 kiara-0.5.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.171944 kiara-0.5.9/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.199943 kiara-0.5.9/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2023-12-29 09:34:13.000000 kiara-0.5.9/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2023-12-29 09:34:13.000000 kiara-0.5.9/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2023-12-29 09:34:13.000000 kiara-0.5.9/scripts/documentation/gen_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-29 09:34:24.255943 kiara-0.5.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.179943 kiara-0.5.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.203943 kiara-0.5.9/src/kiara/
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.203943 kiara-0.5.9/src/kiara/context/
+-rw-r--r--   0 runner    (1001) docker     (127)    22449 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28345 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/context/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6414 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/context/orm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/context/runtime_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.203943 kiara-0.5.9/src/kiara/data_types/
+-rw-r--r--   0 runner    (1001) docker     (127)    19178 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/data_types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.203943 kiara-0.5.9/src/kiara/data_types/included_core_types/
+-rw-r--r--   0 runner    (1001) docker     (127)    17897 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/data_types/included_core_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10220 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/data_types/included_core_types/filesystem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.203943 kiara-0.5.9/src/kiara/data_types/included_core_types/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)     8444 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/data_types/included_core_types/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/data_types/included_core_types/internal/render_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/data_types/included_core_types/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/data_types/included_core_types/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8196 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.203943 kiara-0.5.9/src/kiara/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/doc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/doc/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/doc/generate_api_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/doc/mkdocs_macros_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6035 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/doc/mkdocs_macros_kiara.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.207944 kiara-0.5.9/src/kiara/doc/mkdocstrings/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/doc/mkdocstrings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/doc/mkdocstrings/collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/doc/mkdocstrings/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/doc/mkdocstrings/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15721 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.207944 kiara-0.5.9/src/kiara/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)    10824 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.207944 kiara-0.5.9/src/kiara/interfaces/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.207944 kiara-0.5.9/src/kiara/interfaces/cli/context/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/cli/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16472 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/cli/context/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.207944 kiara-0.5.9/src/kiara/interfaces/cli/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/cli/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15186 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/cli/data/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.207944 kiara-0.5.9/src/kiara/interfaces/cli/info/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/cli/info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/cli/info/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.207944 kiara-0.5.9/src/kiara/interfaces/cli/module/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/cli/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/cli/module/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.207944 kiara-0.5.9/src/kiara/interfaces/cli/operation/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/cli/operation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/cli/operation/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.207944 kiara-0.5.9/src/kiara/interfaces/cli/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/cli/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10182 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/cli/pipeline/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/cli/proxy_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.207944 kiara-0.5.9/src/kiara/interfaces/cli/render/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/cli/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/cli/render/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8237 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/cli/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.207944 kiara-0.5.9/src/kiara/interfaces/cli/type/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/cli/type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/cli/type/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.207944 kiara-0.5.9/src/kiara/interfaces/cli/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/cli/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/cli/workflow/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.211943 kiara-0.5.9/src/kiara/interfaces/python_api/
+-rw-r--r--   0 runner    (1001) docker     (127)   100615 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/python_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5860 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/python_api/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.211943 kiara-0.5.9/src/kiara/interfaces/python_api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/python_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/python_api/models/doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70434 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/python_api/models/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11239 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/python_api/models/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/python_api/models/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10325 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/python_api/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9810 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/python_api/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/python_api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/python_api/value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52348 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/interfaces/python_api/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.211943 kiara-0.5.9/src/kiara/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    12174 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.211943 kiara-0.5.9/src/kiara/models/aliases/
+-rw-r--r--   0 runner    (1001) docker     (127)    13433 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/aliases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8016 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/archives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10258 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8233 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/documentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.215943 kiara-0.5.9/src/kiara/models/events/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/events/alias_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/events/data_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/events/destiny_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/events/job_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/events/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/events/workflow_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19299 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/filesystem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.215943 kiara-0.5.9/src/kiara/models/module/
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/module/destiny.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9406 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/module/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/module/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16327 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/module/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/module/persistence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.215943 kiara-0.5.9/src/kiara/models/module/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)    29161 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/module/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8662 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/module/pipeline/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32647 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/module/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10441 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/module/pipeline/stages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30954 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/module/pipeline/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/module/pipeline/value_refs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/python_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.215943 kiara-0.5.9/src/kiara/models/rendering/
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/rendering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/rendering/values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.215943 kiara-0.5.9/src/kiara/models/runtime_environment/
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/runtime_environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/runtime_environment/kiara.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/runtime_environment/operating_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5697 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/runtime_environment/python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.219943 kiara-0.5.9/src/kiara/models/values/
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/values/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/values/data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10669 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/values/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/values/matchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55108 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/values/value.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.219943 kiara-0.5.9/src/kiara/models/values/value_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/values/value_metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.219943 kiara-0.5.9/src/kiara/models/values/value_metadata/included_metadata_types/
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/values/value_metadata/included_metadata_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/values/value_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12771 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/models/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.219943 kiara-0.5.9/src/kiara/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)    20300 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.219943 kiara-0.5.9/src/kiara/modules/included_core_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/modules/included_core_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/modules/included_core_modules/create_from.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6837 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/modules/included_core_modules/export_as.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9970 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/modules/included_core_modules/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5268 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/modules/included_core_modules/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/modules/included_core_modules/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4220 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/modules/included_core_modules/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/modules/included_core_modules/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/modules/included_core_modules/pretty_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7996 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/modules/included_core_modules/render_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8470 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/modules/included_core_modules/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.219943 kiara-0.5.9/src/kiara/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/operations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.223944 kiara-0.5.9/src/kiara/operations/included_core_operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     7001 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/operations/included_core_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7312 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/operations/included_core_operations/create_from.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/operations/included_core_operations/export_as.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16716 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/operations/included_core_operations/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7155 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/operations/included_core_operations/import_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6327 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/operations/included_core_operations/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/operations/included_core_operations/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8900 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/operations/included_core_operations/pretty_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8458 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/operations/included_core_operations/render_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8899 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/operations/included_core_operations/render_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10168 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/operations/included_core_operations/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.223944 kiara-0.5.9/src/kiara/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)    13652 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/processing/synchronous.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.223944 kiara-0.5.9/src/kiara/registries/
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/registries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.223944 kiara-0.5.9/src/kiara/registries/aliases/
+-rw-r--r--   0 runner    (1001) docker     (127)    13096 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/registries/aliases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4835 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/registries/aliases/archives.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.223944 kiara-0.5.9/src/kiara/registries/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    39898 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/registries/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.223944 kiara-0.5.9/src/kiara/registries/data/data_store/
+-rw-r--r--   0 runner    (1001) docker     (127)    17793 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/registries/data/data_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16968 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/registries/data/data_store/filesystem_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.223944 kiara-0.5.9/src/kiara/registries/destinies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/registries/destinies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6165 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/registries/destinies/filesystem_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10243 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/registries/destinies/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.223944 kiara-0.5.9/src/kiara/registries/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/registries/environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.223944 kiara-0.5.9/src/kiara/registries/events/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/registries/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/registries/events/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/registries/events/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.223944 kiara-0.5.9/src/kiara/registries/ids/
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/registries/ids/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.223944 kiara-0.5.9/src/kiara/registries/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)    19254 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/registries/jobs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.227944 kiara-0.5.9/src/kiara/registries/jobs/job_store/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/registries/jobs/job_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6819 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/registries/jobs/job_store/filesystem_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.227944 kiara-0.5.9/src/kiara/registries/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/registries/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.227944 kiara-0.5.9/src/kiara/registries/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/registries/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.227944 kiara-0.5.9/src/kiara/registries/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)    24894 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/registries/operations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.227944 kiara-0.5.9/src/kiara/registries/rendering/
+-rw-r--r--   0 runner    (1001) docker     (127)    13328 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/registries/rendering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.227944 kiara-0.5.9/src/kiara/registries/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     6261 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/registries/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.227944 kiara-0.5.9/src/kiara/registries/types/
+-rw-r--r--   0 runner    (1001) docker     (127)    10465 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/registries/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.227944 kiara-0.5.9/src/kiara/registries/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)    17272 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/registries/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7073 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/registries/workflows/archives.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.227944 kiara-0.5.9/src/kiara/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/renderers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.227944 kiara-0.5.9/src/kiara/renderers/included_renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/renderers/included_renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/renderers/included_renderers/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12237 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/renderers/included_renderers/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/renderers/included_renderers/value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/renderers/jinja.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.227944 kiara-0.5.9/src/kiara/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.179943 kiara-0.5.9/src/kiara/resources/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.227944 kiara-0.5.9/src/kiara/resources/templates/doc_gen/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/resources/templates/doc_gen/info_listing.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.179943 kiara-0.5.9/src/kiara/resources/templates/render/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.227944 kiara-0.5.9/src/kiara/resources/templates/render/kiara_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/resources/templates/render/kiara_api/api_doc.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.231943 kiara-0.5.9/src/kiara/resources/templates/render/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/resources/templates/render/models/generic_model_info.html
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/resources/templates/render/models/info.operation.html
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/resources/templates/render/models/info.value.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/resources/templates/render/models/macros.html
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/resources/templates/render/models/metadata.authors.html
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/resources/templates/render/models/metadata.context.html
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/resources/templates/render/models/metadata.documentation.html
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/resources/templates/render/models/model_data.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.231943 kiara-0.5.9/src/kiara/resources/templates/render/pipeline/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.231943 kiara-0.5.9/src/kiara/resources/templates/render/pipeline/markdown/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/resources/templates/render/pipeline/markdown/pipeline.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/resources/templates/render/pipeline/pipeline_info.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/resources/templates/render/pipeline/python_script.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.231943 kiara-0.5.9/src/kiara/resources/templates/render/pipeline/static_page/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/resources/templates/render/pipeline/static_page/page.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/resources/templates/render/pipeline/static_page/step.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.231943 kiara-0.5.9/src/kiara/resources/tui/
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/resources/tui/pager_app.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.235943 kiara-0.5.9/src/kiara/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25554 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/class_loading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.235943 kiara-0.5.9/src/kiara/utils/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    12544 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16498 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/cli/rich_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13553 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8167 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.235943 kiara-0.5.9/src/kiara/utils/develop/
+-rw-r--r--   0 runner    (1001) docker     (127)     7856 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/develop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/global_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.235943 kiara-0.5.9/src/kiara/utils/hashfs/
+-rw-r--r--   0 runner    (1001) docker     (127)    16790 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/hashfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9491 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30147 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11262 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/reflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/rendering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/string_vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.235943 kiara-0.5.9/src/kiara/utils/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.235943 kiara-0.5.9/src/kiara/zmq/
+-rw-r--r--   0 runner    (1001) docker     (127)     6194 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/zmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/zmq/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.235943 kiara-0.5.9/src/kiara/zmq/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/zmq/messages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.235943 kiara-0.5.9/src/kiara/zmq/service/
+-rw-r--r--   0 runner    (1001) docker     (127)     8250 2023-12-29 09:34:13.000000 kiara-0.5.9/src/kiara/zmq/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.243944 kiara-0.5.9/src/kiara.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9995 2023-12-29 09:34:24.000000 kiara-0.5.9/src/kiara.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15457 2023-12-29 09:34:24.000000 kiara-0.5.9/src/kiara.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-29 09:34:24.000000 kiara-0.5.9/src/kiara.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5695 2023-12-29 09:34:24.000000 kiara-0.5.9/src/kiara.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2023-12-29 09:34:24.000000 kiara-0.5.9/src/kiara.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-29 09:34:24.000000 kiara-0.5.9/src/kiara.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.179943 kiara-0.5.9/src/mkdocstrings_handlers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.235943 kiara-0.5.9/src/mkdocstrings_handlers/kiara/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2023-12-29 09:34:13.000000 kiara-0.5.9/src/mkdocstrings_handlers/kiara/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.179943 kiara-0.5.9/src/mkdocstrings_handlers/kiara/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.235943 kiara-0.5.9/src/mkdocstrings_handlers/kiara/templates/material/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:13.000000 kiara-0.5.9/src/mkdocstrings_handlers/kiara/templates/material/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.239943 kiara-0.5.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.183943 kiara-0.5.9/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.239943 kiara-0.5.9/tests/resources/invalid_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/resources/invalid_pipelines/logic_4.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.239943 kiara-0.5.9/tests/resources/module_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/resources/module_configs/and.json
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/resources/module_configs/and_wrapped.json
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/resources/module_configs/table_load.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.239943 kiara-0.5.9/tests/resources/pipelines/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.239943 kiara-0.5.9/tests/resources/pipelines/dummy/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/resources/pipelines/dummy/dummy_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/resources/pipelines/dummy/dummy_1_delay.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.239943 kiara-0.5.9/tests/resources/pipelines/logic/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/resources/pipelines/logic/logic_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/resources/pipelines/logic/logic_2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/resources/pipelines/logic/logic_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/resources/pipelines/logic/logic_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/resources/pipelines/table_import.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/resources/pipelines/test_preseed_1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.239943 kiara-0.5.9/tests/test_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_api/test_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_api/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_api/test_module_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_api/test_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.243944 kiara-0.5.9/tests/test_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_cli/test_context_subcommands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_cli/test_data_subcommands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_cli/test_metadata_subcommands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_cli/test_misc_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_cli/test_module_subcommands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_cli/test_operation_subcommands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_cli/test_pipeline_subcommands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_cli/test_run_subcommand.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.243944 kiara-0.5.9/tests/test_included_data_types/
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_included_data_types/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_kiara_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_module_instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_module_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.243944 kiara-0.5.9/tests/test_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_modules/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_modules/test_simple_module_exec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.243944 kiara-0.5.9/tests/test_operation_types/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_operation_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_operation_types/test_extract_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_operation_types/test_persist_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_operation_types/test_render_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_pipeline_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.243944 kiara-0.5.9/tests/test_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_pipelines/test_pipeline_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_pipelines/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_rendering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 09:34:24.243944 kiara-0.5.9/tests/test_values/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_values/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/test_values/test_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2023-12-29 09:34:13.000000 kiara-0.5.9/tests/utils.py
```

### Comparing `kiara-0.5.8/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara-0.5.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/.github/ISSUE_TEMPLATE/feature_request.md` & `kiara-0.5.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/.github/workflows/build-darwin.yaml` & `kiara-0.5.9/.github/workflows/build-darwin.yaml`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/.github/workflows/build-linux.yaml` & `kiara-0.5.9/.github/workflows/build-linux.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -36,46 +36,60 @@
       - name: install tabular types plugin
         run: pip install -U git+https://github.com/DHARPA-project/kiara_plugin.tabular@develop
       - name: install kiara
         run: pip install -U  .[dev_testing]
       - name: display installed kiara and module package versions
         run: pip list | grep kiara
       - name: test with pytest
-        run: make test
+        run: pytest --cov-report=xml --cov=kiara tests
+      - name: Coveralls
+        uses: coverallsapp/github-action@v2
+        with:
+          parallel: true
+          flag-name: run ${{ join(matrix.*, ' - ') }}
+          format: cobertura
+          file: coverage.xml
 
   coverage:
     name: test coverage
     runs-on: ubuntu-latest
+    needs:
+      - test-linux
     steps:
-      - name: "Set up Python 3.10"
-        uses: actions/setup-python@v4
-        with:
-          python-version: "3.10"
-      - name: pip cache
-        id: pip-cache
-        uses: actions/cache@v3
-        with:
-          path: ~/.cache/pip
-          key: ${{ runner.os }}-pip-${{ hashFiles('**/setup.*') }}
-      - uses: actions/checkout@v2
-      - name: install core_types plugin
-        run: pip install -U git+https://github.com/DHARPA-project/kiara_plugin.core_types@develop
-      - name: install tabular types plugin
-        run: pip install -U git+https://github.com/DHARPA-project/kiara_plugin.tabular@develop
-      - name: install kiara
-        run: pip install -U  .[dev_testing]
-      - name: display installed kiara and module package versions
-        run: pip list | grep kiara
-      - name: Run coverage
-        run: coverage run -m pytest tests
-      - name: coveralls
+      - name: Coveralls Finished
         uses: coverallsapp/github-action@v2
         with:
-          format: python
-          allow-empty: true
+          parallel-finished: true
+#          carryforward: "run-1,run-2"
+#      - name: "Set up Python 3.10"
+#        uses: actions/setup-python@v4
+#        with:
+#          python-version: "3.10"
+#      - name: pip cache
+#        id: pip-cache
+#        uses: actions/cache@v3
+#        with:
+#          path: ~/.cache/pip
+#          key: ${{ runner.os }}-pip-${{ hashFiles('**/setup.*') }}
+#      - uses: actions/checkout@v2
+#      - name: install core_types plugin
+#        run: pip install -U git+https://github.com/DHARPA-project/kiara_plugin.core_types@develop
+#      - name: install tabular types plugin
+#        run: pip install -U git+https://github.com/DHARPA-project/kiara_plugin.tabular@develop
+#      - name: install kiara
+#        run: pip install -U  .[dev_testing]
+#      - name: display installed kiara and module package versions
+#        run: pip list | grep kiara
+#      - name: Run coverage
+#        run: coverage run -m pytest tests
+#      - name: coveralls
+#        uses: coverallsapp/github-action@v2
+#        with:
+#          format: python
+#          allow-empty: true
 #      - name: Upload coverage data to coveralls.io
 #        run: coveralls --service=github
 #        env:
 #          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
   mypy-linux:
     name: mypy check on linux
```

### Comparing `kiara-0.5.8/.github/workflows/build-windows.yaml` & `kiara-0.5.9/.github/workflows/build-windows.yaml`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/.gitignore` & `kiara-0.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/.gitlab-ci.yml` & `kiara-0.5.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/.kiara_complete.zsh` & `kiara-0.5.9/.kiara_complete.zsh`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/.pre-commit-config.yaml` & `kiara-0.5.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/CHANGELOG.md` & `kiara-0.5.9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/LICENSE` & `kiara-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/Makefile` & `kiara-0.5.9/Makefile`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/PKG-INFO` & `kiara-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara
-Version: 0.5.8
+Version: 0.5.9
 Summary: Data-centric workflow orchestration.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara
 Project-URL: documentation, https://dharpa.org/kiara.documentation
 Project-URL: repository, https://github.com/DHARPA-Project/kiara
 Keywords: kiara
@@ -78,15 +78,15 @@
 Requires-Dist: mkdocs-literate-nav>=0.4.0; extra == "dev-documentation"
 Requires-Dist: mkdocs-macros-plugin<1.1.0,>=0.7.0; extra == "dev-documentation"
 Requires-Dist: mkdocs-material>=8.0.0; extra == "dev-documentation"
 Requires-Dist: mkdocs-section-index>0.3.0; extra == "dev-documentation"
 Requires-Dist: mkdocstrings[python]>=0.18; extra == "dev-documentation"
 Requires-Dist: mkdocs-gen-files>=0.3.1; extra == "dev-documentation"
 Provides-Extra: dev-testing
-Requires-Dist: coveralls>=3.2.0; extra == "dev-testing"
+Requires-Dist: pytest-cov>=4.1.0; extra == "dev-testing"
 Requires-Dist: flake8>=3.8.4; extra == "dev-testing"
 Requires-Dist: jsonschema>=4.0.0; extra == "dev-testing"
 Requires-Dist: mypy>=0.800; extra == "dev-testing"
 Requires-Dist: pandas-stubs; extra == "dev-testing"
 Requires-Dist: pytest>=6.2.2; extra == "dev-testing"
 Requires-Dist: pytest-cov>=2.11.1; extra == "dev-testing"
 Requires-Dist: pytest-html>=3.1.0; extra == "dev-testing"
```

### Comparing `kiara-0.5.8/README.md` & `kiara-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/ci/conda/conda-pkg-patch.yaml` & `kiara-0.5.9/ci/conda/conda-pkg-patch.yaml`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/dev/dev.ipynb` & `kiara-0.5.9/dev/dev.ipynb`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/dev/script.py` & `kiara-0.5.9/dev/script.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/docs/design_docs/architecture/assumptions.md` & `kiara-0.5.9/docs/design_docs/architecture/assumptions.md`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/docs/design_docs/architecture/data/data_centric_approach.ipynb` & `kiara-0.5.9/docs/design_docs/architecture/data/data_centric_approach.ipynb`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/docs/design_docs/architecture/data/data_formats.ipynb` & `kiara-0.5.9/docs/design_docs/architecture/data/data_formats.ipynb`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/docs/design_docs/architecture/data/dev.ipynb` & `kiara-0.5.9/docs/design_docs/architecture/data/dev.ipynb`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/docs/design_docs/architecture/data/index.md` & `kiara-0.5.9/docs/design_docs/architecture/data/index.md`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/docs/design_docs/architecture/data/persistence.md` & `kiara-0.5.9/docs/design_docs/architecture/data/persistence.md`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/docs/design_docs/architecture/data/requirements.ipynb` & `kiara-0.5.9/docs/design_docs/architecture/data/requirements.ipynb`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/docs/design_docs/architecture/data/result_tree.png` & `kiara-0.5.9/docs/design_docs/architecture/data/result_tree.png`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/docs/design_docs/architecture/decisions.md` & `kiara-0.5.9/docs/design_docs/architecture/decisions.md`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/docs/design_docs/architecture/metadata.md` & `kiara-0.5.9/docs/design_docs/architecture/metadata.md`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/docs/design_docs/architecture/workflows/index.md` & `kiara-0.5.9/docs/design_docs/architecture/workflows/index.md`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/docs/design_docs/architecture/workflows/modularity/modularity.ipynb` & `kiara-0.5.9/docs/design_docs/architecture/workflows/modularity/modularity.ipynb`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/docs/design_docs/architecture/workflows/modularity/modularity_2.ipynb` & `kiara-0.5.9/docs/design_docs/architecture/workflows/modularity/modularity_2.ipynb`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/docs/design_docs/architecture/workflows/modularity/workflows/corpus_processing.yaml` & `kiara-0.5.9/docs/design_docs/architecture/workflows/modularity/workflows/corpus_processing.yaml`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/docs/design_docs/architecture/workflows/modularity/workflows/input_files_processing.yaml` & `kiara-0.5.9/docs/design_docs/architecture/workflows/modularity/workflows/input_files_processing.yaml`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/docs/development/index.md` & `kiara-0.5.9/docs/development/index.md`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/docs/development/install.md` & `kiara-0.5.9/docs/development/install.md`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/docs/development/modules/render_value.md` & `kiara-0.5.9/docs/development/modules/render_value.md`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/docs/development/rendering.md` & `kiara-0.5.9/docs/development/rendering.md`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/examples/data/journals/JournalEdges1902.csv` & `kiara-0.5.9/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/examples/data/journals/JournalNodes1902.csv` & `kiara-0.5.9/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-1_seq-1_ocr.txt` & `kiara-0.5.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-2_seq-1_ocr.txt` & `kiara-0.5.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-2_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-3_seq-1_ocr.txt` & `kiara-0.5.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-3_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-4_seq-1_ocr.txt` & `kiara-0.5.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-4_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-1_seq-1_ocr.txt` & `kiara-0.5.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-2_seq-1_ocr.txt` & `kiara-0.5.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-2_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-3_seq-1_ocr.txt` & `kiara-0.5.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-3_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-4_seq-1_ocr.txt` & `kiara-0.5.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-4_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-16_ed-1_seq-1_ocr.txt` & `kiara-0.5.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-16_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-16_ed-2_seq-1_ocr.txt` & `kiara-0.5.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-16_ed-2_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-16_ed-3_seq-1_ocr.txt` & `kiara-0.5.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-16_ed-3_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-07_ed-1_seq-1_ocr.txt` & `kiara-0.5.9/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-07_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-14_ed-1_seq-1_ocr.txt` & `kiara-0.5.9/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-14_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-14_ed-2_seq-1_ocr.txt` & `kiara-0.5.9/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-14_ed-2_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-21_ed-1_seq-1_ocr.txt` & `kiara-0.5.9/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-21_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-21_ed-2_seq-1_ocr.txt` & `kiara-0.5.9/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-21_ed-2_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/examples/jupyter/install_example.ipynb` & `kiara-0.5.9/examples/jupyter/install_example.ipynb`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/examples/pipelines/mock_pipeline_1.yaml` & `kiara-0.5.9/examples/pipelines/mock_pipeline_1.yaml`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/mkdocs.yml` & `kiara-0.5.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/pyproject.toml` & `kiara-0.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -219,15 +219,15 @@
     "mkdocs-material>=8.0.0",
     "mkdocs-section-index>0.3.0",
     "mkdocstrings[python]>=0.18",
     "mkdocs-gen-files>=0.3.1"
 ]
 
 dev_testing = [
-    "coveralls>=3.2.0",
+    "pytest-cov>=4.1.0",
     "flake8>=3.8.4",
     "jsonschema>=4.0.0",
     "mypy>=0.800",
     "pandas-stubs",
     "pytest>=6.2.2",
     "pytest-cov>=2.11.1",
     "pytest-html>=3.1.0",
```

### Comparing `kiara-0.5.8/scripts/documentation/gen_api_doc_pages.py` & `kiara-0.5.9/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/scripts/documentation/gen_schemas.py` & `kiara-0.5.9/scripts/documentation/gen_schemas.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/__init__.py` & `kiara-0.5.9/src/kiara/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/api.py` & `kiara-0.5.9/src/kiara/api.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/context/__init__.py` & `kiara-0.5.9/src/kiara/context/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/context/config.py` & `kiara-0.5.9/src/kiara/context/config.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/context/orm.py` & `kiara-0.5.9/src/kiara/context/orm.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/context/runtime_config.py` & `kiara-0.5.9/src/kiara/context/runtime_config.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/data_types/__init__.py` & `kiara-0.5.9/src/kiara/data_types/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/data_types/included_core_types/__init__.py` & `kiara-0.5.9/src/kiara/data_types/included_core_types/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/data_types/included_core_types/filesystem.py` & `kiara-0.5.9/src/kiara/data_types/included_core_types/filesystem.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/data_types/included_core_types/internal/__init__.py` & `kiara-0.5.9/src/kiara/data_types/included_core_types/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/data_types/included_core_types/internal/render_value.py` & `kiara-0.5.9/src/kiara/data_types/included_core_types/internal/render_value.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/data_types/included_core_types/metadata.py` & `kiara-0.5.9/src/kiara/data_types/included_core_types/metadata.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/data_types/included_core_types/serialization.py` & `kiara-0.5.9/src/kiara/data_types/included_core_types/serialization.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/defaults.py` & `kiara-0.5.9/src/kiara/defaults.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/doc/__init__.py` & `kiara-0.5.9/src/kiara/doc/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/doc/gen_info_pages.py` & `kiara-0.5.9/src/kiara/doc/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/doc/generate_api_doc.py` & `kiara-0.5.9/src/kiara/doc/generate_api_doc.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/doc/mkdocs_macros_cli.py` & `kiara-0.5.9/src/kiara/doc/mkdocs_macros_cli.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/doc/mkdocs_macros_kiara.py` & `kiara-0.5.9/src/kiara/doc/mkdocs_macros_kiara.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/doc/mkdocstrings/collector.py` & `kiara-0.5.9/src/kiara/doc/mkdocstrings/collector.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/doc/mkdocstrings/handler.py` & `kiara-0.5.9/src/kiara/doc/mkdocstrings/handler.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/doc/mkdocstrings/renderer.py` & `kiara-0.5.9/src/kiara/doc/mkdocstrings/renderer.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/exceptions.py` & `kiara-0.5.9/src/kiara/exceptions.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/interfaces/__init__.py` & `kiara-0.5.9/src/kiara/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/interfaces/cli/__init__.py` & `kiara-0.5.9/src/kiara/interfaces/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/interfaces/cli/context/commands.py` & `kiara-0.5.9/src/kiara/interfaces/cli/context/commands.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/interfaces/cli/data/commands.py` & `kiara-0.5.9/src/kiara/interfaces/cli/data/commands.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/interfaces/cli/info/commands.py` & `kiara-0.5.9/src/kiara/interfaces/cli/info/commands.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/interfaces/cli/module/commands.py` & `kiara-0.5.9/src/kiara/interfaces/cli/module/commands.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/interfaces/cli/operation/commands.py` & `kiara-0.5.9/src/kiara/interfaces/cli/operation/commands.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/interfaces/cli/pipeline/commands.py` & `kiara-0.5.9/src/kiara/interfaces/cli/pipeline/commands.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/interfaces/cli/proxy_cli.py` & `kiara-0.5.9/src/kiara/interfaces/cli/proxy_cli.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/interfaces/cli/render/commands.py` & `kiara-0.5.9/src/kiara/interfaces/cli/render/commands.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/interfaces/cli/run.py` & `kiara-0.5.9/src/kiara/interfaces/cli/run.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/interfaces/cli/type/commands.py` & `kiara-0.5.9/src/kiara/interfaces/cli/type/commands.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/interfaces/cli/workflow/commands.py` & `kiara-0.5.9/src/kiara/interfaces/cli/workflow/commands.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/interfaces/python_api/__init__.py` & `kiara-0.5.9/src/kiara/interfaces/python_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1573,15 +1573,14 @@
         Returns:
             a value map instance
         """
 
         if register_data:
             temp: Dict[str, Union[str, Value, uuid.UUID, None]] = {}
             for k, v in values.items():
-
                 if isinstance(v, (Value, uuid.UUID)):
                     temp[k] = v
                     continue
 
                 if not values_schema:
                     details = "No schema provided."
                     raise KiaraException(
@@ -1591,14 +1590,19 @@
                 if k not in values_schema.keys():
                     details = "Valid field names: " + ", ".join(values_schema.keys())
                     raise KiaraException(
                         f"Invalid field name: '{k}' (value: {str(v)}).", details=details
                     )
 
                 if isinstance(v, str):
+
+                    if v.startswith("alias:"):
+                        temp[k] = v
+                        continue
+
                     try:
                         v = uuid.UUID(v)
                         temp[k] = v
                         continue
                     except Exception:
                         if v.startswith("alias:"):  # type: ignore
                             _v = v.replace("alias:", "")  # type: ignore
@@ -2099,14 +2103,15 @@
 
         Returns:
             the job result value map
 
         """
         if inputs is None:
             inputs = {}
+
         job_id = self.queue_job(
             operation=operation, inputs=inputs, operation_config=operation_config
         )
         return self.context.job_registry.retrieve_result(job_id=job_id)
 
     def get_job(self, job_id: Union[str, uuid.UUID]) -> ActiveJob:
         """Retrieve the status of the job with the provided id."""
```

### Comparing `kiara-0.5.8/src/kiara/interfaces/python_api/batch.py` & `kiara-0.5.9/src/kiara/interfaces/python_api/batch.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/interfaces/python_api/models/doc.py` & `kiara-0.5.9/src/kiara/interfaces/python_api/models/doc.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/interfaces/python_api/models/info.py` & `kiara-0.5.9/src/kiara/interfaces/python_api/models/info.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/interfaces/python_api/models/job.py` & `kiara-0.5.9/src/kiara/interfaces/python_api/models/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,14 +272,15 @@
 
         result = self.run_job()
         self.check_result(result)
 
     def run_job(self) -> "ValueMap":
 
         print(f"Running checks for job '{self._job_desc.job_alias}'...")  # noqa
+
         try:
             result = self._kiara_api.run_job(operation=self._job_desc)
         except Exception as e:
             exc = KiaraException(f"Failed to run job '{self._job_desc.job_alias}': {e}")
             terminal_print(exc)
             raise e
         return result
```

### Comparing `kiara-0.5.8/src/kiara/interfaces/python_api/models/workflow.py` & `kiara-0.5.9/src/kiara/interfaces/python_api/models/workflow.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/interfaces/python_api/operation.py` & `kiara-0.5.9/src/kiara/interfaces/python_api/operation.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/interfaces/python_api/proxy.py` & `kiara-0.5.9/src/kiara/interfaces/python_api/proxy.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/interfaces/python_api/utils.py` & `kiara-0.5.9/src/kiara/interfaces/python_api/utils.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/interfaces/python_api/value.py` & `kiara-0.5.9/src/kiara/interfaces/python_api/value.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/interfaces/python_api/workflow.py` & `kiara-0.5.9/src/kiara/interfaces/python_api/workflow.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/__init__.py` & `kiara-0.5.9/src/kiara/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/aliases/__init__.py` & `kiara-0.5.9/src/kiara/models/aliases/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/archives.py` & `kiara-0.5.9/src/kiara/models/archives.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/context.py` & `kiara-0.5.9/src/kiara/models/context.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/data_types.py` & `kiara-0.5.9/src/kiara/models/data_types.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/documentation.py` & `kiara-0.5.9/src/kiara/models/documentation.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/events/__init__.py` & `kiara-0.5.9/src/kiara/models/events/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/events/alias_registry.py` & `kiara-0.5.9/src/kiara/models/events/alias_registry.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/events/data_registry.py` & `kiara-0.5.9/src/kiara/models/events/data_registry.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/events/destiny_registry.py` & `kiara-0.5.9/src/kiara/models/events/destiny_registry.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/events/job_registry.py` & `kiara-0.5.9/src/kiara/models/events/job_registry.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/events/pipeline.py` & `kiara-0.5.9/src/kiara/models/events/pipeline.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/events/workflow_registry.py` & `kiara-0.5.9/src/kiara/models/events/workflow_registry.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/filesystem.py` & `kiara-0.5.9/src/kiara/models/filesystem.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/module/__init__.py` & `kiara-0.5.9/src/kiara/models/module/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/module/destiny.py` & `kiara-0.5.9/src/kiara/models/module/destiny.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/module/jobs.py` & `kiara-0.5.9/src/kiara/models/module/jobs.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/module/manifest.py` & `kiara-0.5.9/src/kiara/models/module/manifest.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/module/operation.py` & `kiara-0.5.9/src/kiara/models/module/operation.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/module/persistence.py` & `kiara-0.5.9/src/kiara/models/module/persistence.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/module/pipeline/__init__.py` & `kiara-0.5.9/src/kiara/models/module/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/module/pipeline/controller.py` & `kiara-0.5.9/src/kiara/models/module/pipeline/controller.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/module/pipeline/pipeline.py` & `kiara-0.5.9/src/kiara/models/module/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/module/pipeline/stages.py` & `kiara-0.5.9/src/kiara/models/module/pipeline/stages.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/module/pipeline/structure.py` & `kiara-0.5.9/src/kiara/models/module/pipeline/structure.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/module/pipeline/value_refs.py` & `kiara-0.5.9/src/kiara/models/module/pipeline/value_refs.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/python_class.py` & `kiara-0.5.9/src/kiara/models/python_class.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/rendering/__init__.py` & `kiara-0.5.9/src/kiara/models/rendering/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/rendering/values.py` & `kiara-0.5.9/src/kiara/models/rendering/values.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/runtime_environment/__init__.py` & `kiara-0.5.9/src/kiara/models/runtime_environment/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/runtime_environment/kiara.py` & `kiara-0.5.9/src/kiara/models/runtime_environment/kiara.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/runtime_environment/operating_system.py` & `kiara-0.5.9/src/kiara/models/runtime_environment/operating_system.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/runtime_environment/python.py` & `kiara-0.5.9/src/kiara/models/runtime_environment/python.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/values/__init__.py` & `kiara-0.5.9/src/kiara/models/values/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/values/data_type.py` & `kiara-0.5.9/src/kiara/models/values/data_type.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/values/lineage.py` & `kiara-0.5.9/src/kiara/models/values/lineage.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/values/matchers.py` & `kiara-0.5.9/src/kiara/models/values/matchers.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/values/value.py` & `kiara-0.5.9/src/kiara/models/values/value.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/values/value_metadata/__init__.py` & `kiara-0.5.9/src/kiara/models/values/value_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/values/value_metadata/included_metadata_types/__init__.py` & `kiara-0.5.9/src/kiara/models/values/value_metadata/included_metadata_types/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/values/value_schema.py` & `kiara-0.5.9/src/kiara/models/values/value_schema.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/models/workflow.py` & `kiara-0.5.9/src/kiara/models/workflow.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/modules/__init__.py` & `kiara-0.5.9/src/kiara/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/modules/included_core_modules/create_from.py` & `kiara-0.5.9/src/kiara/modules/included_core_modules/create_from.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/modules/included_core_modules/export_as.py` & `kiara-0.5.9/src/kiara/modules/included_core_modules/export_as.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/modules/included_core_modules/filesystem.py` & `kiara-0.5.9/src/kiara/modules/included_core_modules/filesystem.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/modules/included_core_modules/filter.py` & `kiara-0.5.9/src/kiara/modules/included_core_modules/filter.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/modules/included_core_modules/metadata.py` & `kiara-0.5.9/src/kiara/modules/included_core_modules/metadata.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/modules/included_core_modules/mock.py` & `kiara-0.5.9/src/kiara/modules/included_core_modules/mock.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/modules/included_core_modules/pipeline.py` & `kiara-0.5.9/src/kiara/modules/included_core_modules/pipeline.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/modules/included_core_modules/pretty_print.py` & `kiara-0.5.9/src/kiara/modules/included_core_modules/pretty_print.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/modules/included_core_modules/render_value.py` & `kiara-0.5.9/src/kiara/modules/included_core_modules/render_value.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/modules/included_core_modules/serialization.py` & `kiara-0.5.9/src/kiara/modules/included_core_modules/serialization.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/operations/__init__.py` & `kiara-0.5.9/src/kiara/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/operations/included_core_operations/__init__.py` & `kiara-0.5.9/src/kiara/operations/included_core_operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/operations/included_core_operations/create_from.py` & `kiara-0.5.9/src/kiara/operations/included_core_operations/create_from.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/operations/included_core_operations/export_as.py` & `kiara-0.5.9/src/kiara/operations/included_core_operations/export_as.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/operations/included_core_operations/filter.py` & `kiara-0.5.9/src/kiara/operations/included_core_operations/filter.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/operations/included_core_operations/import_data.py` & `kiara-0.5.9/src/kiara/operations/included_core_operations/import_data.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/operations/included_core_operations/metadata.py` & `kiara-0.5.9/src/kiara/operations/included_core_operations/metadata.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/operations/included_core_operations/pipeline.py` & `kiara-0.5.9/src/kiara/operations/included_core_operations/pipeline.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/operations/included_core_operations/pretty_print.py` & `kiara-0.5.9/src/kiara/operations/included_core_operations/pretty_print.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/operations/included_core_operations/render_data.py` & `kiara-0.5.9/src/kiara/operations/included_core_operations/render_data.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/operations/included_core_operations/render_value.py` & `kiara-0.5.9/src/kiara/operations/included_core_operations/render_value.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/operations/included_core_operations/serialize.py` & `kiara-0.5.9/src/kiara/operations/included_core_operations/serialize.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/processing/__init__.py` & `kiara-0.5.9/src/kiara/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/processing/synchronous.py` & `kiara-0.5.9/src/kiara/processing/synchronous.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/registries/__init__.py` & `kiara-0.5.9/src/kiara/registries/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/registries/aliases/__init__.py` & `kiara-0.5.9/src/kiara/registries/aliases/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/registries/aliases/archives.py` & `kiara-0.5.9/src/kiara/registries/aliases/archives.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/registries/data/__init__.py` & `kiara-0.5.9/src/kiara/registries/data/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -364,15 +364,14 @@
 
                 if _value_id is None:
 
                     if not isinstance(value, str):
                         raise Exception(
                             f"Can't retrieve value for '{value}': invalid type '{type(value)}'."
                         )
-
                     _value_id = self._alias_resolver.resolve_alias(value)
         else:
             _value_id = value
 
         assert _value_id is not None
 
         if _value_id in self._registered_values.keys():
@@ -1014,14 +1013,15 @@
         return {k: v.data for k, v in result_values.items()}
 
     def create_valuemap(
         self, data: Mapping[str, Any], schema: Mapping[str, ValueSchema]
     ) -> ValueMap:
         """Extract a set of [Value][kiara.data.values.Value] from Python data and ValueSchemas."""
         input_details = {}
+
         for input_name, value_schema in schema.items():
             input_details[input_name] = {"schema": value_schema}
 
         leftover = set(data.keys())
         leftover.difference_update(input_details.keys())
         if leftover:
             if not STRICT_CHECKS:
@@ -1038,15 +1038,23 @@
         _unresolved = {}
         for input_name, details in input_details.items():
             _d = data.get(input_name, SpecialValue.NOT_SET)
             if isinstance(_d, str):
                 try:
                     _d = uuid.UUID(_d)
                 except Exception:
-                    pass
+                    if schema[input_name].type == "string" and not (
+                        _d.startswith("alias:") or _d.startswith("value:")
+                    ):
+                        pass
+                    else:
+                        try:
+                            _d = self._alias_resolver.resolve_alias(_d)
+                        except Exception:
+                            pass
 
             if isinstance(_d, Value):
                 _resolved[input_name] = _d
             elif isinstance(_d, uuid.UUID):
                 _resolved[input_name] = self.get_value(_d)
             else:
                 _unresolved[input_name] = _d
```

### Comparing `kiara-0.5.8/src/kiara/registries/data/data_store/__init__.py` & `kiara-0.5.9/src/kiara/registries/data/data_store/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/registries/data/data_store/filesystem_store.py` & `kiara-0.5.9/src/kiara/registries/data/data_store/filesystem_store.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/registries/destinies/__init__.py` & `kiara-0.5.9/src/kiara/registries/destinies/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/registries/destinies/filesystem_store.py` & `kiara-0.5.9/src/kiara/registries/destinies/filesystem_store.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/registries/destinies/registry.py` & `kiara-0.5.9/src/kiara/registries/destinies/registry.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/registries/environment/__init__.py` & `kiara-0.5.9/src/kiara/registries/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/registries/events/__init__.py` & `kiara-0.5.9/src/kiara/registries/events/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/registries/events/metadata.py` & `kiara-0.5.9/src/kiara/registries/events/metadata.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/registries/events/registry.py` & `kiara-0.5.9/src/kiara/registries/events/registry.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/registries/ids/__init__.py` & `kiara-0.5.9/src/kiara/registries/ids/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/registries/jobs/__init__.py` & `kiara-0.5.9/src/kiara/registries/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/registries/jobs/job_store/filesystem_store.py` & `kiara-0.5.9/src/kiara/registries/jobs/job_store/filesystem_store.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/registries/models/__init__.py` & `kiara-0.5.9/src/kiara/registries/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/registries/modules/__init__.py` & `kiara-0.5.9/src/kiara/registries/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/registries/operations/__init__.py` & `kiara-0.5.9/src/kiara/registries/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/registries/rendering/__init__.py` & `kiara-0.5.9/src/kiara/registries/rendering/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/registries/templates/__init__.py` & `kiara-0.5.9/src/kiara/registries/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/registries/types/__init__.py` & `kiara-0.5.9/src/kiara/registries/types/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/registries/workflows/__init__.py` & `kiara-0.5.9/src/kiara/registries/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/registries/workflows/archives.py` & `kiara-0.5.9/src/kiara/registries/workflows/archives.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/renderers/__init__.py` & `kiara-0.5.9/src/kiara/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/renderers/included_renderers/api.py` & `kiara-0.5.9/src/kiara/renderers/included_renderers/api.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/renderers/included_renderers/pipeline.py` & `kiara-0.5.9/src/kiara/renderers/included_renderers/pipeline.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/renderers/included_renderers/value.py` & `kiara-0.5.9/src/kiara/renderers/included_renderers/value.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/renderers/jinja.py` & `kiara-0.5.9/src/kiara/renderers/jinja.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/resources/templates/render/models/macros.html` & `kiara-0.5.9/src/kiara/resources/templates/render/models/macros.html`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/resources/templates/render/models/metadata.context.html` & `kiara-0.5.9/src/kiara/resources/templates/render/models/metadata.context.html`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/resources/templates/render/pipeline/pipeline_info.md.j2` & `kiara-0.5.9/src/kiara/resources/templates/render/pipeline/pipeline_info.md.j2`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/resources/templates/render/pipeline/python_script.py.j2` & `kiara-0.5.9/src/kiara/resources/templates/render/pipeline/python_script.py.j2`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/resources/tui/pager_app.css` & `kiara-0.5.9/src/kiara/resources/tui/pager_app.css`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/__init__.py` & `kiara-0.5.9/src/kiara/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/class_loading.py` & `kiara-0.5.9/src/kiara/utils/class_loading.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/cli/__init__.py` & `kiara-0.5.9/src/kiara/utils/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/cli/exceptions.py` & `kiara-0.5.9/src/kiara/utils/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/cli/rich_click.py` & `kiara-0.5.9/src/kiara/utils/cli/rich_click.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/cli/run.py` & `kiara-0.5.9/src/kiara/utils/cli/run.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/concurrency.py` & `kiara-0.5.9/src/kiara/utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/data.py` & `kiara-0.5.9/src/kiara/utils/data.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/db.py` & `kiara-0.5.9/src/kiara/utils/db.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/debug.py` & `kiara-0.5.9/src/kiara/utils/debug.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/develop/__init__.py` & `kiara-0.5.9/src/kiara/utils/develop/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/doc.py` & `kiara-0.5.9/src/kiara/utils/doc.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/downloads.py` & `kiara-0.5.9/src/kiara/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/files.py` & `kiara-0.5.9/src/kiara/utils/files.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/global_metadata.py` & `kiara-0.5.9/src/kiara/utils/global_metadata.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/graphs.py` & `kiara-0.5.9/src/kiara/utils/graphs.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/hashfs/__init__.py` & `kiara-0.5.9/src/kiara/utils/hashfs/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/hashing.py` & `kiara-0.5.9/src/kiara/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/html.py` & `kiara-0.5.9/src/kiara/utils/html.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/json.py` & `kiara-0.5.9/src/kiara/utils/json.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/metadata.py` & `kiara-0.5.9/src/kiara/utils/metadata.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/models.py` & `kiara-0.5.9/src/kiara/utils/models.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/operations.py` & `kiara-0.5.9/src/kiara/utils/operations.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/output.py` & `kiara-0.5.9/src/kiara/utils/output.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/pipelines.py` & `kiara-0.5.9/src/kiara/utils/pipelines.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/reflection.py` & `kiara-0.5.9/src/kiara/utils/reflection.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/rendering.py` & `kiara-0.5.9/src/kiara/utils/rendering.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/string_vars.py` & `kiara-0.5.9/src/kiara/utils/string_vars.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/testing/__init__.py` & `kiara-0.5.9/src/kiara/utils/testing/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,29 +12,42 @@
 
 def get_init_job(jobs_folder: Path) -> Union[None, JobDesc]:
 
     init_test_yaml = jobs_folder / f"{INIT_EXAMPLE_NAME}.yaml"
     if init_test_yaml.is_file():
         return JobDesc.create_from_file(init_test_yaml)
 
+    init_test_yaml = jobs_folder / f"{INIT_EXAMPLE_NAME}.yml"
+    if init_test_yaml.is_file():
+        return JobDesc.create_from_file(init_test_yaml)
+
     init_test_json = jobs_folder / f"{INIT_EXAMPLE_NAME}.json"
     if init_test_json.is_file():
         return JobDesc.create_from_file(init_test_json)
 
     return None
 
 
 def list_job_descs(jobs_folder: Path):
 
     init_job = get_init_job(jobs_folder)
     if init_job is not None:
         yield init_job
 
-    for f in sorted(jobs_folder.glob("*")):
-        if f.name in [f"{INIT_EXAMPLE_NAME}.yaml", f"{INIT_EXAMPLE_NAME}.json"]:
+    files = (
+        list(jobs_folder.glob("*.yaml"))
+        + list(jobs_folder.glob("*.yml"))
+        + list(jobs_folder.glob("*.json"))
+    )
+    for f in sorted(files):
+        if f.name in [
+            f"{INIT_EXAMPLE_NAME}.yaml",
+            f"{INIT_EXAMPLE_NAME}.yml",
+            "{INIT_EXAMPLE_NAME}.json",
+        ]:
             continue
         try:
             job_desc = JobDesc.create_from_file(f)
             yield job_desc
         except Exception as e:
             log_exception(e)
 
@@ -66,14 +79,16 @@
 
     test_checks = test_folder / "outputs.json"
     if not test_checks.is_file():
         test_checks = test_folder / "outputs.yaml"
 
     if test_checks.is_file():
         test_data: Dict[str, Any] = get_data_from_file(test_checks)
+        if test_data is None:
+            test_data = {}
     else:
         test_data = {}
 
     for k, v in test_data.items():
         if k in tests.keys():
             raise Exception(f"Duplicate test name: {k}")
         tests[k] = v
```

### Comparing `kiara-0.5.8/src/kiara/utils/values.py` & `kiara-0.5.9/src/kiara/utils/values.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/utils/windows.py` & `kiara-0.5.9/src/kiara/utils/windows.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/zmq/__init__.py` & `kiara-0.5.9/src/kiara/zmq/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/zmq/client.py` & `kiara-0.5.9/src/kiara/zmq/client.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/zmq/messages/__init__.py` & `kiara-0.5.9/src/kiara/zmq/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara/zmq/service/__init__.py` & `kiara-0.5.9/src/kiara/zmq/service/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara.egg-info/PKG-INFO` & `kiara-0.5.9/src/kiara.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara
-Version: 0.5.8
+Version: 0.5.9
 Summary: Data-centric workflow orchestration.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara
 Project-URL: documentation, https://dharpa.org/kiara.documentation
 Project-URL: repository, https://github.com/DHARPA-Project/kiara
 Keywords: kiara
@@ -78,15 +78,15 @@
 Requires-Dist: mkdocs-literate-nav>=0.4.0; extra == "dev-documentation"
 Requires-Dist: mkdocs-macros-plugin<1.1.0,>=0.7.0; extra == "dev-documentation"
 Requires-Dist: mkdocs-material>=8.0.0; extra == "dev-documentation"
 Requires-Dist: mkdocs-section-index>0.3.0; extra == "dev-documentation"
 Requires-Dist: mkdocstrings[python]>=0.18; extra == "dev-documentation"
 Requires-Dist: mkdocs-gen-files>=0.3.1; extra == "dev-documentation"
 Provides-Extra: dev-testing
-Requires-Dist: coveralls>=3.2.0; extra == "dev-testing"
+Requires-Dist: pytest-cov>=4.1.0; extra == "dev-testing"
 Requires-Dist: flake8>=3.8.4; extra == "dev-testing"
 Requires-Dist: jsonschema>=4.0.0; extra == "dev-testing"
 Requires-Dist: mypy>=0.800; extra == "dev-testing"
 Requires-Dist: pandas-stubs; extra == "dev-testing"
 Requires-Dist: pytest>=6.2.2; extra == "dev-testing"
 Requires-Dist: pytest-cov>=2.11.1; extra == "dev-testing"
 Requires-Dist: pytest-html>=3.1.0; extra == "dev-testing"
```

### Comparing `kiara-0.5.8/src/kiara.egg-info/SOURCES.txt` & `kiara-0.5.9/src/kiara.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara.egg-info/entry_points.txt` & `kiara-0.5.9/src/kiara.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/src/kiara.egg-info/requires.txt` & `kiara-0.5.9/src/kiara.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 mkdocs-macros-plugin<1.1.0,>=0.7.0
 mkdocs-material>=8.0.0
 mkdocs-section-index>0.3.0
 mkdocstrings[python]>=0.18
 mkdocs-gen-files>=0.3.1
 
 [dev_testing]
-coveralls>=3.2.0
+pytest-cov>=4.1.0
 flake8>=3.8.4
 jsonschema>=4.0.0
 mypy>=0.800
 pandas-stubs
 pytest>=6.2.2
 pytest-cov>=2.11.1
 pytest-html>=3.1.0
```

### Comparing `kiara-0.5.8/tests/conftest.py` & `kiara-0.5.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/tests/resources/pipelines/test_preseed_1.yaml` & `kiara-0.5.9/tests/resources/pipelines/test_preseed_1.yaml`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/tests/test_api/test_data_types.py` & `kiara-0.5.9/tests/test_api/test_data_types.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/tests/test_api/test_misc.py` & `kiara-0.5.9/tests/test_api/test_misc.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/tests/test_api/test_module_types.py` & `kiara-0.5.9/tests/test_api/test_module_types.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/tests/test_api/test_operations.py` & `kiara-0.5.9/tests/test_api/test_operations.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/tests/test_cli/test_context_subcommands.py` & `kiara-0.5.9/tests/test_cli/test_context_subcommands.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/tests/test_cli/test_data_subcommands.py` & `kiara-0.5.9/tests/test_cli/test_data_subcommands.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/tests/test_cli/test_metadata_subcommands.py` & `kiara-0.5.9/tests/test_cli/test_metadata_subcommands.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/tests/test_cli/test_misc_commands.py` & `kiara-0.5.9/tests/test_cli/test_misc_commands.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/tests/test_cli/test_module_subcommands.py` & `kiara-0.5.9/tests/test_cli/test_module_subcommands.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/tests/test_cli/test_operation_subcommands.py` & `kiara-0.5.9/tests/test_cli/test_operation_subcommands.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/tests/test_cli/test_pipeline_subcommands.py` & `kiara-0.5.9/tests/test_cli/test_pipeline_subcommands.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/tests/test_cli/test_run_subcommand.py` & `kiara-0.5.9/tests/test_cli/test_run_subcommand.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/tests/test_included_data_types/test_string.py` & `kiara-0.5.9/tests/test_included_data_types/test_string.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/tests/test_kiara_context.py` & `kiara-0.5.9/tests/test_kiara_context.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/tests/test_module_instances.py` & `kiara-0.5.9/tests/test_module_instances.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/tests/test_module_types.py` & `kiara-0.5.9/tests/test_module_types.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/tests/test_modules/test_operations.py` & `kiara-0.5.9/tests/test_modules/test_operations.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/tests/test_modules/test_simple_module_exec.py` & `kiara-0.5.9/tests/test_modules/test_simple_module_exec.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/tests/test_operation_types/test_extract_metadata.py` & `kiara-0.5.9/tests/test_operation_types/test_extract_metadata.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/tests/test_operation_types/test_persist_value.py` & `kiara-0.5.9/tests/test_operation_types/test_persist_value.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/tests/test_operation_types/test_render_value.py` & `kiara-0.5.9/tests/test_operation_types/test_render_value.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/tests/test_operations.py` & `kiara-0.5.9/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/tests/test_pipeline_creation.py` & `kiara-0.5.9/tests/test_pipeline_creation.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/tests/test_pipelines/test_pipeline_configs.py` & `kiara-0.5.9/tests/test_pipelines/test_pipeline_configs.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/tests/test_pipelines/test_pipelines.py` & `kiara-0.5.9/tests/test_pipelines/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/tests/test_rendering.py` & `kiara-0.5.9/tests/test_rendering.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/tests/test_values/test_values.py` & `kiara-0.5.9/tests/test_values/test_values.py`

 * *Files identical despite different names*

### Comparing `kiara-0.5.8/tests/utils.py` & `kiara-0.5.9/tests/utils.py`

 * *Files identical despite different names*

