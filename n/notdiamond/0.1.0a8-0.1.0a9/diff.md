# Comparing `tmp/notdiamond-0.1.0a8.tar.gz` & `tmp/notdiamond-0.1.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notdiamond-0.1.0a8.tar", max compression
+gzip compressed data, was "notdiamond-0.1.0a9.tar", max compression
```

## Comparing `notdiamond-0.1.0a8.tar` & `notdiamond-0.1.0a9.tar`

### file list

```diff
@@ -1,514 +1,549 @@
--rw-r--r--   0        0        0      589 2024-03-01 15:42:06.040247 notdiamond-0.1.0a8/README.md
--rw-r--r--   0        0        0       37 2024-03-01 15:42:06.040996 notdiamond-0.1.0a8/notdiamond/__init__.py
--rw-r--r--   0        0        0      340 2024-02-19 19:24:39.600527 notdiamond-0.1.0a8/notdiamond/exceptions.py
--rw-r--r--   0        0        0        0 2024-01-22 13:51:23.616665 notdiamond-0.1.0a8/notdiamond/llms/__init__.py
--rw-r--r--   0        0        0     8119 2024-03-06 07:49:01.130319 notdiamond-0.1.0a8/notdiamond/llms/llm.py
--rw-r--r--   0        0        0     1044 2024-03-06 07:49:05.639390 notdiamond-0.1.0a8/notdiamond/llms/provider.py
--rw-r--r--   0        0        0     2552 2024-03-06 07:50:02.901316 notdiamond-0.1.0a8/notdiamond/llms/request.py
--rw-r--r--   0        0        0        0 2024-01-22 13:51:23.617063 notdiamond-0.1.0a8/notdiamond/metrics/__init__.py
--rw-r--r--   0        0        0      601 2024-02-19 19:24:39.601384 notdiamond-0.1.0a8/notdiamond/metrics/metric.py
--rw-r--r--   0        0        0      628 2024-02-19 19:24:39.601702 notdiamond-0.1.0a8/notdiamond/metrics/request.py
--rw-r--r--   0        0        0      307 2024-02-29 19:53:45.009032 notdiamond-0.1.0a8/notdiamond/openai/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1175 2024-02-29 19:53:45.009162 notdiamond-0.1.0a8/notdiamond/openai/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0       45 2024-02-29 19:53:44.970083 notdiamond-0.1.0a8/notdiamond/openai/.git
--rw-r--r--   0        0        0       20 2024-02-29 19:53:45.009271 notdiamond-0.1.0a8/notdiamond/openai/.github/CODEOWNERS
--rw-r--r--   0        0        0     1785 2024-02-29 19:53:45.009424 notdiamond-0.1.0a8/notdiamond/openai/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      345 2024-02-29 19:53:45.009499 notdiamond-0.1.0a8/notdiamond/openai/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1028 2024-02-29 19:53:45.009579 notdiamond-0.1.0a8/notdiamond/openai/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0      496 2024-02-29 19:53:45.009648 notdiamond-0.1.0a8/notdiamond/openai/.github/pull_request_template.md
--rw-r--r--   0        0        0      790 2024-02-29 19:53:45.009756 notdiamond-0.1.0a8/notdiamond/openai/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1058 2024-02-29 19:53:45.009827 notdiamond-0.1.0a8/notdiamond/openai/.github/workflows/create-releases.yml
--rw-r--r--   0        0        0      748 2024-02-29 19:53:45.009899 notdiamond-0.1.0a8/notdiamond/openai/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0      691 2024-02-29 19:53:45.009961 notdiamond-0.1.0a8/notdiamond/openai/.github/workflows/release-doctor.yml
--rw-r--r--   0        0        0       82 2024-02-29 19:53:45.010023 notdiamond-0.1.0a8/notdiamond/openai/.gitignore
--rw-r--r--   0        0        0        7 2024-02-29 19:53:45.010074 notdiamond-0.1.0a8/notdiamond/openai/.python-version
--rw-r--r--   0        0        0       19 2024-02-29 19:53:45.010136 notdiamond-0.1.0a8/notdiamond/openai/.release-please-manifest.json
--rw-r--r--   0        0        0       25 2024-02-29 19:53:45.010189 notdiamond-0.1.0a8/notdiamond/openai/.stats.yml
--rw-r--r--   0        0        0    33847 2024-02-29 19:53:45.010362 notdiamond-0.1.0a8/notdiamond/openai/CHANGELOG.md
--rw-r--r--   0        0        0     3482 2024-02-29 19:53:45.010455 notdiamond-0.1.0a8/notdiamond/openai/CONTRIBUTING.md
--rw-r--r--   0        0        0    11336 2024-02-29 19:53:45.010564 notdiamond-0.1.0a8/notdiamond/openai/LICENSE
--rw-r--r--   0        0        0    17202 2024-02-29 19:53:45.010689 notdiamond-0.1.0a8/notdiamond/openai/README.md
--rw-r--r--   0        0        0        0 2024-02-29 20:03:23.605510 notdiamond-0.1.0a8/notdiamond/openai/__init__.py
--rw-r--r--   0        0        0      187 2024-02-29 20:11:45.266162 notdiamond-0.1.0a8/notdiamond/openai/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    17028 2024-02-29 19:53:45.010796 notdiamond-0.1.0a8/notdiamond/openai/api.md
--rw-r--r--   0        0        0      924 2024-02-29 19:53:45.010903 notdiamond-0.1.0a8/notdiamond/openai/bin/check-env-state.py
--rw-r--r--   0        0        0      658 2024-02-29 19:53:45.010981 notdiamond-0.1.0a8/notdiamond/openai/bin/check-release-environment
--rwxr-xr-x   0        0        0     1320 2024-02-29 19:53:45.011047 notdiamond-0.1.0a8/notdiamond/openai/bin/check-test-server
--rw-r--r--   0        0        0      100 2024-02-29 19:53:45.011107 notdiamond-0.1.0a8/notdiamond/openai/bin/publish-pypi
--rw-r--r--   0        0        0     5216 2024-02-29 19:53:45.011197 notdiamond-0.1.0a8/notdiamond/openai/bin/ruffen-docs.py
--rwxr-xr-x   0        0        0       66 2024-02-29 19:53:45.011250 notdiamond-0.1.0a8/notdiamond/openai/bin/test
--rw-r--r--   0        0        0      239 2024-02-29 19:53:45.011341 notdiamond-0.1.0a8/notdiamond/openai/examples/.keep
--rw-r--r--   0        0        0     1336 2024-02-29 19:53:45.011414 notdiamond-0.1.0a8/notdiamond/openai/examples/assistant.py
--rwxr-xr-x   0        0        0      462 2024-02-29 19:53:45.011475 notdiamond-0.1.0a8/notdiamond/openai/examples/async_demo.py
--rwxr-xr-x   0        0        0     1827 2024-02-29 19:53:45.011545 notdiamond-0.1.0a8/notdiamond/openai/examples/audio.py
--rwxr-xr-x   0        0        0     1460 2024-02-29 19:53:45.011610 notdiamond-0.1.0a8/notdiamond/openai/examples/azure.py
--rwxr-xr-x   0        0        0      983 2024-02-29 19:53:45.011671 notdiamond-0.1.0a8/notdiamond/openai/examples/azure_ad.py
--rwxr-xr-x   0        0        0      828 2024-02-29 19:53:45.011734 notdiamond-0.1.0a8/notdiamond/openai/examples/demo.py
--rwxr-xr-x   0        0        0      659 2024-02-29 19:53:45.011796 notdiamond-0.1.0a8/notdiamond/openai/examples/module_client.py
--rw-r--r--   0        0        0      462 2024-02-29 19:53:45.011858 notdiamond-0.1.0a8/notdiamond/openai/examples/picture.py
--rwxr-xr-x   0        0        0     1642 2024-02-29 19:53:45.011921 notdiamond-0.1.0a8/notdiamond/openai/examples/streaming.py
--rw-r--r--   0        0        0     1267 2024-02-29 19:53:45.012005 notdiamond-0.1.0a8/notdiamond/openai/mypy.ini
--rw-r--r--   0        0        0      295 2024-02-29 19:53:45.012139 notdiamond-0.1.0a8/notdiamond/openai/noxfile.py
--rw-r--r--   0        0        0     3903 2024-02-29 19:53:45.012246 notdiamond-0.1.0a8/notdiamond/openai/pyproject.toml
--rw-r--r--   0        0        0     1322 2024-02-29 19:53:45.012387 notdiamond-0.1.0a8/notdiamond/openai/release-please-config.json
--rw-r--r--   0        0        0     2691 2024-02-29 19:53:45.012556 notdiamond-0.1.0a8/notdiamond/openai/requirements-dev.lock
--rw-r--r--   0        0        0     1145 2024-02-29 19:53:45.012646 notdiamond-0.1.0a8/notdiamond/openai/requirements.lock
--rw-r--r--   0        0        0        0 2024-02-29 20:03:30.670281 notdiamond-0.1.0a8/notdiamond/openai/src/__init__.py
--rw-r--r--   0        0        0      191 2024-02-29 20:11:45.266522 notdiamond-0.1.0a8/notdiamond/openai/src/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     9140 2024-02-29 19:53:45.012863 notdiamond-0.1.0a8/notdiamond/openai/src/openai/__init__.py
--rw-r--r--   0        0        0       30 2024-02-29 19:53:45.012955 notdiamond-0.1.0a8/notdiamond/openai/src/openai/__main__.py
--rw-r--r--   0        0        0     7629 2024-02-29 20:11:45.267964 notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    42814 2024-02-29 20:11:45.351538 notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/_base_client.cpython-310.pyc
--rw-r--r--   0        0        0    12888 2024-02-29 20:11:45.326822 notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/_client.cpython-310.pyc
--rw-r--r--   0        0        0     6085 2024-02-29 20:11:45.278798 notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/_compat.cpython-310.pyc
--rw-r--r--   0        0        0      609 2024-02-29 20:11:45.282175 notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/_constants.cpython-310.pyc
--rw-r--r--   0        0        0     4489 2024-02-29 20:11:45.337545 notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/_exceptions.cpython-310.pyc
--rw-r--r--   0        0        0     4279 2024-02-29 20:11:45.353761 notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/_files.cpython-310.pyc
--rw-r--r--   0        0        0    14577 2024-02-29 20:11:45.335157 notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/_legacy_response.cpython-310.pyc
--rw-r--r--   0        0        0    13764 2024-02-29 20:11:45.271553 notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/_models.cpython-310.pyc
--rw-r--r--   0        0        0     3538 2024-02-29 20:11:49.022777 notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/_module_client.cpython-310.pyc
--rw-r--r--   0        0        0     4170 2024-02-29 20:11:45.352822 notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/_qs.cpython-310.pyc
--rw-r--r--   0        0        0     1535 2024-02-29 20:11:45.339587 notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/_resource.cpython-310.pyc
--rw-r--r--   0        0        0    24036 2024-02-29 20:11:45.343022 notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/_response.cpython-310.pyc
--rw-r--r--   0        0        0     9196 2024-02-29 20:11:45.336719 notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/_streaming.cpython-310.pyc
--rw-r--r--   0        0        0     5925 2024-02-29 20:11:45.272712 notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/_types.cpython-310.pyc
--rw-r--r--   0        0        0      245 2024-02-29 20:11:49.017226 notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/_version.cpython-310.pyc
--rw-r--r--   0        0        0     2942 2024-02-29 20:11:45.344151 notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/pagination.cpython-310.pyc
--rw-r--r--   0        0        0      293 2024-02-29 20:11:49.020800 notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/version.cpython-310.pyc
--rw-r--r--   0        0        0    62655 2024-02-29 19:53:45.013190 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_base_client.py
--rw-r--r--   0        0        0    20791 2024-02-29 19:11:33.863189 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_client.py
--rw-r--r--   0        0        0     6389 2024-02-29 19:53:45.013412 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_compat.py
--rw-r--r--   0        0        0      423 2024-02-29 19:53:45.013490 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_constants.py
--rw-r--r--   0        0        0     3614 2024-02-29 19:53:45.013576 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_exceptions.py
--rw-r--r--   0        0        0      107 2024-02-29 19:53:45.013683 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_extras/__init__.py
--rw-r--r--   0        0        0      310 2024-02-29 20:11:49.000634 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_extras/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      761 2024-02-29 20:11:49.001664 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_extras/__pycache__/_common.cpython-310.pyc
--rw-r--r--   0        0        0     1208 2024-02-29 20:11:49.001222 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_extras/__pycache__/numpy_proxy.cpython-310.pyc
--rw-r--r--   0        0        0     1032 2024-02-29 20:11:49.002105 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_extras/__pycache__/pandas_proxy.cpython-310.pyc
--rw-r--r--   0        0        0      364 2024-02-29 19:53:45.013765 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_extras/_common.py
--rw-r--r--   0        0        0      799 2024-02-29 19:53:45.013855 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_extras/numpy_proxy.py
--rw-r--r--   0        0        0      637 2024-02-29 19:53:45.013929 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_extras/pandas_proxy.py
--rw-r--r--   0        0        0     3470 2024-02-29 19:53:45.014001 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_files.py
--rw-r--r--   0        0        0    14903 2024-02-29 19:53:45.014111 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_legacy_response.py
--rw-r--r--   0        0        0    16432 2024-02-29 19:53:45.014250 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_models.py
--rw-r--r--   0        0        0     2280 2024-02-29 19:53:45.014347 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_module_client.py
--rw-r--r--   0        0        0     4846 2024-02-29 19:53:45.014419 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_qs.py
--rw-r--r--   0        0        0     1067 2024-02-29 19:53:45.014480 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_resource.py
--rw-r--r--   0        0        0    27957 2024-02-29 19:53:45.014770 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_response.py
--rw-r--r--   0        0        0     9034 2024-02-29 19:53:45.015004 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_streaming.py
--rw-r--r--   0        0        0     6123 2024-02-29 19:53:45.015107 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_types.py
--rw-r--r--   0        0        0     1727 2024-02-29 19:53:45.015288 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/__init__.py
--rw-r--r--   0        0        0     1393 2024-02-29 20:11:45.274182 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      938 2024-02-29 20:11:49.017835 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/__pycache__/_logs.cpython-310.pyc
--rw-r--r--   0        0        0     2394 2024-02-29 20:11:45.275523 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/__pycache__/_proxy.cpython-310.pyc
--rw-r--r--   0        0        0      641 2024-02-29 20:11:45.280329 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/__pycache__/_streams.cpython-310.pyc
--rw-r--r--   0        0        0     2659 2024-02-29 20:11:45.274794 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/__pycache__/_sync.cpython-310.pyc
--rw-r--r--   0        0        0     6444 2024-02-29 20:11:45.281572 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/__pycache__/_transform.cpython-310.pyc
--rw-r--r--   0        0        0     3265 2024-02-29 20:11:45.279942 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/__pycache__/_typing.cpython-310.pyc
--rw-r--r--   0        0        0    12147 2024-02-29 20:11:45.277655 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/__pycache__/_utils.cpython-310.pyc
--rw-r--r--   0        0        0      774 2024-02-29 19:53:45.015369 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/_logs.py
--rw-r--r--   0        0        0     1909 2024-02-29 19:53:45.015442 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2024-02-29 19:53:45.015505 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2024-02-29 19:53:45.015577 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/_sync.py
--rw-r--r--   0        0        0     7223 2024-02-29 19:53:45.015668 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2024-02-29 19:53:45.015750 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/_typing.py
--rw-r--r--   0        0        0    11105 2024-02-29 19:53:45.015855 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/_utils.py
--rw-r--r--   0        0        0      126 2024-02-29 19:53:45.015929 notdiamond-0.1.0a8/notdiamond/openai/src/openai/_version.py
--rw-r--r--   0        0        0       31 2024-02-29 19:53:45.016028 notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/__init__.py
--rw-r--r--   0        0        0       58 2024-02-29 19:53:45.016128 notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/_api/__init__.py
--rw-r--r--   0        0        0      451 2024-02-29 19:53:45.016199 notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/_api/_main.py
--rw-r--r--   0        0        0     3347 2024-02-29 19:53:45.016267 notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/_api/audio.py
--rw-r--r--   0        0        0      300 2024-02-29 19:53:45.016373 notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/_api/chat/__init__.py
--rw-r--r--   0        0        0     5363 2024-02-29 19:53:45.016452 notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/_api/chat/completions.py
--rw-r--r--   0        0        0     6412 2024-02-29 19:53:45.016539 notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/_api/completions.py
--rw-r--r--   0        0        0     2345 2024-02-29 19:53:45.016605 notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/_api/files.py
--rw-r--r--   0        0        0     5062 2024-02-29 19:53:45.016661 notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/_api/image.py
--rw-r--r--   0        0        0     1295 2024-02-29 19:53:45.016728 notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/_api/models.py
--rw-r--r--   0        0        0     6743 2024-02-29 19:53:45.016813 notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/_cli.py
--rw-r--r--   0        0        0      479 2024-02-29 19:53:45.016883 notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/_errors.py
--rw-r--r--   0        0        0      491 2024-02-29 19:53:45.016949 notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/_models.py
--rw-r--r--   0        0        0     1406 2024-02-29 19:53:45.017526 notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/_progress.py
--rw-r--r--   0        0        0       58 2024-02-29 19:53:45.017760 notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/_tools/__init__.py
--rw-r--r--   0        0        0      467 2024-02-29 19:53:45.017856 notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/_tools/_main.py
--rw-r--r--   0        0        0     1543 2024-02-29 19:53:45.017933 notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/_tools/fine_tunes.py
--rw-r--r--   0        0        0     4910 2024-02-29 19:53:45.018022 notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/_tools/migrate.py
--rw-r--r--   0        0        0      848 2024-02-29 19:53:45.018096 notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/_utils.py
--rw-r--r--   0        0        0      224 2024-02-29 19:53:45.018213 notdiamond-0.1.0a8/notdiamond/openai/src/openai/lib/.keep
--rw-r--r--   0        0        0     2384 2024-02-29 20:11:49.021843 notdiamond-0.1.0a8/notdiamond/openai/src/openai/lib/__pycache__/_old_api.cpython-310.pyc
--rw-r--r--   0        0        0    12573 2024-02-29 20:11:49.020116 notdiamond-0.1.0a8/notdiamond/openai/src/openai/lib/__pycache__/azure.cpython-310.pyc
--rw-r--r--   0        0        0     1947 2024-02-29 19:53:45.018335 notdiamond-0.1.0a8/notdiamond/openai/src/openai/lib/_old_api.py
--rw-r--r--   0        0        0    35189 2024-02-29 19:53:45.018585 notdiamond-0.1.0a8/notdiamond/openai/src/openai/lib/_validators.py
--rw-r--r--   0        0        0    21021 2024-02-29 19:53:45.018707 notdiamond-0.1.0a8/notdiamond/openai/src/openai/lib/azure.py
--rw-r--r--   0        0        0     2727 2024-02-29 19:53:45.018801 notdiamond-0.1.0a8/notdiamond/openai/src/openai/pagination.py
--rw-r--r--   0        0        0        0 2024-02-29 19:53:45.018833 notdiamond-0.1.0a8/notdiamond/openai/src/openai/py.typed
--rw-r--r--   0        0        0     3766 2024-02-29 19:53:45.018942 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/__init__.py
--rw-r--r--   0        0        0     2704 2024-02-29 20:11:45.327645 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    21296 2024-02-29 20:11:49.004989 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/__pycache__/completions.cpython-310.pyc
--rw-r--r--   0        0        0     7113 2024-02-29 20:11:49.000033 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/__pycache__/embeddings.cpython-310.pyc
--rw-r--r--   0        0        0    11879 2024-02-29 20:11:48.995302 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/__pycache__/files.cpython-310.pyc
--rw-r--r--   0        0        0    11992 2024-02-29 20:11:48.997626 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/__pycache__/images.cpython-310.pyc
--rw-r--r--   0        0        0     5940 2024-02-29 20:11:48.998933 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/__pycache__/models.cpython-310.pyc
--rw-r--r--   0        0        0     5188 2024-02-29 20:11:49.016748 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/__pycache__/moderations.cpython-310.pyc
--rw-r--r--   0        0        0     1654 2024-02-29 19:53:45.019052 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/audio/__init__.py
--rw-r--r--   0        0        0     1282 2024-02-29 20:11:48.984278 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/audio/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5750 2024-02-29 20:11:48.985376 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/audio/__pycache__/audio.cpython-310.pyc
--rw-r--r--   0        0        0     5952 2024-02-29 20:11:48.986309 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/audio/__pycache__/speech.cpython-310.pyc
--rw-r--r--   0        0        0     7001 2024-02-29 20:11:48.993205 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/audio/__pycache__/transcriptions.cpython-310.pyc
--rw-r--r--   0        0        0     6145 2024-02-29 20:11:48.992132 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/audio/__pycache__/translations.cpython-310.pyc
--rw-r--r--   0        0        0     4448 2024-02-29 19:53:45.019137 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/audio/audio.py
--rw-r--r--   0        0        0     8179 2024-02-29 19:53:45.019228 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/audio/speech.py
--rw-r--r--   0        0        0    10601 2024-02-29 19:53:45.019321 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/audio/transcriptions.py
--rw-r--r--   0        0        0     8805 2024-02-29 19:53:45.019419 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/audio/translations.py
--rw-r--r--   0        0        0     1170 2024-02-29 19:53:45.019595 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/__init__.py
--rw-r--r--   0        0        0      972 2024-02-29 20:11:45.328248 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4669 2024-02-29 20:11:45.329098 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/__pycache__/beta.cpython-310.pyc
--rw-r--r--   0        0        0      816 2024-02-29 19:53:45.019705 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/assistants/__init__.py
--rw-r--r--   0        0        0      744 2024-02-29 20:11:45.420692 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/assistants/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    14914 2024-02-29 20:11:45.429546 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/assistants/__pycache__/assistants.cpython-310.pyc
--rw-r--r--   0        0        0     9460 2024-02-29 20:11:45.422404 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/assistants/__pycache__/files.cpython-310.pyc
--rw-r--r--   0        0        0    30627 2024-02-29 19:53:45.019797 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/assistants/assistants.py
--rw-r--r--   0        0        0    19432 2024-02-29 19:53:45.019906 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/assistants/files.py
--rw-r--r--   0        0        0     3340 2024-02-29 19:53:45.019995 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/beta.py
--rw-r--r--   0        0        0     1144 2024-02-29 19:53:45.020117 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/__init__.py
--rw-r--r--   0        0        0      966 2024-02-29 20:11:45.329523 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    13265 2024-02-29 20:11:45.413040 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/__pycache__/threads.cpython-310.pyc
--rw-r--r--   0        0        0      790 2024-02-29 19:53:45.020219 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/messages/__init__.py
--rw-r--r--   0        0        0      736 2024-02-29 20:11:45.413614 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/messages/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7304 2024-02-29 20:11:45.414945 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/messages/__pycache__/files.cpython-310.pyc
--rw-r--r--   0        0        0    12033 2024-02-29 20:11:45.419920 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/messages/__pycache__/messages.cpython-310.pyc
--rw-r--r--   0        0        0    12267 2024-02-29 19:53:45.020290 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/messages/files.py
--rw-r--r--   0        0        0    22831 2024-02-29 19:53:45.020400 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/messages/messages.py
--rw-r--r--   0        0        0      738 2024-02-29 19:53:45.020508 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/runs/__init__.py
--rw-r--r--   0        0        0      704 2024-02-29 20:11:45.330150 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/runs/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    15291 2024-02-29 20:11:45.332650 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/runs/__pycache__/runs.cpython-310.pyc
--rw-r--r--   0        0        0     7279 2024-02-29 20:11:45.339076 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/runs/__pycache__/steps.cpython-310.pyc
--rw-r--r--   0        0        0    32278 2024-02-29 19:53:45.020714 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/runs/runs.py
--rw-r--r--   0        0        0    12141 2024-02-29 19:53:45.021178 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/runs/steps.py
--rw-r--r--   0        0        0    25273 2024-02-29 19:53:45.021761 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/threads.py
--rw-r--r--   0        0        0      816 2024-02-29 19:53:45.022037 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/chat/__init__.py
--rw-r--r--   0        0        0      733 2024-02-29 20:11:45.430464 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/chat/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3541 2024-02-29 20:11:45.431163 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/chat/__pycache__/chat.cpython-310.pyc
--rw-r--r--   0        0        0    26512 2024-02-29 20:11:45.434914 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/chat/__pycache__/completions.cpython-310.pyc
--rw-r--r--   0        0        0     2309 2024-02-29 19:53:45.022177 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/chat/chat.py
--rw-r--r--   0        0        0    71495 2024-02-29 20:05:02.015985 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/chat/completions.py
--rw-r--r--   0        0        0    56586 2024-02-29 19:53:45.022511 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/completions.py
--rw-r--r--   0        0        0    10677 2024-02-29 19:53:45.022614 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/embeddings.py
--rw-r--r--   0        0        0    26000 2024-02-29 19:53:45.022763 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/files.py
--rw-r--r--   0        0        0      804 2024-02-29 19:53:45.022894 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/fine_tuning/__init__.py
--rw-r--r--   0        0        0      734 2024-02-29 20:11:49.005802 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/fine_tuning/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3598 2024-02-29 20:11:49.015690 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/fine_tuning/__pycache__/fine_tuning.cpython-310.pyc
--rw-r--r--   0        0        0    11568 2024-02-29 20:11:49.007415 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/fine_tuning/__pycache__/jobs.cpython-310.pyc
--rw-r--r--   0        0        0     2338 2024-02-29 19:53:45.022980 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/fine_tuning/fine_tuning.py
--rw-r--r--   0        0        0    24455 2024-02-29 19:53:45.023095 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/fine_tuning/jobs.py
--rw-r--r--   0        0        0    24159 2024-02-29 19:53:45.023190 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/images.py
--rw-r--r--   0        0        0    10150 2024-02-29 19:53:45.023295 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/models.py
--rw-r--r--   0        0        0     6576 2024-02-29 19:53:45.023376 notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/moderations.py
--rw-r--r--   0        0        0     1629 2024-02-29 19:53:45.023494 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__init__.py
--rw-r--r--   0        0        0     1571 2024-02-29 20:11:45.268720 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      915 2024-02-29 20:11:45.297816 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/completion.cpython-310.pyc
--rw-r--r--   0        0        0     1078 2024-02-29 20:11:45.299574 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/completion_choice.cpython-310.pyc
--rw-r--r--   0        0        0     1774 2024-02-29 20:11:45.319155 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/completion_create_params.cpython-310.pyc
--rw-r--r--   0        0        0      546 2024-02-29 20:11:45.298210 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/completion_usage.cpython-310.pyc
--rw-r--r--   0        0        0      930 2024-02-29 20:11:45.320379 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/create_embedding_response.cpython-310.pyc
--rw-r--r--   0        0        0      625 2024-02-29 20:11:45.296413 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/embedding.cpython-310.pyc
--rw-r--r--   0        0        0      980 2024-02-29 20:11:45.318291 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/embedding_create_params.cpython-310.pyc
--rw-r--r--   0        0        0      249 2024-02-29 20:11:45.311226 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/file_content.cpython-310.pyc
--rw-r--r--   0        0        0      716 2024-02-29 20:11:45.316491 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/file_create_params.cpython-310.pyc
--rw-r--r--   0        0        0      576 2024-02-29 20:11:45.311648 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/file_deleted.cpython-310.pyc
--rw-r--r--   0        0        0      548 2024-02-29 20:11:45.314820 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/file_list_params.cpython-310.pyc
--rw-r--r--   0        0        0      864 2024-02-29 20:11:45.308677 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/file_object.cpython-310.pyc
--rw-r--r--   0        0        0      596 2024-02-29 20:11:45.269260 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/image.cpython-310.pyc
--rw-r--r--   0        0        0      984 2024-02-29 20:11:45.323781 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/image_create_variation_params.cpython-310.pyc
--rw-r--r--   0        0        0     1023 2024-02-29 20:11:45.315787 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/image_edit_params.cpython-310.pyc
--rw-r--r--   0        0        0     1067 2024-02-29 20:11:45.317221 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/image_generate_params.cpython-310.pyc
--rw-r--r--   0        0        0      585 2024-02-29 20:11:45.313551 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/images_response.cpython-310.pyc
--rw-r--r--   0        0        0      597 2024-02-29 20:11:45.292767 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/model.cpython-310.pyc
--rw-r--r--   0        0        0      509 2024-02-29 20:11:45.312680 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/model_deleted.cpython-310.pyc
--rw-r--r--   0        0        0     1643 2024-02-29 20:11:45.305031 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/moderation.cpython-310.pyc
--rw-r--r--   0        0        0      772 2024-02-29 20:11:45.319920 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/moderation_create_params.cpython-310.pyc
--rw-r--r--   0        0        0      641 2024-02-29 20:11:45.322148 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/moderation_create_response.cpython-310.pyc
--rw-r--r--   0        0        0      461 2024-02-29 19:53:45.023613 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/audio/__init__.py
--rw-r--r--   0        0        0      572 2024-02-29 20:11:48.986811 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/audio/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      921 2024-02-29 20:11:48.989899 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/audio/__pycache__/speech_create_params.cpython-310.pyc
--rw-r--r--   0        0        0      475 2024-02-29 20:11:48.988110 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/audio/__pycache__/transcription.cpython-310.pyc
--rw-r--r--   0        0        0     1031 2024-02-29 20:11:48.991006 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/audio/__pycache__/transcription_create_params.cpython-310.pyc
--rw-r--r--   0        0        0      471 2024-02-29 20:11:48.987131 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/audio/__pycache__/translation.cpython-310.pyc
--rw-r--r--   0        0        0      860 2024-02-29 20:11:48.990535 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/audio/__pycache__/translation_create_params.cpython-310.pyc
--rw-r--r--   0        0        0     1417 2024-02-29 19:53:45.023701 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/audio/speech_create_params.py
--rw-r--r--   0        0        0      164 2024-02-29 19:53:45.023771 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/audio/transcription.py
--rw-r--r--   0        0        0     2018 2024-02-29 19:53:45.023855 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/audio/transcription_create_params.py
--rw-r--r--   0        0        0      160 2024-02-29 19:53:45.023924 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/audio/translation.py
--rw-r--r--   0        0        0     1404 2024-02-29 19:53:45.024012 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/audio/translation_create_params.py
--rw-r--r--   0        0        0      791 2024-02-29 19:53:45.024141 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/__init__.py
--rw-r--r--   0        0        0      856 2024-02-29 20:11:45.360292 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1541 2024-02-29 20:11:45.362441 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/__pycache__/assistant.cpython-310.pyc
--rw-r--r--   0        0        0     1635 2024-02-29 20:11:45.370165 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/__pycache__/assistant_create_params.cpython-310.pyc
--rw-r--r--   0        0        0      604 2024-02-29 20:11:45.367009 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/__pycache__/assistant_deleted.cpython-310.pyc
--rw-r--r--   0        0        0      672 2024-02-29 20:11:45.369553 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/__pycache__/assistant_list_params.cpython-310.pyc
--rw-r--r--   0        0        0     1625 2024-02-29 20:11:45.372373 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/__pycache__/assistant_update_params.cpython-310.pyc
--rw-r--r--   0        0        0      670 2024-02-29 20:11:45.360954 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/__pycache__/thread.cpython-310.pyc
--rw-r--r--   0        0        0     2102 2024-02-29 20:11:45.373247 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/__pycache__/thread_create_and_run_params.cpython-310.pyc
--rw-r--r--   0        0        0     1001 2024-02-29 20:11:45.368488 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/__pycache__/thread_create_params.cpython-310.pyc
--rw-r--r--   0        0        0      595 2024-02-29 20:11:45.365775 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/__pycache__/thread_deleted.cpython-310.pyc
--rw-r--r--   0        0        0      614 2024-02-29 20:11:45.369105 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/__pycache__/thread_update_params.cpython-310.pyc
--rw-r--r--   0        0        0     2562 2024-02-29 19:53:45.024233 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/assistant.py
--rw-r--r--   0        0        0     2553 2024-02-29 19:53:45.024320 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/assistant_create_params.py
--rw-r--r--   0        0        0      268 2024-02-29 19:53:45.024389 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/assistant_deleted.py
--rw-r--r--   0        0        0     1187 2024-02-29 19:53:45.024491 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/assistant_list_params.py
--rw-r--r--   0        0        0     2670 2024-02-29 19:53:45.024575 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/assistant_update_params.py
--rw-r--r--   0        0        0      356 2024-02-29 19:53:45.024684 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/assistants/__init__.py
--rw-r--r--   0        0        0      500 2024-02-29 20:11:45.423086 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/assistants/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      646 2024-02-29 20:11:45.423638 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/assistants/__pycache__/assistant_file.cpython-310.pyc
--rw-r--r--   0        0        0      597 2024-02-29 20:11:45.426218 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/assistants/__pycache__/file_create_params.cpython-310.pyc
--rw-r--r--   0        0        0      625 2024-02-29 20:11:45.426764 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/assistants/__pycache__/file_delete_response.cpython-310.pyc
--rw-r--r--   0        0        0      673 2024-02-29 20:11:45.424945 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/assistants/__pycache__/file_list_params.cpython-310.pyc
--rw-r--r--   0        0        0      554 2024-02-29 19:53:45.024753 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/assistants/assistant_file.py
--rw-r--r--   0        0        0      484 2024-02-29 19:53:45.024832 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/assistants/file_create_params.py
--rw-r--r--   0        0        0      278 2024-02-29 19:53:45.024898 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/assistants/file_delete_response.py
--rw-r--r--   0        0        0     1177 2024-02-29 19:53:45.024959 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/assistants/file_list_params.py
--rw-r--r--   0        0        0       89 2024-02-29 19:53:45.025061 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/chat/__init__.py
--rw-r--r--   0        0        0      781 2024-02-29 19:53:45.025134 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/thread.py
--rw-r--r--   0        0        0     3740 2024-02-29 19:53:45.025222 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/thread_create_and_run_params.py
--rw-r--r--   0        0        0     1631 2024-02-29 19:53:45.025720 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/thread_create_params.py
--rw-r--r--   0        0        0      259 2024-02-29 19:53:45.025931 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/thread_deleted.py
--rw-r--r--   0        0        0      554 2024-02-29 19:53:45.026023 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/thread_update_params.py
--rw-r--r--   0        0        0     1024 2024-02-29 19:53:45.026152 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/__init__.py
--rw-r--r--   0        0        0     1060 2024-02-29 20:11:45.374444 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      764 2024-02-29 20:11:45.389323 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/__pycache__/message_content_image_file.cpython-310.pyc
--rw-r--r--   0        0        0     1762 2024-02-29 20:11:45.385099 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/__pycache__/message_content_text.cpython-310.pyc
--rw-r--r--   0        0        0      796 2024-02-29 20:11:45.395433 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/__pycache__/message_create_params.cpython-310.pyc
--rw-r--r--   0        0        0      676 2024-02-29 20:11:45.394972 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/__pycache__/message_list_params.cpython-310.pyc
--rw-r--r--   0        0        0      679 2024-02-29 20:11:45.395851 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/__pycache__/message_update_params.cpython-310.pyc
--rw-r--r--   0        0        0      825 2024-02-29 20:11:45.376715 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/__pycache__/required_action_function_tool_call.cpython-310.pyc
--rw-r--r--   0        0        0     2920 2024-02-29 20:11:45.375228 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/__pycache__/run.cpython-310.pyc
--rw-r--r--   0        0        0     1611 2024-02-29 20:11:45.393982 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/__pycache__/run_create_params.cpython-310.pyc
--rw-r--r--   0        0        0      668 2024-02-29 20:11:45.393164 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/__pycache__/run_list_params.cpython-310.pyc
--rw-r--r--   0        0        0      406 2024-02-29 20:11:45.375713 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/__pycache__/run_status.cpython-310.pyc
--rw-r--r--   0        0        0      900 2024-02-29 20:11:45.396247 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/__pycache__/run_submit_tool_outputs_params.cpython-310.pyc
--rw-r--r--   0        0        0      671 2024-02-29 20:11:45.394565 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/__pycache__/run_update_params.cpython-310.pyc
--rw-r--r--   0        0        0     1113 2024-02-29 20:11:45.383874 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/__pycache__/thread_message.cpython-310.pyc
--rw-r--r--   0        0        0      489 2024-02-29 19:53:45.026231 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/message_content_image_file.py
--rw-r--r--   0        0        0     1575 2024-02-29 19:53:45.026301 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/message_content_text.py
--rw-r--r--   0        0        0     1100 2024-02-29 19:53:45.026379 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/message_create_params.py
--rw-r--r--   0        0        0     1183 2024-02-29 19:53:45.026446 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/message_list_params.py
--rw-r--r--   0        0        0      596 2024-02-29 19:53:45.026506 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/message_update_params.py
--rw-r--r--   0        0        0      206 2024-02-29 19:53:45.026620 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/messages/__init__.py
--rw-r--r--   0        0        0      380 2024-02-29 20:11:45.415542 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/messages/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      734 2024-02-29 20:11:45.417400 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/messages/__pycache__/file_list_params.cpython-310.pyc
--rw-r--r--   0        0        0      651 2024-02-29 20:11:45.416061 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/messages/__pycache__/message_file.cpython-310.pyc
--rw-r--r--   0        0        0     1217 2024-02-29 19:53:45.026682 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/messages/file_list_params.py
--rw-r--r--   0        0        0      695 2024-02-29 19:53:45.026746 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/messages/message_file.py
--rw-r--r--   0        0        0      855 2024-02-29 19:53:45.026839 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/required_action_function_tool_call.py
--rw-r--r--   0        0        0     4902 2024-02-29 19:53:45.026924 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/run.py
--rw-r--r--   0        0        0     2520 2024-02-29 19:53:45.027003 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/run_create_params.py
--rw-r--r--   0        0        0     1175 2024-02-29 19:53:45.027079 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/run_list_params.py
--rw-r--r--   0        0        0      249 2024-02-29 19:53:45.027160 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/run_status.py
--rw-r--r--   0        0        0      727 2024-02-29 19:53:45.027231 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/run_submit_tool_outputs_params.py
--rw-r--r--   0        0        0      588 2024-02-29 19:53:45.027299 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/run_update_params.py
--rw-r--r--   0        0        0      574 2024-02-29 19:53:45.027419 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/__init__.py
--rw-r--r--   0        0        0      687 2024-02-29 20:11:45.396681 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1542 2024-02-29 20:11:45.397989 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/code_tool_call.cpython-310.pyc
--rw-r--r--   0        0        0      879 2024-02-29 20:11:45.401406 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/function_tool_call.cpython-310.pyc
--rw-r--r--   0        0        0      790 2024-02-29 20:11:45.405146 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/message_creation_step_details.cpython-310.pyc
--rw-r--r--   0        0        0      613 2024-02-29 20:11:45.403185 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/retrieval_tool_call.cpython-310.pyc
--rw-r--r--   0        0        0     1870 2024-02-29 20:11:45.397189 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/run_step.cpython-310.pyc
--rw-r--r--   0        0        0      730 2024-02-29 20:11:45.410682 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/step_list_params.cpython-310.pyc
--rw-r--r--   0        0        0      864 2024-02-29 20:11:45.397532 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/tool_calls_step_details.cpython-310.pyc
--rw-r--r--   0        0        0     1632 2024-02-29 19:53:45.027543 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/code_tool_call.py
--rw-r--r--   0        0        0      887 2024-02-29 19:53:45.027644 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/function_tool_call.py
--rw-r--r--   0        0        0      473 2024-02-29 19:53:45.027736 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/message_creation_step_details.py
--rw-r--r--   0        0        0      481 2024-02-29 19:53:45.027816 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/retrieval_tool_call.py
--rw-r--r--   0        0        0     3312 2024-02-29 19:53:45.027927 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/run_step.py
--rw-r--r--   0        0        0     1217 2024-02-29 19:53:45.027999 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/step_list_params.py
--rw-r--r--   0        0        0      736 2024-02-29 19:53:45.028067 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/tool_calls_step_details.py
--rw-r--r--   0        0        0     2057 2024-02-29 19:53:45.028136 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/thread_message.py
--rw-r--r--   0        0        0     2431 2024-02-29 19:53:45.028280 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__init__.py
--rw-r--r--   0        0        0     2057 2024-02-29 20:11:48.950251 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1583 2024-02-29 20:11:48.951224 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion.cpython-310.pyc
--rw-r--r--   0        0        0     1181 2024-02-29 20:11:48.981137 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_assistant_message_param.cpython-310.pyc
--rw-r--r--   0        0        0     2474 2024-02-29 20:11:48.967167 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_chunk.cpython-310.pyc
--rw-r--r--   0        0        0      918 2024-02-29 20:11:48.978609 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_content_part_image_param.cpython-310.pyc
--rw-r--r--   0        0        0      588 2024-02-29 20:11:48.977892 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_content_part_param.cpython-310.pyc
--rw-r--r--   0        0        0      687 2024-02-29 20:11:48.978201 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_content_part_text_param.cpython-310.pyc
--rw-r--r--   0        0        0      628 2024-02-29 20:11:48.982841 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_function_call_option_param.cpython-310.pyc
--rw-r--r--   0        0        0      777 2024-02-29 20:11:48.980319 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_function_message_param.cpython-310.pyc
--rw-r--r--   0        0        0     1052 2024-02-29 20:11:48.952840 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_message.cpython-310.pyc
--rw-r--r--   0        0        0      868 2024-02-29 20:11:48.976682 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_message_param.cpython-310.pyc
--rw-r--r--   0        0        0      815 2024-02-29 20:11:48.954109 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_message_tool_call.cpython-310.pyc
--rw-r--r--   0        0        0      913 2024-02-29 20:11:48.981593 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_message_tool_call_param.cpython-310.pyc
--rw-r--r--   0        0        0      861 2024-02-29 20:11:48.982420 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_named_tool_choice_param.cpython-310.pyc
--rw-r--r--   0        0        0      365 2024-02-29 20:11:48.966307 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_role.cpython-310.pyc
--rw-r--r--   0        0        0      712 2024-02-29 20:11:48.979205 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_system_message_param.cpython-310.pyc
--rw-r--r--   0        0        0      929 2024-02-29 20:11:48.958374 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_token_logprob.cpython-310.pyc
--rw-r--r--   0        0        0      566 2024-02-29 20:11:48.982102 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_tool_choice_option_param.cpython-310.pyc
--rw-r--r--   0        0        0      709 2024-02-29 20:11:48.977112 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_tool_message_param.cpython-310.pyc
--rw-r--r--   0        0        0      744 2024-02-29 20:11:48.976072 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_tool_param.cpython-310.pyc
--rw-r--r--   0        0        0      904 2024-02-29 20:11:48.977567 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_user_message_param.cpython-310.pyc
--rw-r--r--   0        0        0     3056 2024-02-29 20:11:48.975542 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/completion_create_params.cpython-310.pyc
--rw-r--r--   0        0        0     2288 2024-02-29 19:53:45.028388 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion.py
--rw-r--r--   0        0        0     1605 2024-02-29 19:53:45.028458 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_assistant_message_param.py
--rw-r--r--   0        0        0     4062 2024-02-29 19:53:45.028534 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_chunk.py
--rw-r--r--   0        0        0      764 2024-02-29 19:53:45.028616 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_content_part_image_param.py
--rw-r--r--   0        0        0      453 2024-02-29 19:53:45.028757 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_content_part_param.py
--rw-r--r--   0        0        0      396 2024-02-29 19:53:45.028828 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_content_part_text_param.py
--rw-r--r--   0        0        0      332 2024-02-29 19:53:45.028900 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_function_call_option_param.py
--rw-r--r--   0        0        0      558 2024-02-29 19:53:45.028982 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_function_message_param.py
--rw-r--r--   0        0        0     1249 2024-02-29 19:53:45.029056 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_message.py
--rw-r--r--   0        0        0      805 2024-02-29 19:53:45.029280 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_message_param.py
--rw-r--r--   0        0        0      867 2024-02-29 19:53:45.029390 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_message_tool_call.py
--rw-r--r--   0        0        0      976 2024-02-29 19:53:45.029472 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_message_tool_call_param.py
--rw-r--r--   0        0        0      536 2024-02-29 19:53:45.029558 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_named_tool_choice_param.py
--rw-r--r--   0        0        0      207 2024-02-29 19:53:45.029628 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_role.py
--rw-r--r--   0        0        0      605 2024-02-29 19:53:45.029701 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_system_message_param.py
--rw-r--r--   0        0        0     1440 2024-02-29 19:53:45.029779 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_token_logprob.py
--rw-r--r--   0        0        0      399 2024-02-29 19:53:45.029842 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_tool_choice_option_param.py
--rw-r--r--   0        0        0      520 2024-02-29 19:53:45.029912 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_tool_message_param.py
--rw-r--r--   0        0        0      452 2024-02-29 19:53:45.029988 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_tool_param.py
--rw-r--r--   0        0        0      759 2024-02-29 19:53:45.030069 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_user_message_param.py
--rw-r--r--   0        0        0    10599 2024-02-29 19:53:45.030179 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/completion_create_params.py
--rw-r--r--   0        0        0     1139 2024-02-29 19:53:45.030297 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/completion.py
--rw-r--r--   0        0        0      932 2024-02-29 19:53:45.030410 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/completion_choice.py
--rw-r--r--   0        0        0     7223 2024-02-29 19:53:45.030573 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/completion_create_params.py
--rw-r--r--   0        0        0      401 2024-02-29 19:53:45.030763 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/completion_usage.py
--rw-r--r--   0        0        0      765 2024-02-29 19:53:45.030878 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/create_embedding_response.py
--rw-r--r--   0        0        0      604 2024-02-29 19:53:45.030960 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/embedding.py
--rw-r--r--   0        0        0     1852 2024-02-29 19:53:45.031044 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/embedding_create_params.py
--rw-r--r--   0        0        0      100 2024-02-29 19:53:45.031116 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/file_content.py
--rw-r--r--   0        0        0      840 2024-02-29 19:53:45.031201 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/file_create_params.py
--rw-r--r--   0        0        0      244 2024-02-29 19:53:45.031283 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/file_deleted.py
--rw-r--r--   0        0        0      277 2024-02-29 19:53:45.031367 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/file_list_params.py
--rw-r--r--   0        0        0     1193 2024-02-29 19:53:45.031461 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/file_object.py
--rw-r--r--   0        0        0      431 2024-02-29 19:53:45.031698 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/fine_tuning/__init__.py
--rw-r--r--   0        0        0      560 2024-02-29 20:11:49.007978 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/fine_tuning/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1598 2024-02-29 20:11:49.008618 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/fine_tuning/__pycache__/fine_tuning_job.cpython-310.pyc
--rw-r--r--   0        0        0      684 2024-02-29 20:11:49.013635 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/fine_tuning/__pycache__/fine_tuning_job_event.cpython-310.pyc
--rw-r--r--   0        0        0     1160 2024-02-29 20:11:49.012393 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/fine_tuning/__pycache__/job_create_params.cpython-310.pyc
--rw-r--r--   0        0        0      595 2024-02-29 20:11:49.014930 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/fine_tuning/__pycache__/job_list_events_params.cpython-310.pyc
--rw-r--r--   0        0        0      582 2024-02-29 20:11:49.011903 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/fine_tuning/__pycache__/job_list_params.cpython-310.pyc
--rw-r--r--   0        0        0     3312 2024-02-29 19:53:45.031854 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/fine_tuning/fine_tuning_job.py
--rw-r--r--   0        0        0      341 2024-02-29 19:53:45.031945 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/fine_tuning/fine_tuning_job_event.py
--rw-r--r--   0        0        0     2578 2024-02-29 19:53:45.032060 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/fine_tuning/job_create_params.py
--rw-r--r--   0        0        0      367 2024-02-29 19:53:45.032160 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/fine_tuning/job_list_events_params.py
--rw-r--r--   0        0        0      363 2024-02-29 19:53:45.032229 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/fine_tuning/job_list_params.py
--rw-r--r--   0        0        0      574 2024-02-29 19:53:45.032319 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/image.py
--rw-r--r--   0        0        0     1342 2024-02-29 19:53:45.032411 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/image_create_variation_params.py
--rw-r--r--   0        0        0     1702 2024-02-29 19:53:45.032482 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/image_edit_params.py
--rw-r--r--   0        0        0     2008 2024-02-29 19:53:45.032563 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/image_generate_params.py
--rw-r--r--   0        0        0      241 2024-02-29 19:53:45.032629 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/images_response.py
--rw-r--r--   0        0        0      499 2024-02-29 19:53:45.032733 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/model.py
--rw-r--r--   0        0        0      195 2024-02-29 19:53:45.032829 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/model_deleted.py
--rw-r--r--   0        0        0     3946 2024-02-29 19:53:45.032928 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/moderation.py
--rw-r--r--   0        0        0      921 2024-02-29 19:53:45.033016 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/moderation_create_params.py
--rw-r--r--   0        0        0      451 2024-02-29 19:53:45.033086 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/moderation_create_response.py
--rw-r--r--   0        0        0      202 2024-02-29 19:53:45.033209 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/shared/__init__.py
--rw-r--r--   0        0        0      335 2024-02-29 20:11:45.294228 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/shared/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      689 2024-02-29 20:11:45.294720 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/shared/__pycache__/function_definition.cpython-310.pyc
--rw-r--r--   0        0        0      326 2024-02-29 20:11:45.295085 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/shared/__pycache__/function_parameters.cpython-310.pyc
--rw-r--r--   0        0        0     1034 2024-02-29 19:53:45.033313 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/shared/function_definition.py
--rw-r--r--   0        0        0      152 2024-02-29 19:53:45.033381 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/shared/function_parameters.py
--rw-r--r--   0        0        0      202 2024-02-29 19:53:45.033475 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/shared_params/__init__.py
--rw-r--r--   0        0        0      342 2024-02-29 20:11:45.370593 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/shared_params/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      735 2024-02-29 20:11:45.371046 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/shared_params/__pycache__/function_definition.cpython-310.pyc
--rw-r--r--   0        0        0      379 2024-02-29 20:11:45.371530 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/shared_params/__pycache__/function_parameters.cpython-310.pyc
--rw-r--r--   0        0        0     1045 2024-02-29 19:53:45.033543 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/shared_params/function_definition.py
--rw-r--r--   0        0        0      188 2024-02-29 19:53:45.033602 notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/shared_params/function_parameters.py
--rw-r--r--   0        0        0       62 2024-02-29 19:53:45.034068 notdiamond-0.1.0a8/notdiamond/openai/src/openai/version.py
--rw-r--r--   0        0        0       53 2024-02-29 19:53:45.034185 notdiamond-0.1.0a8/notdiamond/openai/tests/__init__.py
--rw-r--r--   0        0        0      193 2024-03-01 15:43:17.169340 notdiamond-0.1.0a8/notdiamond/openai/tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1900 2024-03-01 15:43:17.171904 notdiamond-0.1.0a8/notdiamond/openai/tests/__pycache__/conftest.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0    55728 2024-03-01 15:43:17.978233 notdiamond-0.1.0a8/notdiamond/openai/tests/__pycache__/test_client.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0     3181 2024-03-01 15:43:17.999785 notdiamond-0.1.0a8/notdiamond/openai/tests/__pycache__/test_deepcopy.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0     4422 2024-03-01 15:43:18.006049 notdiamond-0.1.0a8/notdiamond/openai/tests/__pycache__/test_extract_files.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0     4055 2024-03-01 15:43:18.010620 notdiamond-0.1.0a8/notdiamond/openai/tests/__pycache__/test_files.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0     3161 2024-03-01 15:43:18.016784 notdiamond-0.1.0a8/notdiamond/openai/tests/__pycache__/test_legacy_response.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0    56374 2024-03-01 15:43:18.078942 notdiamond-0.1.0a8/notdiamond/openai/tests/__pycache__/test_models.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0    13057 2024-03-01 15:43:18.148960 notdiamond-0.1.0a8/notdiamond/openai/tests/__pycache__/test_module_client.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0     8287 2024-03-01 15:43:18.169284 notdiamond-0.1.0a8/notdiamond/openai/tests/__pycache__/test_qs.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0     7371 2024-03-01 15:43:18.176395 notdiamond-0.1.0a8/notdiamond/openai/tests/__pycache__/test_required_args.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0     8431 2024-03-01 15:43:18.183627 notdiamond-0.1.0a8/notdiamond/openai/tests/__pycache__/test_response.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0     6263 2024-03-01 15:43:18.194766 notdiamond-0.1.0a8/notdiamond/openai/tests/__pycache__/test_streaming.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0    23550 2024-03-01 15:43:18.218793 notdiamond-0.1.0a8/notdiamond/openai/tests/__pycache__/test_transform.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0       53 2024-02-29 19:53:45.034297 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/__init__.py
--rw-r--r--   0        0        0      207 2024-03-01 15:43:17.178166 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    11419 2024-03-01 15:43:17.729416 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/__pycache__/test_completions.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0     6349 2024-03-01 15:43:17.740226 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/__pycache__/test_embeddings.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0    25185 2024-03-01 15:43:17.773350 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/__pycache__/test_files.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0    12139 2024-03-01 15:43:17.795628 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/__pycache__/test_images.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0    11404 2024-03-01 15:43:17.822202 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/__pycache__/test_models.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0     6213 2024-03-01 15:43:17.835417 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/__pycache__/test_moderations.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0       53 2024-02-29 19:53:45.034444 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/audio/__init__.py
--rw-r--r--   0        0        0      213 2024-03-01 15:43:17.178726 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/audio/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     8738 2024-03-01 15:43:17.187953 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/audio/__pycache__/test_speech.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0     6471 2024-03-01 15:43:17.365949 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/audio/__pycache__/test_transcriptions.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0     6363 2024-03-01 15:43:17.376705 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/audio/__pycache__/test_translations.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0     5750 2024-02-29 19:53:45.034582 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/audio/test_speech.py
--rw-r--r--   0        0        0     4391 2024-02-29 19:53:45.034661 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/audio/test_transcriptions.py
--rw-r--r--   0        0        0     4149 2024-02-29 19:53:45.034870 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/audio/test_translations.py
--rw-r--r--   0        0        0       53 2024-02-29 19:53:45.035011 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/__init__.py
--rw-r--r--   0        0        0      212 2024-03-01 15:43:17.383638 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    17950 2024-03-01 15:43:17.434648 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/__pycache__/test_assistants.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0    17770 2024-03-01 15:43:17.465122 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/__pycache__/test_threads.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0       53 2024-02-29 19:53:45.035185 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/assistants/__init__.py
--rw-r--r--   0        0        0      223 2024-03-01 15:43:17.384451 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/assistants/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    16689 2024-03-01 15:43:17.403120 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/assistants/__pycache__/test_files.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0    15388 2024-02-29 19:53:45.035303 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/assistants/test_files.py
--rw-r--r--   0        0        0       53 2024-02-29 19:53:45.035415 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/chat/__init__.py
--rw-r--r--   0        0        0    17298 2024-02-29 19:53:45.035495 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/test_assistants.py
--rw-r--r--   0        0        0    18678 2024-02-29 19:53:45.035624 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/test_threads.py
--rw-r--r--   0        0        0       53 2024-02-29 19:53:45.035742 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/threads/__init__.py
--rw-r--r--   0        0        0      220 2024-03-01 15:43:17.474843 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/threads/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    17836 2024-03-01 15:43:17.576555 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/threads/__pycache__/test_messages.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0    21240 2024-03-01 15:43:17.615039 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/threads/__pycache__/test_runs.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0       53 2024-02-29 19:53:45.035862 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/threads/messages/__init__.py
--rw-r--r--   0        0        0      229 2024-03-01 15:43:17.475394 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/threads/messages/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    12104 2024-03-01 15:43:17.532189 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/threads/messages/__pycache__/test_files.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0    10298 2024-02-29 19:53:45.035942 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/threads/messages/test_files.py
--rw-r--r--   0        0        0       53 2024-02-29 19:53:45.036163 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/threads/runs/__init__.py
--rw-r--r--   0        0        0      225 2024-03-01 15:43:17.540244 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/threads/runs/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    12015 2024-03-01 15:43:17.549749 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/threads/runs/__pycache__/test_steps.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0     9914 2024-02-29 19:53:45.036293 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/threads/runs/test_steps.py
--rw-r--r--   0        0        0    16951 2024-02-29 19:53:45.036439 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/threads/test_messages.py
--rw-r--r--   0        0        0    24332 2024-02-29 19:53:45.036597 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/threads/test_runs.py
--rw-r--r--   0        0        0       53 2024-02-29 19:53:45.036745 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/chat/__init__.py
--rw-r--r--   0        0        0      212 2024-03-01 15:43:17.626537 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/chat/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    12617 2024-03-01 15:43:17.636395 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/chat/__pycache__/test_completions.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0    15543 2024-02-29 19:53:45.036856 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/chat/test_completions.py
--rw-r--r--   0        0        0       53 2024-02-29 19:53:45.036977 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/fine_tuning/__init__.py
--rw-r--r--   0        0        0      219 2024-03-01 15:43:17.643705 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/fine_tuning/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    20186 2024-03-01 15:43:17.665860 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/fine_tuning/__pycache__/test_jobs.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0    17397 2024-02-29 19:53:45.037119 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/fine_tuning/test_jobs.py
--rw-r--r--   0        0        0     8682 2024-02-29 19:53:45.037231 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/test_completions.py
--rw-r--r--   0        0        0     4469 2024-02-29 19:53:45.037348 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/test_embeddings.py
--rw-r--r--   0        0        0    19256 2024-02-29 19:53:45.037503 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/test_files.py
--rw-r--r--   0        0        0    11122 2024-02-29 19:53:45.037622 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/test_images.py
--rw-r--r--   0        0        0     8691 2024-02-29 19:53:45.037707 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/test_models.py
--rw-r--r--   0        0        0     3862 2024-02-29 19:53:45.037781 notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/test_moderations.py
--rw-r--r--   0        0        0     1425 2024-02-29 19:53:45.037865 notdiamond-0.1.0a8/notdiamond/openai/tests/conftest.py
--rw-r--r--   0        0        0     2773 2024-03-01 15:43:17.842433 notdiamond-0.1.0a8/notdiamond/openai/tests/lib/__pycache__/test_azure.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0      900 2024-03-01 15:43:17.858421 notdiamond-0.1.0a8/notdiamond/openai/tests/lib/__pycache__/test_old_api.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0     1792 2024-02-29 19:53:45.037989 notdiamond-0.1.0a8/notdiamond/openai/tests/lib/test_azure.py
--rw-r--r--   0        0        0      424 2024-02-29 19:53:45.038066 notdiamond-0.1.0a8/notdiamond/openai/tests/lib/test_old_api.py
--rw-r--r--   0        0        0    57182 2024-02-29 19:53:45.038323 notdiamond-0.1.0a8/notdiamond/openai/tests/test_client.py
--rw-r--r--   0        0        0     1564 2024-02-29 19:53:45.038414 notdiamond-0.1.0a8/notdiamond/openai/tests/test_deepcopy.py
--rw-r--r--   0        0        0     1939 2024-02-29 19:53:45.038495 notdiamond-0.1.0a8/notdiamond/openai/tests/test_extract_files.py
--rw-r--r--   0        0        0     1576 2024-02-29 19:53:45.038574 notdiamond-0.1.0a8/notdiamond/openai/tests/test_files.py
--rw-r--r--   0        0        0     1710 2024-02-29 19:53:45.038662 notdiamond-0.1.0a8/notdiamond/openai/tests/test_legacy_response.py
--rw-r--r--   0        0        0    16286 2024-02-29 19:53:45.038772 notdiamond-0.1.0a8/notdiamond/openai/tests/test_models.py
--rw-r--r--   0        0        0     5453 2024-02-29 19:53:45.038852 notdiamond-0.1.0a8/notdiamond/openai/tests/test_module_client.py
--rw-r--r--   0        0        0     3200 2024-02-29 19:53:45.038924 notdiamond-0.1.0a8/notdiamond/openai/tests/test_qs.py
--rw-r--r--   0        0        0     3057 2024-02-29 19:53:45.038999 notdiamond-0.1.0a8/notdiamond/openai/tests/test_required_args.py
--rw-r--r--   0        0        0     4572 2024-02-29 19:53:45.039060 notdiamond-0.1.0a8/notdiamond/openai/tests/test_response.py
--rw-r--r--   0        0        0     2302 2024-02-29 19:53:45.039141 notdiamond-0.1.0a8/notdiamond/openai/tests/test_streaming.py
--rw-r--r--   0        0        0     9933 2024-02-29 19:53:45.039235 notdiamond-0.1.0a8/notdiamond/openai/tests/test_transform.py
--rw-r--r--   0        0        0     3105 2024-03-01 15:43:18.227994 notdiamond-0.1.0a8/notdiamond/openai/tests/test_utils/__pycache__/test_proxy.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0     5671 2024-03-01 15:43:18.234937 notdiamond-0.1.0a8/notdiamond/openai/tests/test_utils/__pycache__/test_typing.cpython-310-pytest-8.0.0.pyc
--rw-r--r--   0        0        0      687 2024-02-29 19:53:45.039383 notdiamond-0.1.0a8/notdiamond/openai/tests/test_utils/test_proxy.py
--rw-r--r--   0        0        0     2477 2024-02-29 19:53:45.039460 notdiamond-0.1.0a8/notdiamond/openai/tests/test_utils/test_typing.py
--rw-r--r--   0        0        0     3850 2024-02-29 19:53:45.039546 notdiamond-0.1.0a8/notdiamond/openai/tests/utils.py
--rw-r--r--   0        0        0        0 2024-01-22 13:51:23.617800 notdiamond-0.1.0a8/notdiamond/prompts/__init__.py
--rw-r--r--   0        0        0      346 2024-02-19 19:24:39.601816 notdiamond-0.1.0a8/notdiamond/prompts/hash.py
--rw-r--r--   0        0        0     7378 2024-02-29 15:13:41.623628 notdiamond-0.1.0a8/notdiamond/prompts/prompt.py
--rw-r--r--   0        0        0      688 2024-03-06 08:03:55.584981 notdiamond-0.1.0a8/notdiamond/settings.py
--rw-r--r--   0        0        0      611 2024-02-19 19:24:39.602110 notdiamond-0.1.0a8/notdiamond/types.py
--rw-r--r--   0        0        0      638 2024-03-06 08:07:49.417559 notdiamond-0.1.0a8/pyproject.toml
--rw-r--r--   0        0        0     1245 1970-01-01 00:00:00.000000 notdiamond-0.1.0a8/PKG-INFO
+-rw-r--r--   0        0        0      589 2024-03-01 15:42:06.040247 notdiamond-0.1.0a9/README.md
+-rw-r--r--   0        0        0       37 2024-03-01 15:42:06.040996 notdiamond-0.1.0a9/notdiamond/__init__.py
+-rw-r--r--   0        0        0      340 2024-02-19 19:24:39.600527 notdiamond-0.1.0a9/notdiamond/exceptions.py
+-rw-r--r--   0        0        0        0 2024-01-22 13:51:23.616665 notdiamond-0.1.0a9/notdiamond/llms/__init__.py
+-rw-r--r--   0        0        0     8119 2024-03-06 07:49:01.130319 notdiamond-0.1.0a9/notdiamond/llms/llm.py
+-rw-r--r--   0        0        0     1044 2024-03-06 07:49:05.639390 notdiamond-0.1.0a9/notdiamond/llms/provider.py
+-rw-r--r--   0        0        0     2552 2024-03-06 07:50:02.901316 notdiamond-0.1.0a9/notdiamond/llms/request.py
+-rw-r--r--   0        0        0        0 2024-01-22 13:51:23.617063 notdiamond-0.1.0a9/notdiamond/metrics/__init__.py
+-rw-r--r--   0        0        0      601 2024-02-19 19:24:39.601384 notdiamond-0.1.0a9/notdiamond/metrics/metric.py
+-rw-r--r--   0        0        0      628 2024-02-19 19:24:39.601702 notdiamond-0.1.0a9/notdiamond/metrics/request.py
+-rw-r--r--   0        0        0      307 2024-02-29 19:53:45.009032 notdiamond-0.1.0a9/notdiamond/openai/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1175 2024-02-29 19:53:45.009162 notdiamond-0.1.0a9/notdiamond/openai/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0       45 2024-02-29 19:53:44.970083 notdiamond-0.1.0a9/notdiamond/openai/.git
+-rw-r--r--   0        0        0       20 2024-02-29 19:53:45.009271 notdiamond-0.1.0a9/notdiamond/openai/.github/CODEOWNERS
+-rw-r--r--   0        0        0     1785 2024-02-29 19:53:45.009424 notdiamond-0.1.0a9/notdiamond/openai/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      345 2024-02-29 19:53:45.009499 notdiamond-0.1.0a9/notdiamond/openai/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1028 2024-02-29 19:53:45.009579 notdiamond-0.1.0a9/notdiamond/openai/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      496 2024-02-29 19:53:45.009648 notdiamond-0.1.0a9/notdiamond/openai/.github/pull_request_template.md
+-rw-r--r--   0        0        0      790 2024-02-29 19:53:45.009756 notdiamond-0.1.0a9/notdiamond/openai/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1058 2024-02-29 19:53:45.009827 notdiamond-0.1.0a9/notdiamond/openai/.github/workflows/create-releases.yml
+-rw-r--r--   0        0        0      748 2024-02-29 19:53:45.009899 notdiamond-0.1.0a9/notdiamond/openai/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0      691 2024-02-29 19:53:45.009961 notdiamond-0.1.0a9/notdiamond/openai/.github/workflows/release-doctor.yml
+-rw-r--r--   0        0        0       82 2024-02-29 19:53:45.010023 notdiamond-0.1.0a9/notdiamond/openai/.gitignore
+-rw-r--r--   0        0        0        7 2024-02-29 19:53:45.010074 notdiamond-0.1.0a9/notdiamond/openai/.python-version
+-rw-r--r--   0        0        0       19 2024-02-29 19:53:45.010136 notdiamond-0.1.0a9/notdiamond/openai/.release-please-manifest.json
+-rw-r--r--   0        0        0       25 2024-02-29 19:53:45.010189 notdiamond-0.1.0a9/notdiamond/openai/.stats.yml
+-rw-r--r--   0        0        0    33847 2024-02-29 19:53:45.010362 notdiamond-0.1.0a9/notdiamond/openai/CHANGELOG.md
+-rw-r--r--   0        0        0     3482 2024-02-29 19:53:45.010455 notdiamond-0.1.0a9/notdiamond/openai/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11336 2024-02-29 19:53:45.010564 notdiamond-0.1.0a9/notdiamond/openai/LICENSE
+-rw-r--r--   0        0        0    17202 2024-02-29 19:53:45.010689 notdiamond-0.1.0a9/notdiamond/openai/README.md
+-rw-r--r--   0        0        0        0 2024-02-29 20:03:23.605510 notdiamond-0.1.0a9/notdiamond/openai/__init__.py
+-rw-r--r--   0        0        0      187 2024-02-29 20:11:45.266162 notdiamond-0.1.0a9/notdiamond/openai/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    17028 2024-02-29 19:53:45.010796 notdiamond-0.1.0a9/notdiamond/openai/api.md
+-rw-r--r--   0        0        0      924 2024-02-29 19:53:45.010903 notdiamond-0.1.0a9/notdiamond/openai/bin/check-env-state.py
+-rw-r--r--   0        0        0      658 2024-02-29 19:53:45.010981 notdiamond-0.1.0a9/notdiamond/openai/bin/check-release-environment
+-rwxr-xr-x   0        0        0     1320 2024-02-29 19:53:45.011047 notdiamond-0.1.0a9/notdiamond/openai/bin/check-test-server
+-rw-r--r--   0        0        0      100 2024-02-29 19:53:45.011107 notdiamond-0.1.0a9/notdiamond/openai/bin/publish-pypi
+-rw-r--r--   0        0        0     5216 2024-02-29 19:53:45.011197 notdiamond-0.1.0a9/notdiamond/openai/bin/ruffen-docs.py
+-rwxr-xr-x   0        0        0       66 2024-02-29 19:53:45.011250 notdiamond-0.1.0a9/notdiamond/openai/bin/test
+-rw-r--r--   0        0        0      239 2024-02-29 19:53:45.011341 notdiamond-0.1.0a9/notdiamond/openai/examples/.keep
+-rw-r--r--   0        0        0     1336 2024-02-29 19:53:45.011414 notdiamond-0.1.0a9/notdiamond/openai/examples/assistant.py
+-rwxr-xr-x   0        0        0      462 2024-02-29 19:53:45.011475 notdiamond-0.1.0a9/notdiamond/openai/examples/async_demo.py
+-rwxr-xr-x   0        0        0     1827 2024-02-29 19:53:45.011545 notdiamond-0.1.0a9/notdiamond/openai/examples/audio.py
+-rwxr-xr-x   0        0        0     1460 2024-02-29 19:53:45.011610 notdiamond-0.1.0a9/notdiamond/openai/examples/azure.py
+-rwxr-xr-x   0        0        0      983 2024-02-29 19:53:45.011671 notdiamond-0.1.0a9/notdiamond/openai/examples/azure_ad.py
+-rwxr-xr-x   0        0        0      828 2024-02-29 19:53:45.011734 notdiamond-0.1.0a9/notdiamond/openai/examples/demo.py
+-rwxr-xr-x   0        0        0      659 2024-02-29 19:53:45.011796 notdiamond-0.1.0a9/notdiamond/openai/examples/module_client.py
+-rw-r--r--   0        0        0      462 2024-02-29 19:53:45.011858 notdiamond-0.1.0a9/notdiamond/openai/examples/picture.py
+-rwxr-xr-x   0        0        0     1642 2024-02-29 19:53:45.011921 notdiamond-0.1.0a9/notdiamond/openai/examples/streaming.py
+-rw-r--r--   0        0        0     1267 2024-02-29 19:53:45.012005 notdiamond-0.1.0a9/notdiamond/openai/mypy.ini
+-rw-r--r--   0        0        0      295 2024-02-29 19:53:45.012139 notdiamond-0.1.0a9/notdiamond/openai/noxfile.py
+-rw-r--r--   0        0        0     3903 2024-02-29 19:53:45.012246 notdiamond-0.1.0a9/notdiamond/openai/pyproject.toml
+-rw-r--r--   0        0        0     1322 2024-02-29 19:53:45.012387 notdiamond-0.1.0a9/notdiamond/openai/release-please-config.json
+-rw-r--r--   0        0        0     2691 2024-02-29 19:53:45.012556 notdiamond-0.1.0a9/notdiamond/openai/requirements-dev.lock
+-rw-r--r--   0        0        0     1145 2024-02-29 19:53:45.012646 notdiamond-0.1.0a9/notdiamond/openai/requirements.lock
+-rw-r--r--   0        0        0        0 2024-02-29 20:03:30.670281 notdiamond-0.1.0a9/notdiamond/openai/src/__init__.py
+-rw-r--r--   0        0        0      191 2024-02-29 20:11:45.266522 notdiamond-0.1.0a9/notdiamond/openai/src/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     9140 2024-02-29 19:53:45.012863 notdiamond-0.1.0a9/notdiamond/openai/src/openai/__init__.py
+-rw-r--r--   0        0        0       30 2024-02-29 19:53:45.012955 notdiamond-0.1.0a9/notdiamond/openai/src/openai/__main__.py
+-rw-r--r--   0        0        0     7629 2024-02-29 20:11:45.267964 notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    42814 2024-02-29 20:11:45.351538 notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/_base_client.cpython-310.pyc
+-rw-r--r--   0        0        0    12888 2024-02-29 20:11:45.326822 notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/_client.cpython-310.pyc
+-rw-r--r--   0        0        0     6085 2024-02-29 20:11:45.278798 notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/_compat.cpython-310.pyc
+-rw-r--r--   0        0        0      609 2024-02-29 20:11:45.282175 notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/_constants.cpython-310.pyc
+-rw-r--r--   0        0        0     4489 2024-02-29 20:11:45.337545 notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/_exceptions.cpython-310.pyc
+-rw-r--r--   0        0        0     4279 2024-02-29 20:11:45.353761 notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/_files.cpython-310.pyc
+-rw-r--r--   0        0        0    14577 2024-02-29 20:11:45.335157 notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/_legacy_response.cpython-310.pyc
+-rw-r--r--   0        0        0    13764 2024-02-29 20:11:45.271553 notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/_models.cpython-310.pyc
+-rw-r--r--   0        0        0     3538 2024-02-29 20:11:49.022777 notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/_module_client.cpython-310.pyc
+-rw-r--r--   0        0        0     4170 2024-02-29 20:11:45.352822 notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/_qs.cpython-310.pyc
+-rw-r--r--   0        0        0     1535 2024-02-29 20:11:45.339587 notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/_resource.cpython-310.pyc
+-rw-r--r--   0        0        0    24036 2024-02-29 20:11:45.343022 notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/_response.cpython-310.pyc
+-rw-r--r--   0        0        0     9196 2024-02-29 20:11:45.336719 notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/_streaming.cpython-310.pyc
+-rw-r--r--   0        0        0     5925 2024-02-29 20:11:45.272712 notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/_types.cpython-310.pyc
+-rw-r--r--   0        0        0      245 2024-02-29 20:11:49.017226 notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/_version.cpython-310.pyc
+-rw-r--r--   0        0        0     2942 2024-02-29 20:11:45.344151 notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/pagination.cpython-310.pyc
+-rw-r--r--   0        0        0      293 2024-02-29 20:11:49.020800 notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/version.cpython-310.pyc
+-rw-r--r--   0        0        0    62655 2024-02-29 19:53:45.013190 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_base_client.py
+-rw-r--r--   0        0        0    20791 2024-02-29 19:11:33.863189 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_client.py
+-rw-r--r--   0        0        0     6389 2024-02-29 19:53:45.013412 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_compat.py
+-rw-r--r--   0        0        0      423 2024-02-29 19:53:45.013490 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_constants.py
+-rw-r--r--   0        0        0     3614 2024-02-29 19:53:45.013576 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_exceptions.py
+-rw-r--r--   0        0        0      107 2024-02-29 19:53:45.013683 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_extras/__init__.py
+-rw-r--r--   0        0        0      310 2024-02-29 20:11:49.000634 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_extras/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      761 2024-02-29 20:11:49.001664 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_extras/__pycache__/_common.cpython-310.pyc
+-rw-r--r--   0        0        0     1208 2024-02-29 20:11:49.001222 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_extras/__pycache__/numpy_proxy.cpython-310.pyc
+-rw-r--r--   0        0        0     1032 2024-02-29 20:11:49.002105 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_extras/__pycache__/pandas_proxy.cpython-310.pyc
+-rw-r--r--   0        0        0      364 2024-02-29 19:53:45.013765 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_extras/_common.py
+-rw-r--r--   0        0        0      799 2024-02-29 19:53:45.013855 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_extras/numpy_proxy.py
+-rw-r--r--   0        0        0      637 2024-02-29 19:53:45.013929 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_extras/pandas_proxy.py
+-rw-r--r--   0        0        0     3470 2024-02-29 19:53:45.014001 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_files.py
+-rw-r--r--   0        0        0    14903 2024-02-29 19:53:45.014111 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_legacy_response.py
+-rw-r--r--   0        0        0    16432 2024-02-29 19:53:45.014250 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_models.py
+-rw-r--r--   0        0        0     2280 2024-02-29 19:53:45.014347 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_module_client.py
+-rw-r--r--   0        0        0     4846 2024-02-29 19:53:45.014419 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_qs.py
+-rw-r--r--   0        0        0     1067 2024-02-29 19:53:45.014480 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_resource.py
+-rw-r--r--   0        0        0    27957 2024-02-29 19:53:45.014770 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_response.py
+-rw-r--r--   0        0        0     9034 2024-02-29 19:53:45.015004 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_streaming.py
+-rw-r--r--   0        0        0     6123 2024-02-29 19:53:45.015107 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_types.py
+-rw-r--r--   0        0        0     1727 2024-02-29 19:53:45.015288 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/__init__.py
+-rw-r--r--   0        0        0     1393 2024-02-29 20:11:45.274182 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      938 2024-02-29 20:11:49.017835 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/__pycache__/_logs.cpython-310.pyc
+-rw-r--r--   0        0        0     2394 2024-02-29 20:11:45.275523 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/__pycache__/_proxy.cpython-310.pyc
+-rw-r--r--   0        0        0      641 2024-02-29 20:11:45.280329 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/__pycache__/_streams.cpython-310.pyc
+-rw-r--r--   0        0        0     2659 2024-02-29 20:11:45.274794 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/__pycache__/_sync.cpython-310.pyc
+-rw-r--r--   0        0        0     6444 2024-02-29 20:11:45.281572 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/__pycache__/_transform.cpython-310.pyc
+-rw-r--r--   0        0        0     3265 2024-02-29 20:11:45.279942 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/__pycache__/_typing.cpython-310.pyc
+-rw-r--r--   0        0        0    12147 2024-02-29 20:11:45.277655 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/__pycache__/_utils.cpython-310.pyc
+-rw-r--r--   0        0        0      774 2024-02-29 19:53:45.015369 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/_logs.py
+-rw-r--r--   0        0        0     1909 2024-02-29 19:53:45.015442 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2024-02-29 19:53:45.015505 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2024-02-29 19:53:45.015577 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/_sync.py
+-rw-r--r--   0        0        0     7223 2024-02-29 19:53:45.015668 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2024-02-29 19:53:45.015750 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/_typing.py
+-rw-r--r--   0        0        0    11105 2024-02-29 19:53:45.015855 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/_utils.py
+-rw-r--r--   0        0        0      126 2024-02-29 19:53:45.015929 notdiamond-0.1.0a9/notdiamond/openai/src/openai/_version.py
+-rw-r--r--   0        0        0       31 2024-02-29 19:53:45.016028 notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/__init__.py
+-rw-r--r--   0        0        0       58 2024-02-29 19:53:45.016128 notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/_api/__init__.py
+-rw-r--r--   0        0        0      451 2024-02-29 19:53:45.016199 notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/_api/_main.py
+-rw-r--r--   0        0        0     3347 2024-02-29 19:53:45.016267 notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/_api/audio.py
+-rw-r--r--   0        0        0      300 2024-02-29 19:53:45.016373 notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/_api/chat/__init__.py
+-rw-r--r--   0        0        0     5363 2024-02-29 19:53:45.016452 notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/_api/chat/completions.py
+-rw-r--r--   0        0        0     6412 2024-02-29 19:53:45.016539 notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/_api/completions.py
+-rw-r--r--   0        0        0     2345 2024-02-29 19:53:45.016605 notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/_api/files.py
+-rw-r--r--   0        0        0     5062 2024-02-29 19:53:45.016661 notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/_api/image.py
+-rw-r--r--   0        0        0     1295 2024-02-29 19:53:45.016728 notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/_api/models.py
+-rw-r--r--   0        0        0     6743 2024-02-29 19:53:45.016813 notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/_cli.py
+-rw-r--r--   0        0        0      479 2024-02-29 19:53:45.016883 notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/_errors.py
+-rw-r--r--   0        0        0      491 2024-02-29 19:53:45.016949 notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/_models.py
+-rw-r--r--   0        0        0     1406 2024-02-29 19:53:45.017526 notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/_progress.py
+-rw-r--r--   0        0        0       58 2024-02-29 19:53:45.017760 notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/_tools/__init__.py
+-rw-r--r--   0        0        0      467 2024-02-29 19:53:45.017856 notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/_tools/_main.py
+-rw-r--r--   0        0        0     1543 2024-02-29 19:53:45.017933 notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/_tools/fine_tunes.py
+-rw-r--r--   0        0        0     4910 2024-02-29 19:53:45.018022 notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/_tools/migrate.py
+-rw-r--r--   0        0        0      848 2024-02-29 19:53:45.018096 notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/_utils.py
+-rw-r--r--   0        0        0      224 2024-02-29 19:53:45.018213 notdiamond-0.1.0a9/notdiamond/openai/src/openai/lib/.keep
+-rw-r--r--   0        0        0     2384 2024-02-29 20:11:49.021843 notdiamond-0.1.0a9/notdiamond/openai/src/openai/lib/__pycache__/_old_api.cpython-310.pyc
+-rw-r--r--   0        0        0    12573 2024-02-29 20:11:49.020116 notdiamond-0.1.0a9/notdiamond/openai/src/openai/lib/__pycache__/azure.cpython-310.pyc
+-rw-r--r--   0        0        0     1947 2024-02-29 19:53:45.018335 notdiamond-0.1.0a9/notdiamond/openai/src/openai/lib/_old_api.py
+-rw-r--r--   0        0        0    35189 2024-02-29 19:53:45.018585 notdiamond-0.1.0a9/notdiamond/openai/src/openai/lib/_validators.py
+-rw-r--r--   0        0        0    21021 2024-02-29 19:53:45.018707 notdiamond-0.1.0a9/notdiamond/openai/src/openai/lib/azure.py
+-rw-r--r--   0        0        0     2727 2024-02-29 19:53:45.018801 notdiamond-0.1.0a9/notdiamond/openai/src/openai/pagination.py
+-rw-r--r--   0        0        0        0 2024-02-29 19:53:45.018833 notdiamond-0.1.0a9/notdiamond/openai/src/openai/py.typed
+-rw-r--r--   0        0        0     3766 2024-02-29 19:53:45.018942 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/__init__.py
+-rw-r--r--   0        0        0     2704 2024-02-29 20:11:45.327645 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    21296 2024-02-29 20:11:49.004989 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/__pycache__/completions.cpython-310.pyc
+-rw-r--r--   0        0        0     7113 2024-02-29 20:11:49.000033 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/__pycache__/embeddings.cpython-310.pyc
+-rw-r--r--   0        0        0    11879 2024-02-29 20:11:48.995302 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/__pycache__/files.cpython-310.pyc
+-rw-r--r--   0        0        0    11992 2024-02-29 20:11:48.997626 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/__pycache__/images.cpython-310.pyc
+-rw-r--r--   0        0        0     5940 2024-02-29 20:11:48.998933 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/__pycache__/models.cpython-310.pyc
+-rw-r--r--   0        0        0     5188 2024-02-29 20:11:49.016748 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/__pycache__/moderations.cpython-310.pyc
+-rw-r--r--   0        0        0     1654 2024-02-29 19:53:45.019052 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/audio/__init__.py
+-rw-r--r--   0        0        0     1282 2024-02-29 20:11:48.984278 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/audio/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5750 2024-02-29 20:11:48.985376 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/audio/__pycache__/audio.cpython-310.pyc
+-rw-r--r--   0        0        0     5952 2024-02-29 20:11:48.986309 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/audio/__pycache__/speech.cpython-310.pyc
+-rw-r--r--   0        0        0     7001 2024-02-29 20:11:48.993205 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/audio/__pycache__/transcriptions.cpython-310.pyc
+-rw-r--r--   0        0        0     6145 2024-02-29 20:11:48.992132 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/audio/__pycache__/translations.cpython-310.pyc
+-rw-r--r--   0        0        0     4448 2024-02-29 19:53:45.019137 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/audio/audio.py
+-rw-r--r--   0        0        0     8179 2024-02-29 19:53:45.019228 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/audio/speech.py
+-rw-r--r--   0        0        0    10601 2024-02-29 19:53:45.019321 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/audio/transcriptions.py
+-rw-r--r--   0        0        0     8805 2024-02-29 19:53:45.019419 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/audio/translations.py
+-rw-r--r--   0        0        0     1170 2024-02-29 19:53:45.019595 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/__init__.py
+-rw-r--r--   0        0        0      972 2024-02-29 20:11:45.328248 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4669 2024-02-29 20:11:45.329098 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/__pycache__/beta.cpython-310.pyc
+-rw-r--r--   0        0        0      816 2024-02-29 19:53:45.019705 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/assistants/__init__.py
+-rw-r--r--   0        0        0      744 2024-02-29 20:11:45.420692 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/assistants/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    14914 2024-02-29 20:11:45.429546 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/assistants/__pycache__/assistants.cpython-310.pyc
+-rw-r--r--   0        0        0     9460 2024-02-29 20:11:45.422404 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/assistants/__pycache__/files.cpython-310.pyc
+-rw-r--r--   0        0        0    30627 2024-02-29 19:53:45.019797 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/assistants/assistants.py
+-rw-r--r--   0        0        0    19432 2024-02-29 19:53:45.019906 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/assistants/files.py
+-rw-r--r--   0        0        0     3340 2024-02-29 19:53:45.019995 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/beta.py
+-rw-r--r--   0        0        0     1144 2024-02-29 19:53:45.020117 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/__init__.py
+-rw-r--r--   0        0        0      966 2024-02-29 20:11:45.329523 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    13265 2024-02-29 20:11:45.413040 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/__pycache__/threads.cpython-310.pyc
+-rw-r--r--   0        0        0      790 2024-02-29 19:53:45.020219 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/messages/__init__.py
+-rw-r--r--   0        0        0      736 2024-02-29 20:11:45.413614 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/messages/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7304 2024-02-29 20:11:45.414945 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/messages/__pycache__/files.cpython-310.pyc
+-rw-r--r--   0        0        0    12033 2024-02-29 20:11:45.419920 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/messages/__pycache__/messages.cpython-310.pyc
+-rw-r--r--   0        0        0    12267 2024-02-29 19:53:45.020290 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/messages/files.py
+-rw-r--r--   0        0        0    22831 2024-02-29 19:53:45.020400 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/messages/messages.py
+-rw-r--r--   0        0        0      738 2024-02-29 19:53:45.020508 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/runs/__init__.py
+-rw-r--r--   0        0        0      704 2024-02-29 20:11:45.330150 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/runs/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    15291 2024-02-29 20:11:45.332650 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/runs/__pycache__/runs.cpython-310.pyc
+-rw-r--r--   0        0        0     7279 2024-02-29 20:11:45.339076 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/runs/__pycache__/steps.cpython-310.pyc
+-rw-r--r--   0        0        0    32278 2024-02-29 19:53:45.020714 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/runs/runs.py
+-rw-r--r--   0        0        0    12141 2024-02-29 19:53:45.021178 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/runs/steps.py
+-rw-r--r--   0        0        0    25273 2024-02-29 19:53:45.021761 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/threads.py
+-rw-r--r--   0        0        0      816 2024-02-29 19:53:45.022037 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/chat/__init__.py
+-rw-r--r--   0        0        0      733 2024-02-29 20:11:45.430464 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/chat/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3541 2024-02-29 20:11:45.431163 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/chat/__pycache__/chat.cpython-310.pyc
+-rw-r--r--   0        0        0    26512 2024-02-29 20:11:45.434914 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/chat/__pycache__/completions.cpython-310.pyc
+-rw-r--r--   0        0        0     2309 2024-02-29 19:53:45.022177 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/chat/chat.py
+-rw-r--r--   0        0        0    71495 2024-02-29 20:05:02.015985 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/chat/completions.py
+-rw-r--r--   0        0        0    56586 2024-02-29 19:53:45.022511 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/completions.py
+-rw-r--r--   0        0        0    10677 2024-02-29 19:53:45.022614 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/embeddings.py
+-rw-r--r--   0        0        0    26000 2024-02-29 19:53:45.022763 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/files.py
+-rw-r--r--   0        0        0      804 2024-02-29 19:53:45.022894 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/fine_tuning/__init__.py
+-rw-r--r--   0        0        0      734 2024-02-29 20:11:49.005802 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/fine_tuning/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3598 2024-02-29 20:11:49.015690 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/fine_tuning/__pycache__/fine_tuning.cpython-310.pyc
+-rw-r--r--   0        0        0    11568 2024-02-29 20:11:49.007415 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/fine_tuning/__pycache__/jobs.cpython-310.pyc
+-rw-r--r--   0        0        0     2338 2024-02-29 19:53:45.022980 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/fine_tuning/fine_tuning.py
+-rw-r--r--   0        0        0    24455 2024-02-29 19:53:45.023095 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/fine_tuning/jobs.py
+-rw-r--r--   0        0        0    24159 2024-02-29 19:53:45.023190 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/images.py
+-rw-r--r--   0        0        0    10150 2024-02-29 19:53:45.023295 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/models.py
+-rw-r--r--   0        0        0     6576 2024-02-29 19:53:45.023376 notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/moderations.py
+-rw-r--r--   0        0        0     1629 2024-02-29 19:53:45.023494 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__init__.py
+-rw-r--r--   0        0        0     1571 2024-02-29 20:11:45.268720 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      915 2024-02-29 20:11:45.297816 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/completion.cpython-310.pyc
+-rw-r--r--   0        0        0     1078 2024-02-29 20:11:45.299574 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/completion_choice.cpython-310.pyc
+-rw-r--r--   0        0        0     1774 2024-02-29 20:11:45.319155 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/completion_create_params.cpython-310.pyc
+-rw-r--r--   0        0        0      546 2024-02-29 20:11:45.298210 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/completion_usage.cpython-310.pyc
+-rw-r--r--   0        0        0      930 2024-02-29 20:11:45.320379 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/create_embedding_response.cpython-310.pyc
+-rw-r--r--   0        0        0      625 2024-02-29 20:11:45.296413 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/embedding.cpython-310.pyc
+-rw-r--r--   0        0        0      980 2024-02-29 20:11:45.318291 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/embedding_create_params.cpython-310.pyc
+-rw-r--r--   0        0        0      249 2024-02-29 20:11:45.311226 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/file_content.cpython-310.pyc
+-rw-r--r--   0        0        0      716 2024-02-29 20:11:45.316491 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/file_create_params.cpython-310.pyc
+-rw-r--r--   0        0        0      576 2024-02-29 20:11:45.311648 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/file_deleted.cpython-310.pyc
+-rw-r--r--   0        0        0      548 2024-02-29 20:11:45.314820 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/file_list_params.cpython-310.pyc
+-rw-r--r--   0        0        0      864 2024-02-29 20:11:45.308677 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/file_object.cpython-310.pyc
+-rw-r--r--   0        0        0      596 2024-02-29 20:11:45.269260 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/image.cpython-310.pyc
+-rw-r--r--   0        0        0      984 2024-02-29 20:11:45.323781 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/image_create_variation_params.cpython-310.pyc
+-rw-r--r--   0        0        0     1023 2024-02-29 20:11:45.315787 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/image_edit_params.cpython-310.pyc
+-rw-r--r--   0        0        0     1067 2024-02-29 20:11:45.317221 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/image_generate_params.cpython-310.pyc
+-rw-r--r--   0        0        0      585 2024-02-29 20:11:45.313551 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/images_response.cpython-310.pyc
+-rw-r--r--   0        0        0      597 2024-02-29 20:11:45.292767 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/model.cpython-310.pyc
+-rw-r--r--   0        0        0      509 2024-02-29 20:11:45.312680 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/model_deleted.cpython-310.pyc
+-rw-r--r--   0        0        0     1643 2024-02-29 20:11:45.305031 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/moderation.cpython-310.pyc
+-rw-r--r--   0        0        0      772 2024-02-29 20:11:45.319920 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/moderation_create_params.cpython-310.pyc
+-rw-r--r--   0        0        0      641 2024-02-29 20:11:45.322148 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/moderation_create_response.cpython-310.pyc
+-rw-r--r--   0        0        0      461 2024-02-29 19:53:45.023613 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/audio/__init__.py
+-rw-r--r--   0        0        0      572 2024-02-29 20:11:48.986811 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/audio/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      921 2024-02-29 20:11:48.989899 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/audio/__pycache__/speech_create_params.cpython-310.pyc
+-rw-r--r--   0        0        0      475 2024-02-29 20:11:48.988110 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/audio/__pycache__/transcription.cpython-310.pyc
+-rw-r--r--   0        0        0     1031 2024-02-29 20:11:48.991006 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/audio/__pycache__/transcription_create_params.cpython-310.pyc
+-rw-r--r--   0        0        0      471 2024-02-29 20:11:48.987131 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/audio/__pycache__/translation.cpython-310.pyc
+-rw-r--r--   0        0        0      860 2024-02-29 20:11:48.990535 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/audio/__pycache__/translation_create_params.cpython-310.pyc
+-rw-r--r--   0        0        0     1417 2024-02-29 19:53:45.023701 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/audio/speech_create_params.py
+-rw-r--r--   0        0        0      164 2024-02-29 19:53:45.023771 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/audio/transcription.py
+-rw-r--r--   0        0        0     2018 2024-02-29 19:53:45.023855 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/audio/transcription_create_params.py
+-rw-r--r--   0        0        0      160 2024-02-29 19:53:45.023924 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/audio/translation.py
+-rw-r--r--   0        0        0     1404 2024-02-29 19:53:45.024012 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/audio/translation_create_params.py
+-rw-r--r--   0        0        0      791 2024-02-29 19:53:45.024141 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/__init__.py
+-rw-r--r--   0        0        0      856 2024-02-29 20:11:45.360292 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1541 2024-02-29 20:11:45.362441 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/__pycache__/assistant.cpython-310.pyc
+-rw-r--r--   0        0        0     1635 2024-02-29 20:11:45.370165 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/__pycache__/assistant_create_params.cpython-310.pyc
+-rw-r--r--   0        0        0      604 2024-02-29 20:11:45.367009 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/__pycache__/assistant_deleted.cpython-310.pyc
+-rw-r--r--   0        0        0      672 2024-02-29 20:11:45.369553 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/__pycache__/assistant_list_params.cpython-310.pyc
+-rw-r--r--   0        0        0     1625 2024-02-29 20:11:45.372373 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/__pycache__/assistant_update_params.cpython-310.pyc
+-rw-r--r--   0        0        0      670 2024-02-29 20:11:45.360954 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/__pycache__/thread.cpython-310.pyc
+-rw-r--r--   0        0        0     2102 2024-02-29 20:11:45.373247 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/__pycache__/thread_create_and_run_params.cpython-310.pyc
+-rw-r--r--   0        0        0     1001 2024-02-29 20:11:45.368488 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/__pycache__/thread_create_params.cpython-310.pyc
+-rw-r--r--   0        0        0      595 2024-02-29 20:11:45.365775 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/__pycache__/thread_deleted.cpython-310.pyc
+-rw-r--r--   0        0        0      614 2024-02-29 20:11:45.369105 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/__pycache__/thread_update_params.cpython-310.pyc
+-rw-r--r--   0        0        0     2562 2024-02-29 19:53:45.024233 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/assistant.py
+-rw-r--r--   0        0        0     2553 2024-02-29 19:53:45.024320 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/assistant_create_params.py
+-rw-r--r--   0        0        0      268 2024-02-29 19:53:45.024389 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/assistant_deleted.py
+-rw-r--r--   0        0        0     1187 2024-02-29 19:53:45.024491 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/assistant_list_params.py
+-rw-r--r--   0        0        0     2670 2024-02-29 19:53:45.024575 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/assistant_update_params.py
+-rw-r--r--   0        0        0      356 2024-02-29 19:53:45.024684 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/assistants/__init__.py
+-rw-r--r--   0        0        0      500 2024-02-29 20:11:45.423086 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/assistants/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      646 2024-02-29 20:11:45.423638 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/assistants/__pycache__/assistant_file.cpython-310.pyc
+-rw-r--r--   0        0        0      597 2024-02-29 20:11:45.426218 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/assistants/__pycache__/file_create_params.cpython-310.pyc
+-rw-r--r--   0        0        0      625 2024-02-29 20:11:45.426764 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/assistants/__pycache__/file_delete_response.cpython-310.pyc
+-rw-r--r--   0        0        0      673 2024-02-29 20:11:45.424945 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/assistants/__pycache__/file_list_params.cpython-310.pyc
+-rw-r--r--   0        0        0      554 2024-02-29 19:53:45.024753 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/assistants/assistant_file.py
+-rw-r--r--   0        0        0      484 2024-02-29 19:53:45.024832 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/assistants/file_create_params.py
+-rw-r--r--   0        0        0      278 2024-02-29 19:53:45.024898 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/assistants/file_delete_response.py
+-rw-r--r--   0        0        0     1177 2024-02-29 19:53:45.024959 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/assistants/file_list_params.py
+-rw-r--r--   0        0        0       89 2024-02-29 19:53:45.025061 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/chat/__init__.py
+-rw-r--r--   0        0        0      781 2024-02-29 19:53:45.025134 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/thread.py
+-rw-r--r--   0        0        0     3740 2024-02-29 19:53:45.025222 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/thread_create_and_run_params.py
+-rw-r--r--   0        0        0     1631 2024-02-29 19:53:45.025720 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/thread_create_params.py
+-rw-r--r--   0        0        0      259 2024-02-29 19:53:45.025931 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/thread_deleted.py
+-rw-r--r--   0        0        0      554 2024-02-29 19:53:45.026023 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/thread_update_params.py
+-rw-r--r--   0        0        0     1024 2024-02-29 19:53:45.026152 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/__init__.py
+-rw-r--r--   0        0        0     1060 2024-02-29 20:11:45.374444 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      764 2024-02-29 20:11:45.389323 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/__pycache__/message_content_image_file.cpython-310.pyc
+-rw-r--r--   0        0        0     1762 2024-02-29 20:11:45.385099 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/__pycache__/message_content_text.cpython-310.pyc
+-rw-r--r--   0        0        0      796 2024-02-29 20:11:45.395433 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/__pycache__/message_create_params.cpython-310.pyc
+-rw-r--r--   0        0        0      676 2024-02-29 20:11:45.394972 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/__pycache__/message_list_params.cpython-310.pyc
+-rw-r--r--   0        0        0      679 2024-02-29 20:11:45.395851 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/__pycache__/message_update_params.cpython-310.pyc
+-rw-r--r--   0        0        0      825 2024-02-29 20:11:45.376715 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/__pycache__/required_action_function_tool_call.cpython-310.pyc
+-rw-r--r--   0        0        0     2920 2024-02-29 20:11:45.375228 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/__pycache__/run.cpython-310.pyc
+-rw-r--r--   0        0        0     1611 2024-02-29 20:11:45.393982 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/__pycache__/run_create_params.cpython-310.pyc
+-rw-r--r--   0        0        0      668 2024-02-29 20:11:45.393164 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/__pycache__/run_list_params.cpython-310.pyc
+-rw-r--r--   0        0        0      406 2024-02-29 20:11:45.375713 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/__pycache__/run_status.cpython-310.pyc
+-rw-r--r--   0        0        0      900 2024-02-29 20:11:45.396247 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/__pycache__/run_submit_tool_outputs_params.cpython-310.pyc
+-rw-r--r--   0        0        0      671 2024-02-29 20:11:45.394565 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/__pycache__/run_update_params.cpython-310.pyc
+-rw-r--r--   0        0        0     1113 2024-02-29 20:11:45.383874 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/__pycache__/thread_message.cpython-310.pyc
+-rw-r--r--   0        0        0      489 2024-02-29 19:53:45.026231 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/message_content_image_file.py
+-rw-r--r--   0        0        0     1575 2024-02-29 19:53:45.026301 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/message_content_text.py
+-rw-r--r--   0        0        0     1100 2024-02-29 19:53:45.026379 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/message_create_params.py
+-rw-r--r--   0        0        0     1183 2024-02-29 19:53:45.026446 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/message_list_params.py
+-rw-r--r--   0        0        0      596 2024-02-29 19:53:45.026506 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/message_update_params.py
+-rw-r--r--   0        0        0      206 2024-02-29 19:53:45.026620 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/messages/__init__.py
+-rw-r--r--   0        0        0      380 2024-02-29 20:11:45.415542 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/messages/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      734 2024-02-29 20:11:45.417400 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/messages/__pycache__/file_list_params.cpython-310.pyc
+-rw-r--r--   0        0        0      651 2024-02-29 20:11:45.416061 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/messages/__pycache__/message_file.cpython-310.pyc
+-rw-r--r--   0        0        0     1217 2024-02-29 19:53:45.026682 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/messages/file_list_params.py
+-rw-r--r--   0        0        0      695 2024-02-29 19:53:45.026746 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/messages/message_file.py
+-rw-r--r--   0        0        0      855 2024-02-29 19:53:45.026839 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/required_action_function_tool_call.py
+-rw-r--r--   0        0        0     4902 2024-02-29 19:53:45.026924 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/run.py
+-rw-r--r--   0        0        0     2520 2024-02-29 19:53:45.027003 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/run_create_params.py
+-rw-r--r--   0        0        0     1175 2024-02-29 19:53:45.027079 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/run_list_params.py
+-rw-r--r--   0        0        0      249 2024-02-29 19:53:45.027160 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/run_status.py
+-rw-r--r--   0        0        0      727 2024-02-29 19:53:45.027231 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/run_submit_tool_outputs_params.py
+-rw-r--r--   0        0        0      588 2024-02-29 19:53:45.027299 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/run_update_params.py
+-rw-r--r--   0        0        0      574 2024-02-29 19:53:45.027419 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/__init__.py
+-rw-r--r--   0        0        0      687 2024-02-29 20:11:45.396681 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1542 2024-02-29 20:11:45.397989 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/code_tool_call.cpython-310.pyc
+-rw-r--r--   0        0        0      879 2024-02-29 20:11:45.401406 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/function_tool_call.cpython-310.pyc
+-rw-r--r--   0        0        0      790 2024-02-29 20:11:45.405146 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/message_creation_step_details.cpython-310.pyc
+-rw-r--r--   0        0        0      613 2024-02-29 20:11:45.403185 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/retrieval_tool_call.cpython-310.pyc
+-rw-r--r--   0        0        0     1870 2024-02-29 20:11:45.397189 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/run_step.cpython-310.pyc
+-rw-r--r--   0        0        0      730 2024-02-29 20:11:45.410682 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/step_list_params.cpython-310.pyc
+-rw-r--r--   0        0        0      864 2024-02-29 20:11:45.397532 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/tool_calls_step_details.cpython-310.pyc
+-rw-r--r--   0        0        0     1632 2024-02-29 19:53:45.027543 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/code_tool_call.py
+-rw-r--r--   0        0        0      887 2024-02-29 19:53:45.027644 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/function_tool_call.py
+-rw-r--r--   0        0        0      473 2024-02-29 19:53:45.027736 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/message_creation_step_details.py
+-rw-r--r--   0        0        0      481 2024-02-29 19:53:45.027816 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/retrieval_tool_call.py
+-rw-r--r--   0        0        0     3312 2024-02-29 19:53:45.027927 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/run_step.py
+-rw-r--r--   0        0        0     1217 2024-02-29 19:53:45.027999 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/step_list_params.py
+-rw-r--r--   0        0        0      736 2024-02-29 19:53:45.028067 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/tool_calls_step_details.py
+-rw-r--r--   0        0        0     2057 2024-02-29 19:53:45.028136 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/thread_message.py
+-rw-r--r--   0        0        0     2431 2024-02-29 19:53:45.028280 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__init__.py
+-rw-r--r--   0        0        0     2057 2024-02-29 20:11:48.950251 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1583 2024-02-29 20:11:48.951224 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion.cpython-310.pyc
+-rw-r--r--   0        0        0     1181 2024-02-29 20:11:48.981137 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_assistant_message_param.cpython-310.pyc
+-rw-r--r--   0        0        0     2474 2024-02-29 20:11:48.967167 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_chunk.cpython-310.pyc
+-rw-r--r--   0        0        0      918 2024-02-29 20:11:48.978609 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_content_part_image_param.cpython-310.pyc
+-rw-r--r--   0        0        0      588 2024-02-29 20:11:48.977892 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_content_part_param.cpython-310.pyc
+-rw-r--r--   0        0        0      687 2024-02-29 20:11:48.978201 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_content_part_text_param.cpython-310.pyc
+-rw-r--r--   0        0        0      628 2024-02-29 20:11:48.982841 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_function_call_option_param.cpython-310.pyc
+-rw-r--r--   0        0        0      777 2024-02-29 20:11:48.980319 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_function_message_param.cpython-310.pyc
+-rw-r--r--   0        0        0     1052 2024-02-29 20:11:48.952840 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_message.cpython-310.pyc
+-rw-r--r--   0        0        0      868 2024-02-29 20:11:48.976682 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_message_param.cpython-310.pyc
+-rw-r--r--   0        0        0      815 2024-02-29 20:11:48.954109 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_message_tool_call.cpython-310.pyc
+-rw-r--r--   0        0        0      913 2024-02-29 20:11:48.981593 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_message_tool_call_param.cpython-310.pyc
+-rw-r--r--   0        0        0      861 2024-02-29 20:11:48.982420 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_named_tool_choice_param.cpython-310.pyc
+-rw-r--r--   0        0        0      365 2024-02-29 20:11:48.966307 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_role.cpython-310.pyc
+-rw-r--r--   0        0        0      712 2024-02-29 20:11:48.979205 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_system_message_param.cpython-310.pyc
+-rw-r--r--   0        0        0      929 2024-02-29 20:11:48.958374 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_token_logprob.cpython-310.pyc
+-rw-r--r--   0        0        0      566 2024-02-29 20:11:48.982102 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_tool_choice_option_param.cpython-310.pyc
+-rw-r--r--   0        0        0      709 2024-02-29 20:11:48.977112 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_tool_message_param.cpython-310.pyc
+-rw-r--r--   0        0        0      744 2024-02-29 20:11:48.976072 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_tool_param.cpython-310.pyc
+-rw-r--r--   0        0        0      904 2024-02-29 20:11:48.977567 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_user_message_param.cpython-310.pyc
+-rw-r--r--   0        0        0     3056 2024-02-29 20:11:48.975542 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/completion_create_params.cpython-310.pyc
+-rw-r--r--   0        0        0     2288 2024-02-29 19:53:45.028388 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion.py
+-rw-r--r--   0        0        0     1605 2024-02-29 19:53:45.028458 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_assistant_message_param.py
+-rw-r--r--   0        0        0     4062 2024-02-29 19:53:45.028534 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_chunk.py
+-rw-r--r--   0        0        0      764 2024-02-29 19:53:45.028616 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_content_part_image_param.py
+-rw-r--r--   0        0        0      453 2024-02-29 19:53:45.028757 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_content_part_param.py
+-rw-r--r--   0        0        0      396 2024-02-29 19:53:45.028828 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_content_part_text_param.py
+-rw-r--r--   0        0        0      332 2024-02-29 19:53:45.028900 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_function_call_option_param.py
+-rw-r--r--   0        0        0      558 2024-02-29 19:53:45.028982 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_function_message_param.py
+-rw-r--r--   0        0        0     1249 2024-02-29 19:53:45.029056 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_message.py
+-rw-r--r--   0        0        0      805 2024-02-29 19:53:45.029280 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_message_param.py
+-rw-r--r--   0        0        0      867 2024-02-29 19:53:45.029390 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_message_tool_call.py
+-rw-r--r--   0        0        0      976 2024-02-29 19:53:45.029472 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_message_tool_call_param.py
+-rw-r--r--   0        0        0      536 2024-02-29 19:53:45.029558 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_named_tool_choice_param.py
+-rw-r--r--   0        0        0      207 2024-02-29 19:53:45.029628 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_role.py
+-rw-r--r--   0        0        0      605 2024-02-29 19:53:45.029701 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_system_message_param.py
+-rw-r--r--   0        0        0     1440 2024-02-29 19:53:45.029779 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_token_logprob.py
+-rw-r--r--   0        0        0      399 2024-02-29 19:53:45.029842 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_tool_choice_option_param.py
+-rw-r--r--   0        0        0      520 2024-02-29 19:53:45.029912 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_tool_message_param.py
+-rw-r--r--   0        0        0      452 2024-02-29 19:53:45.029988 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_tool_param.py
+-rw-r--r--   0        0        0      759 2024-02-29 19:53:45.030069 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_user_message_param.py
+-rw-r--r--   0        0        0    10599 2024-02-29 19:53:45.030179 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/completion_create_params.py
+-rw-r--r--   0        0        0     1139 2024-02-29 19:53:45.030297 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/completion.py
+-rw-r--r--   0        0        0      932 2024-02-29 19:53:45.030410 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/completion_choice.py
+-rw-r--r--   0        0        0     7223 2024-02-29 19:53:45.030573 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/completion_create_params.py
+-rw-r--r--   0        0        0      401 2024-02-29 19:53:45.030763 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/completion_usage.py
+-rw-r--r--   0        0        0      765 2024-02-29 19:53:45.030878 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/create_embedding_response.py
+-rw-r--r--   0        0        0      604 2024-02-29 19:53:45.030960 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/embedding.py
+-rw-r--r--   0        0        0     1852 2024-02-29 19:53:45.031044 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/embedding_create_params.py
+-rw-r--r--   0        0        0      100 2024-02-29 19:53:45.031116 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/file_content.py
+-rw-r--r--   0        0        0      840 2024-02-29 19:53:45.031201 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/file_create_params.py
+-rw-r--r--   0        0        0      244 2024-02-29 19:53:45.031283 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/file_deleted.py
+-rw-r--r--   0        0        0      277 2024-02-29 19:53:45.031367 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/file_list_params.py
+-rw-r--r--   0        0        0     1193 2024-02-29 19:53:45.031461 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/file_object.py
+-rw-r--r--   0        0        0      431 2024-02-29 19:53:45.031698 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/fine_tuning/__init__.py
+-rw-r--r--   0        0        0      560 2024-02-29 20:11:49.007978 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/fine_tuning/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1598 2024-02-29 20:11:49.008618 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/fine_tuning/__pycache__/fine_tuning_job.cpython-310.pyc
+-rw-r--r--   0        0        0      684 2024-02-29 20:11:49.013635 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/fine_tuning/__pycache__/fine_tuning_job_event.cpython-310.pyc
+-rw-r--r--   0        0        0     1160 2024-02-29 20:11:49.012393 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/fine_tuning/__pycache__/job_create_params.cpython-310.pyc
+-rw-r--r--   0        0        0      595 2024-02-29 20:11:49.014930 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/fine_tuning/__pycache__/job_list_events_params.cpython-310.pyc
+-rw-r--r--   0        0        0      582 2024-02-29 20:11:49.011903 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/fine_tuning/__pycache__/job_list_params.cpython-310.pyc
+-rw-r--r--   0        0        0     3312 2024-02-29 19:53:45.031854 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/fine_tuning/fine_tuning_job.py
+-rw-r--r--   0        0        0      341 2024-02-29 19:53:45.031945 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/fine_tuning/fine_tuning_job_event.py
+-rw-r--r--   0        0        0     2578 2024-02-29 19:53:45.032060 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/fine_tuning/job_create_params.py
+-rw-r--r--   0        0        0      367 2024-02-29 19:53:45.032160 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/fine_tuning/job_list_events_params.py
+-rw-r--r--   0        0        0      363 2024-02-29 19:53:45.032229 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/fine_tuning/job_list_params.py
+-rw-r--r--   0        0        0      574 2024-02-29 19:53:45.032319 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/image.py
+-rw-r--r--   0        0        0     1342 2024-02-29 19:53:45.032411 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/image_create_variation_params.py
+-rw-r--r--   0        0        0     1702 2024-02-29 19:53:45.032482 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/image_edit_params.py
+-rw-r--r--   0        0        0     2008 2024-02-29 19:53:45.032563 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/image_generate_params.py
+-rw-r--r--   0        0        0      241 2024-02-29 19:53:45.032629 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/images_response.py
+-rw-r--r--   0        0        0      499 2024-02-29 19:53:45.032733 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/model.py
+-rw-r--r--   0        0        0      195 2024-02-29 19:53:45.032829 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/model_deleted.py
+-rw-r--r--   0        0        0     3946 2024-02-29 19:53:45.032928 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/moderation.py
+-rw-r--r--   0        0        0      921 2024-02-29 19:53:45.033016 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/moderation_create_params.py
+-rw-r--r--   0        0        0      451 2024-02-29 19:53:45.033086 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/moderation_create_response.py
+-rw-r--r--   0        0        0      202 2024-02-29 19:53:45.033209 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/shared/__init__.py
+-rw-r--r--   0        0        0      335 2024-02-29 20:11:45.294228 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/shared/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      689 2024-02-29 20:11:45.294720 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/shared/__pycache__/function_definition.cpython-310.pyc
+-rw-r--r--   0        0        0      326 2024-02-29 20:11:45.295085 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/shared/__pycache__/function_parameters.cpython-310.pyc
+-rw-r--r--   0        0        0     1034 2024-02-29 19:53:45.033313 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/shared/function_definition.py
+-rw-r--r--   0        0        0      152 2024-02-29 19:53:45.033381 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/shared/function_parameters.py
+-rw-r--r--   0        0        0      202 2024-02-29 19:53:45.033475 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/shared_params/__init__.py
+-rw-r--r--   0        0        0      342 2024-02-29 20:11:45.370593 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/shared_params/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      735 2024-02-29 20:11:45.371046 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/shared_params/__pycache__/function_definition.cpython-310.pyc
+-rw-r--r--   0        0        0      379 2024-02-29 20:11:45.371530 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/shared_params/__pycache__/function_parameters.cpython-310.pyc
+-rw-r--r--   0        0        0     1045 2024-02-29 19:53:45.033543 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/shared_params/function_definition.py
+-rw-r--r--   0        0        0      188 2024-02-29 19:53:45.033602 notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/shared_params/function_parameters.py
+-rw-r--r--   0        0        0       62 2024-02-29 19:53:45.034068 notdiamond-0.1.0a9/notdiamond/openai/src/openai/version.py
+-rw-r--r--   0        0        0       53 2024-02-29 19:53:45.034185 notdiamond-0.1.0a9/notdiamond/openai/tests/__init__.py
+-rw-r--r--   0        0        0      193 2024-03-01 15:43:17.169340 notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1900 2024-03-01 15:43:17.171904 notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/conftest.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0     1900 2024-03-06 14:07:01.691582 notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/conftest.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0    55728 2024-03-01 15:43:17.978233 notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_client.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0    55728 2024-03-06 14:07:02.659384 notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_client.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0     3181 2024-03-01 15:43:17.999785 notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_deepcopy.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0     3181 2024-03-06 14:07:02.683485 notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_deepcopy.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0     4422 2024-03-01 15:43:18.006049 notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_extract_files.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0     4422 2024-03-06 14:07:02.688934 notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_extract_files.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0     4055 2024-03-01 15:43:18.010620 notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_files.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0     4055 2024-03-06 14:07:02.693989 notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_files.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0     3161 2024-03-01 15:43:18.016784 notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_legacy_response.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0     3161 2024-03-06 14:07:02.702024 notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_legacy_response.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0    56374 2024-03-01 15:43:18.078942 notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_models.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0    56374 2024-03-06 14:07:02.825206 notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_models.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0    13057 2024-03-01 15:43:18.148960 notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_module_client.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0    13057 2024-03-06 14:07:02.842384 notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_module_client.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0     8287 2024-03-01 15:43:18.169284 notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_qs.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0     8287 2024-03-06 14:07:02.858033 notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_qs.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0     7371 2024-03-01 15:43:18.176395 notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_required_args.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0     7371 2024-03-06 14:07:02.866623 notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_required_args.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0     8431 2024-03-01 15:43:18.183627 notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_response.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0     8431 2024-03-06 14:07:02.874776 notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_response.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0     6263 2024-03-01 15:43:18.194766 notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_streaming.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0     6263 2024-03-06 14:07:02.883734 notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_streaming.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0    23550 2024-03-01 15:43:18.218793 notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_transform.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0    23550 2024-03-06 14:07:02.910164 notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_transform.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0       53 2024-02-29 19:53:45.034297 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/__init__.py
+-rw-r--r--   0        0        0      207 2024-03-01 15:43:17.178166 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    11419 2024-03-01 15:43:17.729416 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/__pycache__/test_completions.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0    11419 2024-03-06 14:07:02.384476 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/__pycache__/test_completions.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0     6349 2024-03-01 15:43:17.740226 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/__pycache__/test_embeddings.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0     6349 2024-03-06 14:07:02.397400 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/__pycache__/test_embeddings.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0    25185 2024-03-01 15:43:17.773350 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/__pycache__/test_files.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0    25185 2024-03-06 14:07:02.433171 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/__pycache__/test_files.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0    12139 2024-03-01 15:43:17.795628 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/__pycache__/test_images.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0    12139 2024-03-06 14:07:02.457880 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/__pycache__/test_images.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0    11404 2024-03-01 15:43:17.822202 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/__pycache__/test_models.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0    11404 2024-03-06 14:07:02.534076 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/__pycache__/test_models.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0     6213 2024-03-01 15:43:17.835417 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/__pycache__/test_moderations.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0     6213 2024-03-06 14:07:02.546174 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/__pycache__/test_moderations.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0       53 2024-02-29 19:53:45.034444 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/audio/__init__.py
+-rw-r--r--   0        0        0      213 2024-03-01 15:43:17.178726 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/audio/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     8738 2024-03-01 15:43:17.187953 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/audio/__pycache__/test_speech.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0     8738 2024-03-06 14:07:01.707035 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/audio/__pycache__/test_speech.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0     6471 2024-03-01 15:43:17.365949 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/audio/__pycache__/test_transcriptions.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0     6471 2024-03-06 14:07:01.937439 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/audio/__pycache__/test_transcriptions.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0     6363 2024-03-01 15:43:17.376705 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/audio/__pycache__/test_translations.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0     6363 2024-03-06 14:07:01.951055 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/audio/__pycache__/test_translations.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0     5750 2024-02-29 19:53:45.034582 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/audio/test_speech.py
+-rw-r--r--   0        0        0     4391 2024-02-29 19:53:45.034661 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/audio/test_transcriptions.py
+-rw-r--r--   0        0        0     4149 2024-02-29 19:53:45.034870 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/audio/test_translations.py
+-rw-r--r--   0        0        0       53 2024-02-29 19:53:45.035011 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/__init__.py
+-rw-r--r--   0        0        0      212 2024-03-01 15:43:17.383638 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    17950 2024-03-01 15:43:17.434648 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/__pycache__/test_assistants.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0    17950 2024-03-06 14:07:02.066854 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/__pycache__/test_assistants.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0    17770 2024-03-01 15:43:17.465122 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/__pycache__/test_threads.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0    17770 2024-03-06 14:07:02.116507 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/__pycache__/test_threads.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0       53 2024-02-29 19:53:45.035185 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/assistants/__init__.py
+-rw-r--r--   0        0        0      223 2024-03-01 15:43:17.384451 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/assistants/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    16689 2024-03-01 15:43:17.403120 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/assistants/__pycache__/test_files.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0    16689 2024-03-06 14:07:01.979367 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/assistants/__pycache__/test_files.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0    15388 2024-02-29 19:53:45.035303 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/assistants/test_files.py
+-rw-r--r--   0        0        0       53 2024-02-29 19:53:45.035415 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/chat/__init__.py
+-rw-r--r--   0        0        0    17298 2024-02-29 19:53:45.035495 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/test_assistants.py
+-rw-r--r--   0        0        0    18678 2024-02-29 19:53:45.035624 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/test_threads.py
+-rw-r--r--   0        0        0       53 2024-02-29 19:53:45.035742 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/threads/__init__.py
+-rw-r--r--   0        0        0      220 2024-03-01 15:43:17.474843 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/threads/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    17836 2024-03-01 15:43:17.576555 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/threads/__pycache__/test_messages.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0    17836 2024-03-06 14:07:02.204584 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/threads/__pycache__/test_messages.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0    21240 2024-03-01 15:43:17.615039 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/threads/__pycache__/test_runs.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0    21240 2024-03-06 14:07:02.243966 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/threads/__pycache__/test_runs.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0       53 2024-02-29 19:53:45.035862 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/threads/messages/__init__.py
+-rw-r--r--   0        0        0      229 2024-03-01 15:43:17.475394 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/threads/messages/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    12104 2024-03-01 15:43:17.532189 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/threads/messages/__pycache__/test_files.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0    12104 2024-03-06 14:07:02.145196 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/threads/messages/__pycache__/test_files.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0    10298 2024-02-29 19:53:45.035942 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/threads/messages/test_files.py
+-rw-r--r--   0        0        0       53 2024-02-29 19:53:45.036163 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/threads/runs/__init__.py
+-rw-r--r--   0        0        0      225 2024-03-01 15:43:17.540244 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/threads/runs/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    12015 2024-03-01 15:43:17.549749 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/threads/runs/__pycache__/test_steps.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0    12015 2024-03-06 14:07:02.175253 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/threads/runs/__pycache__/test_steps.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0     9914 2024-02-29 19:53:45.036293 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/threads/runs/test_steps.py
+-rw-r--r--   0        0        0    16951 2024-02-29 19:53:45.036439 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/threads/test_messages.py
+-rw-r--r--   0        0        0    24332 2024-02-29 19:53:45.036597 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/threads/test_runs.py
+-rw-r--r--   0        0        0       53 2024-02-29 19:53:45.036745 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/chat/__init__.py
+-rw-r--r--   0        0        0      212 2024-03-01 15:43:17.626537 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/chat/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    12617 2024-03-01 15:43:17.636395 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/chat/__pycache__/test_completions.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0    12617 2024-03-06 14:07:02.324400 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/chat/__pycache__/test_completions.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0    15543 2024-02-29 19:53:45.036856 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/chat/test_completions.py
+-rw-r--r--   0        0        0       53 2024-02-29 19:53:45.036977 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/fine_tuning/__init__.py
+-rw-r--r--   0        0        0      219 2024-03-01 15:43:17.643705 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/fine_tuning/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    20186 2024-03-01 15:43:17.665860 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/fine_tuning/__pycache__/test_jobs.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0    20186 2024-03-06 14:07:02.364798 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/fine_tuning/__pycache__/test_jobs.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0    17397 2024-02-29 19:53:45.037119 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/fine_tuning/test_jobs.py
+-rw-r--r--   0        0        0     8682 2024-02-29 19:53:45.037231 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/test_completions.py
+-rw-r--r--   0        0        0     4469 2024-02-29 19:53:45.037348 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/test_embeddings.py
+-rw-r--r--   0        0        0    19256 2024-02-29 19:53:45.037503 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/test_files.py
+-rw-r--r--   0        0        0    11122 2024-02-29 19:53:45.037622 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/test_images.py
+-rw-r--r--   0        0        0     8691 2024-02-29 19:53:45.037707 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/test_models.py
+-rw-r--r--   0        0        0     3862 2024-02-29 19:53:45.037781 notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/test_moderations.py
+-rw-r--r--   0        0        0     1425 2024-02-29 19:53:45.037865 notdiamond-0.1.0a9/notdiamond/openai/tests/conftest.py
+-rw-r--r--   0        0        0     2773 2024-03-01 15:43:17.842433 notdiamond-0.1.0a9/notdiamond/openai/tests/lib/__pycache__/test_azure.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0     2773 2024-03-06 14:07:02.553845 notdiamond-0.1.0a9/notdiamond/openai/tests/lib/__pycache__/test_azure.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0      900 2024-03-01 15:43:17.858421 notdiamond-0.1.0a9/notdiamond/openai/tests/lib/__pycache__/test_old_api.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0      900 2024-03-06 14:07:02.571581 notdiamond-0.1.0a9/notdiamond/openai/tests/lib/__pycache__/test_old_api.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0     1792 2024-02-29 19:53:45.037989 notdiamond-0.1.0a9/notdiamond/openai/tests/lib/test_azure.py
+-rw-r--r--   0        0        0      424 2024-02-29 19:53:45.038066 notdiamond-0.1.0a9/notdiamond/openai/tests/lib/test_old_api.py
+-rw-r--r--   0        0        0    57182 2024-02-29 19:53:45.038323 notdiamond-0.1.0a9/notdiamond/openai/tests/test_client.py
+-rw-r--r--   0        0        0     1564 2024-02-29 19:53:45.038414 notdiamond-0.1.0a9/notdiamond/openai/tests/test_deepcopy.py
+-rw-r--r--   0        0        0     1939 2024-02-29 19:53:45.038495 notdiamond-0.1.0a9/notdiamond/openai/tests/test_extract_files.py
+-rw-r--r--   0        0        0     1576 2024-02-29 19:53:45.038574 notdiamond-0.1.0a9/notdiamond/openai/tests/test_files.py
+-rw-r--r--   0        0        0     1710 2024-02-29 19:53:45.038662 notdiamond-0.1.0a9/notdiamond/openai/tests/test_legacy_response.py
+-rw-r--r--   0        0        0    16286 2024-02-29 19:53:45.038772 notdiamond-0.1.0a9/notdiamond/openai/tests/test_models.py
+-rw-r--r--   0        0        0     5453 2024-02-29 19:53:45.038852 notdiamond-0.1.0a9/notdiamond/openai/tests/test_module_client.py
+-rw-r--r--   0        0        0     3200 2024-02-29 19:53:45.038924 notdiamond-0.1.0a9/notdiamond/openai/tests/test_qs.py
+-rw-r--r--   0        0        0     3057 2024-02-29 19:53:45.038999 notdiamond-0.1.0a9/notdiamond/openai/tests/test_required_args.py
+-rw-r--r--   0        0        0     4572 2024-02-29 19:53:45.039060 notdiamond-0.1.0a9/notdiamond/openai/tests/test_response.py
+-rw-r--r--   0        0        0     2302 2024-02-29 19:53:45.039141 notdiamond-0.1.0a9/notdiamond/openai/tests/test_streaming.py
+-rw-r--r--   0        0        0     9933 2024-02-29 19:53:45.039235 notdiamond-0.1.0a9/notdiamond/openai/tests/test_transform.py
+-rw-r--r--   0        0        0     3105 2024-03-01 15:43:18.227994 notdiamond-0.1.0a9/notdiamond/openai/tests/test_utils/__pycache__/test_proxy.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0     3105 2024-03-06 14:07:02.919163 notdiamond-0.1.0a9/notdiamond/openai/tests/test_utils/__pycache__/test_proxy.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0     5671 2024-03-01 15:43:18.234937 notdiamond-0.1.0a9/notdiamond/openai/tests/test_utils/__pycache__/test_typing.cpython-310-pytest-8.0.0.pyc
+-rw-r--r--   0        0        0     5671 2024-03-06 14:07:02.926971 notdiamond-0.1.0a9/notdiamond/openai/tests/test_utils/__pycache__/test_typing.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0      687 2024-02-29 19:53:45.039383 notdiamond-0.1.0a9/notdiamond/openai/tests/test_utils/test_proxy.py
+-rw-r--r--   0        0        0     2477 2024-02-29 19:53:45.039460 notdiamond-0.1.0a9/notdiamond/openai/tests/test_utils/test_typing.py
+-rw-r--r--   0        0        0     3850 2024-02-29 19:53:45.039546 notdiamond-0.1.0a9/notdiamond/openai/tests/utils.py
+-rw-r--r--   0        0        0        0 2024-01-22 13:51:23.617800 notdiamond-0.1.0a9/notdiamond/prompts/__init__.py
+-rw-r--r--   0        0        0      346 2024-02-19 19:24:39.601816 notdiamond-0.1.0a9/notdiamond/prompts/hash.py
+-rw-r--r--   0        0        0     7378 2024-02-29 15:13:41.623628 notdiamond-0.1.0a9/notdiamond/prompts/prompt.py
+-rw-r--r--   0        0        0      688 2024-03-06 08:03:55.584981 notdiamond-0.1.0a9/notdiamond/settings.py
+-rw-r--r--   0        0        0      611 2024-02-19 19:24:39.602110 notdiamond-0.1.0a9/notdiamond/types.py
+-rw-r--r--   0        0        0      646 2024-03-06 14:08:57.942498 notdiamond-0.1.0a9/pyproject.toml
+-rw-r--r--   0        0        0     1352 1970-01-01 00:00:00.000000 notdiamond-0.1.0a9/PKG-INFO
```

### Comparing `notdiamond-0.1.0a8/README.md` & `notdiamond-0.1.0a9/README.md`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/llms/llm.py` & `notdiamond-0.1.0a9/notdiamond/llms/llm.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/llms/provider.py` & `notdiamond-0.1.0a9/notdiamond/llms/provider.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/llms/request.py` & `notdiamond-0.1.0a9/notdiamond/llms/request.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/metrics/metric.py` & `notdiamond-0.1.0a9/notdiamond/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/metrics/request.py` & `notdiamond-0.1.0a9/notdiamond/metrics/request.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/.devcontainer/devcontainer.json` & `notdiamond-0.1.0a9/notdiamond/openai/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/.github/ISSUE_TEMPLATE/bug_report.yml` & `notdiamond-0.1.0a9/notdiamond/openai/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/.github/ISSUE_TEMPLATE/feature_request.yml` & `notdiamond-0.1.0a9/notdiamond/openai/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/.github/workflows/ci.yml` & `notdiamond-0.1.0a9/notdiamond/openai/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/.github/workflows/create-releases.yml` & `notdiamond-0.1.0a9/notdiamond/openai/.github/workflows/create-releases.yml`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/.github/workflows/publish-pypi.yml` & `notdiamond-0.1.0a9/notdiamond/openai/.github/workflows/publish-pypi.yml`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/.github/workflows/release-doctor.yml` & `notdiamond-0.1.0a9/notdiamond/openai/.github/workflows/release-doctor.yml`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/CHANGELOG.md` & `notdiamond-0.1.0a9/notdiamond/openai/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/CONTRIBUTING.md` & `notdiamond-0.1.0a9/notdiamond/openai/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/LICENSE` & `notdiamond-0.1.0a9/notdiamond/openai/LICENSE`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/README.md` & `notdiamond-0.1.0a9/notdiamond/openai/README.md`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/api.md` & `notdiamond-0.1.0a9/notdiamond/openai/api.md`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/bin/check-env-state.py` & `notdiamond-0.1.0a9/notdiamond/openai/bin/check-env-state.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/bin/check-release-environment` & `notdiamond-0.1.0a9/notdiamond/openai/bin/check-release-environment`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/bin/check-test-server` & `notdiamond-0.1.0a9/notdiamond/openai/bin/check-test-server`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/bin/ruffen-docs.py` & `notdiamond-0.1.0a9/notdiamond/openai/bin/ruffen-docs.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/examples/assistant.py` & `notdiamond-0.1.0a9/notdiamond/openai/examples/assistant.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/examples/audio.py` & `notdiamond-0.1.0a9/notdiamond/openai/examples/audio.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/examples/azure.py` & `notdiamond-0.1.0a9/notdiamond/openai/examples/azure.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/examples/azure_ad.py` & `notdiamond-0.1.0a9/notdiamond/openai/examples/azure_ad.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/examples/demo.py` & `notdiamond-0.1.0a9/notdiamond/openai/examples/demo.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/examples/module_client.py` & `notdiamond-0.1.0a9/notdiamond/openai/examples/module_client.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/examples/streaming.py` & `notdiamond-0.1.0a9/notdiamond/openai/examples/streaming.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/mypy.ini` & `notdiamond-0.1.0a9/notdiamond/openai/mypy.ini`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/pyproject.toml` & `notdiamond-0.1.0a9/notdiamond/openai/pyproject.toml`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/release-please-config.json` & `notdiamond-0.1.0a9/notdiamond/openai/release-please-config.json`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/requirements-dev.lock` & `notdiamond-0.1.0a9/notdiamond/openai/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/requirements.lock` & `notdiamond-0.1.0a9/notdiamond/openai/requirements.lock`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/__init__.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/__init__.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/_base_client.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/_base_client.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/_client.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/_client.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/_compat.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/_compat.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/_constants.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/_constants.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/_exceptions.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/_exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/_files.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/_files.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/_legacy_response.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/_legacy_response.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/_models.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/_models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/_module_client.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/_module_client.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/_qs.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/_qs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/_resource.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/_resource.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/_response.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/_response.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/_streaming.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/_streaming.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/_types.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/_types.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/__pycache__/pagination.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/__pycache__/pagination.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_base_client.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_base_client.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_client.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_client.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_compat.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_compat.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_exceptions.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_exceptions.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_extras/__pycache__/_common.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_extras/__pycache__/_common.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_extras/__pycache__/numpy_proxy.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_extras/__pycache__/numpy_proxy.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_extras/__pycache__/pandas_proxy.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_extras/__pycache__/pandas_proxy.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_extras/numpy_proxy.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_extras/numpy_proxy.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_extras/pandas_proxy.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_extras/pandas_proxy.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_files.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_files.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_legacy_response.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_legacy_response.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_models.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_models.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_module_client.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_module_client.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_qs.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_qs.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_resource.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_resource.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_response.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_response.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_streaming.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_streaming.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_types.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_types.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/__init__.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/__pycache__/__init__.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/__pycache__/_logs.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/__pycache__/_logs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/__pycache__/_proxy.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/__pycache__/_proxy.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/__pycache__/_streams.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/__pycache__/_streams.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/__pycache__/_sync.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/__pycache__/_sync.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/__pycache__/_transform.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/__pycache__/_transform.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/__pycache__/_typing.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/__pycache__/_typing.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/__pycache__/_utils.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/__pycache__/_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/_logs.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/_proxy.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/_sync.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/_transform.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/_typing.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/_utils/_utils.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/_api/audio.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/_api/audio.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/_api/chat/completions.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/_api/chat/completions.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/_api/completions.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/_api/completions.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/_api/files.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/_api/files.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/_api/image.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/_api/image.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/_api/models.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/_api/models.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/_cli.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/_cli.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/_progress.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/_progress.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/_tools/fine_tunes.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/_tools/fine_tunes.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/_tools/migrate.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/_tools/migrate.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/cli/_utils.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/cli/_utils.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/lib/__pycache__/_old_api.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/lib/__pycache__/_old_api.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/lib/__pycache__/azure.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/lib/__pycache__/azure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/lib/_old_api.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/lib/_old_api.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/lib/_validators.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/lib/_validators.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/lib/azure.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/lib/azure.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/pagination.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/pagination.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/__init__.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/__pycache__/__init__.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/__pycache__/completions.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/__pycache__/completions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/__pycache__/embeddings.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/__pycache__/embeddings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/__pycache__/files.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/__pycache__/files.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/__pycache__/images.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/__pycache__/images.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/__pycache__/models.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/__pycache__/models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/__pycache__/moderations.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/__pycache__/moderations.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/audio/__init__.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/audio/__pycache__/__init__.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/audio/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/audio/__pycache__/audio.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/audio/__pycache__/audio.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/audio/__pycache__/speech.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/audio/__pycache__/speech.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/audio/__pycache__/transcriptions.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/audio/__pycache__/transcriptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/audio/__pycache__/translations.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/audio/__pycache__/translations.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/audio/audio.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/audio/audio.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/audio/speech.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/audio/speech.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/audio/transcriptions.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/audio/transcriptions.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/audio/translations.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/audio/translations.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/__init__.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/__pycache__/__init__.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/__pycache__/beta.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/__pycache__/beta.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/assistants/__init__.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/assistants/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/assistants/__pycache__/__init__.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/assistants/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/assistants/__pycache__/assistants.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/assistants/__pycache__/assistants.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/assistants/__pycache__/files.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/assistants/__pycache__/files.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/assistants/assistants.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/assistants/assistants.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/assistants/files.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/assistants/files.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/beta.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/beta.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/__init__.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/__pycache__/__init__.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/__pycache__/threads.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/__pycache__/threads.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/messages/__init__.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/messages/__pycache__/__init__.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/messages/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/messages/__pycache__/files.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/messages/__pycache__/files.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/messages/__pycache__/messages.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/messages/__pycache__/messages.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/messages/files.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/messages/files.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/messages/messages.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/messages/messages.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/runs/__init__.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/runs/__pycache__/__init__.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/runs/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/runs/__pycache__/runs.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/runs/__pycache__/runs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/runs/__pycache__/steps.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/runs/__pycache__/steps.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/runs/runs.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/runs/runs.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/runs/steps.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/runs/steps.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/beta/threads/threads.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/beta/threads/threads.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/chat/__init__.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/chat/__pycache__/__init__.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/chat/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/chat/__pycache__/chat.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/chat/__pycache__/chat.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/chat/__pycache__/completions.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/chat/__pycache__/completions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/chat/chat.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/chat/chat.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/chat/completions.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/chat/completions.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/completions.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/completions.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/embeddings.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/embeddings.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/files.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/files.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/fine_tuning/__init__.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/fine_tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/fine_tuning/__pycache__/__init__.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/fine_tuning/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/fine_tuning/__pycache__/fine_tuning.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/fine_tuning/__pycache__/fine_tuning.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/fine_tuning/__pycache__/jobs.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/fine_tuning/__pycache__/jobs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/fine_tuning/fine_tuning.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/fine_tuning/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/fine_tuning/jobs.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/fine_tuning/jobs.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/images.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/images.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/models.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/models.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/resources/moderations.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/resources/moderations.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__init__.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/__init__.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/completion.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/completion.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/completion_choice.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/completion_choice.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/completion_create_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/completion_create_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/completion_usage.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/completion_usage.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/create_embedding_response.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/create_embedding_response.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/embedding.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/embedding.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/embedding_create_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/embedding_create_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/file_create_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/file_create_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/file_deleted.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/file_deleted.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/file_list_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/file_list_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/file_object.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/file_object.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/image.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/image.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/image_create_variation_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/image_create_variation_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/image_edit_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/image_edit_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/image_generate_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/image_generate_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/images_response.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/images_response.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/model.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/moderation.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/moderation.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/moderation_create_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/moderation_create_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/__pycache__/moderation_create_response.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/__pycache__/moderation_create_response.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/audio/__pycache__/__init__.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/audio/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/audio/__pycache__/speech_create_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/audio/__pycache__/speech_create_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/audio/__pycache__/transcription_create_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/audio/__pycache__/transcription_create_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/audio/__pycache__/translation_create_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/audio/__pycache__/translation_create_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/audio/speech_create_params.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/audio/speech_create_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/audio/transcription_create_params.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/audio/transcription_create_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/audio/translation_create_params.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/audio/translation_create_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/__init__.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/__pycache__/__init__.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/__pycache__/assistant.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/__pycache__/assistant.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/__pycache__/assistant_create_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/__pycache__/assistant_create_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/__pycache__/assistant_deleted.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/__pycache__/assistant_deleted.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/__pycache__/assistant_list_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/__pycache__/assistant_list_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/__pycache__/assistant_update_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/__pycache__/assistant_update_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/__pycache__/thread.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/__pycache__/thread.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/__pycache__/thread_create_and_run_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/__pycache__/thread_create_and_run_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/__pycache__/thread_create_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/__pycache__/thread_create_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/__pycache__/thread_deleted.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/__pycache__/thread_deleted.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/__pycache__/thread_update_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/__pycache__/thread_update_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/assistant.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/assistant.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/assistant_create_params.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/assistant_create_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/assistant_list_params.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/assistant_list_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/assistant_update_params.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/assistant_update_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/assistants/__pycache__/assistant_file.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/assistants/__pycache__/assistant_file.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/assistants/__pycache__/file_create_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/assistants/__pycache__/file_create_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/assistants/__pycache__/file_delete_response.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/assistants/__pycache__/file_delete_response.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/assistants/__pycache__/file_list_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/assistants/__pycache__/file_list_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/assistants/assistant_file.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/assistants/assistant_file.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/assistants/file_list_params.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/assistants/file_list_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/thread.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/thread.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/thread_create_and_run_params.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/thread_create_and_run_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/thread_create_params.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/thread_create_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/thread_update_params.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/thread_update_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/__init__.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/__pycache__/__init__.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/__pycache__/message_content_image_file.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/__pycache__/message_content_image_file.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/__pycache__/message_content_text.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/__pycache__/message_content_text.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/__pycache__/message_create_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/__pycache__/message_create_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/__pycache__/message_list_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/__pycache__/message_list_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/__pycache__/message_update_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/__pycache__/message_update_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/__pycache__/required_action_function_tool_call.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/__pycache__/required_action_function_tool_call.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/__pycache__/run.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/__pycache__/run.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/__pycache__/run_create_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/__pycache__/run_create_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/__pycache__/run_list_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/__pycache__/run_list_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/__pycache__/run_submit_tool_outputs_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/__pycache__/run_submit_tool_outputs_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/__pycache__/run_update_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/__pycache__/run_update_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/__pycache__/thread_message.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/__pycache__/thread_message.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/message_content_text.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/message_content_text.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/message_create_params.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/message_create_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/message_list_params.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/message_list_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/message_update_params.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/message_update_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/messages/__pycache__/file_list_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/messages/__pycache__/file_list_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/messages/__pycache__/message_file.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/messages/__pycache__/message_file.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/messages/file_list_params.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/messages/file_list_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/messages/message_file.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/messages/message_file.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/required_action_function_tool_call.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/required_action_function_tool_call.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/run.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/run.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/run_create_params.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/run_create_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/run_list_params.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/run_list_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/run_submit_tool_outputs_params.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/run_submit_tool_outputs_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/run_update_params.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/run_update_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/__init__.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/__init__.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/code_tool_call.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/code_tool_call.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/function_tool_call.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/function_tool_call.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/message_creation_step_details.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/message_creation_step_details.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/retrieval_tool_call.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/retrieval_tool_call.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/run_step.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/run_step.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/step_list_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/step_list_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/tool_calls_step_details.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/__pycache__/tool_calls_step_details.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/code_tool_call.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/code_tool_call.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/function_tool_call.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/function_tool_call.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/run_step.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/run_step.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/step_list_params.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/step_list_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/runs/tool_calls_step_details.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/runs/tool_calls_step_details.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/beta/threads/thread_message.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/beta/threads/thread_message.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__init__.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/__init__.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_assistant_message_param.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_assistant_message_param.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_chunk.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_chunk.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_content_part_image_param.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_content_part_image_param.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_content_part_param.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_content_part_param.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_content_part_text_param.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_content_part_text_param.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_function_call_option_param.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_function_call_option_param.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_function_message_param.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_function_message_param.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_message.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_message.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_message_param.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_message_param.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_message_tool_call.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_message_tool_call.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_message_tool_call_param.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_message_tool_call_param.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_named_tool_choice_param.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_named_tool_choice_param.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_system_message_param.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_system_message_param.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_token_logprob.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_token_logprob.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_tool_choice_option_param.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_tool_choice_option_param.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_tool_message_param.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_tool_message_param.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_tool_param.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_tool_param.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_user_message_param.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/chat_completion_user_message_param.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/__pycache__/completion_create_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/__pycache__/completion_create_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_assistant_message_param.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_assistant_message_param.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_chunk.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_chunk.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_content_part_image_param.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_content_part_image_param.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_function_message_param.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_function_message_param.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_message.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_message.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_message_param.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_message_param.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_message_tool_call.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_message_tool_call.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_message_tool_call_param.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_message_tool_call_param.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_named_tool_choice_param.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_named_tool_choice_param.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_system_message_param.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_system_message_param.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_token_logprob.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_token_logprob.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_tool_message_param.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_tool_message_param.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/chat_completion_user_message_param.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/chat_completion_user_message_param.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/chat/completion_create_params.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/chat/completion_create_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/completion.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/completion.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/completion_choice.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/completion_choice.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/completion_create_params.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/completion_create_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/create_embedding_response.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/create_embedding_response.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/embedding.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/embedding.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/embedding_create_params.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/embedding_create_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/file_create_params.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/file_create_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/file_object.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/file_object.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/fine_tuning/__pycache__/__init__.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/fine_tuning/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/fine_tuning/__pycache__/fine_tuning_job.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/fine_tuning/__pycache__/fine_tuning_job.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/fine_tuning/__pycache__/fine_tuning_job_event.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/fine_tuning/__pycache__/fine_tuning_job_event.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/fine_tuning/__pycache__/job_create_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/fine_tuning/__pycache__/job_create_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/fine_tuning/__pycache__/job_list_events_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/fine_tuning/__pycache__/job_list_events_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/fine_tuning/__pycache__/job_list_params.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/fine_tuning/__pycache__/job_list_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/fine_tuning/fine_tuning_job.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/fine_tuning/fine_tuning_job.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/fine_tuning/job_create_params.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/fine_tuning/job_create_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/image.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/image.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/image_create_variation_params.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/image_create_variation_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/image_edit_params.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/image_edit_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/image_generate_params.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/image_generate_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/moderation.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/moderation.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/moderation_create_params.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/moderation_create_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/shared/__pycache__/function_definition.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/shared/__pycache__/function_definition.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/shared/function_definition.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/shared/function_definition.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/shared_params/__pycache__/function_definition.cpython-310.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/shared_params/__pycache__/function_definition.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/src/openai/types/shared_params/function_definition.py` & `notdiamond-0.1.0a9/notdiamond/openai/src/openai/types/shared_params/function_definition.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/__pycache__/conftest.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/conftest.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/__pycache__/test_client.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_client.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/__pycache__/test_deepcopy.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_deepcopy.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/__pycache__/test_extract_files.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_extract_files.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/__pycache__/test_files.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_files.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/__pycache__/test_legacy_response.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_legacy_response.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/__pycache__/test_models.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_models.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/__pycache__/test_module_client.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_module_client.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/__pycache__/test_qs.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_qs.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/__pycache__/test_required_args.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_required_args.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/__pycache__/test_response.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_response.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/__pycache__/test_streaming.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_streaming.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/__pycache__/test_transform.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/__pycache__/test_transform.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/__pycache__/test_completions.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/__pycache__/test_completions.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/__pycache__/test_embeddings.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/__pycache__/test_embeddings.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/__pycache__/test_files.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/__pycache__/test_files.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/__pycache__/test_images.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/__pycache__/test_images.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/__pycache__/test_models.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/__pycache__/test_models.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/__pycache__/test_moderations.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/__pycache__/test_moderations.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/audio/__pycache__/test_speech.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/audio/__pycache__/test_speech.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/audio/__pycache__/test_transcriptions.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/audio/__pycache__/test_transcriptions.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/audio/__pycache__/test_translations.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/audio/__pycache__/test_translations.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/audio/test_speech.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/audio/test_speech.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/audio/test_transcriptions.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/audio/test_transcriptions.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/audio/test_translations.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/audio/test_translations.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/__pycache__/test_assistants.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/__pycache__/test_assistants.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/__pycache__/test_threads.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/__pycache__/test_threads.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/assistants/__pycache__/test_files.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/assistants/__pycache__/test_files.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/assistants/test_files.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/assistants/test_files.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/test_assistants.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/test_assistants.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/test_threads.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/test_threads.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/threads/__pycache__/test_messages.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/threads/__pycache__/test_messages.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/threads/__pycache__/test_runs.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/threads/__pycache__/test_runs.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/threads/messages/__pycache__/test_files.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/threads/messages/__pycache__/test_files.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/threads/messages/test_files.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/threads/messages/test_files.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/threads/runs/__pycache__/test_steps.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/threads/runs/__pycache__/test_steps.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/threads/runs/test_steps.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/threads/runs/test_steps.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/threads/test_messages.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/threads/test_messages.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/beta/threads/test_runs.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/beta/threads/test_runs.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/chat/__pycache__/test_completions.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/chat/__pycache__/test_completions.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/chat/test_completions.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/chat/test_completions.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/fine_tuning/__pycache__/test_jobs.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/fine_tuning/__pycache__/test_jobs.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/fine_tuning/test_jobs.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/fine_tuning/test_jobs.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/test_completions.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/test_completions.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/test_embeddings.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/test_files.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/test_files.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/test_images.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/test_images.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/test_models.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/test_models.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/api_resources/test_moderations.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/api_resources/test_moderations.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/conftest.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/lib/__pycache__/test_azure.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/lib/__pycache__/test_azure.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/lib/__pycache__/test_old_api.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/lib/__pycache__/test_old_api.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/lib/test_azure.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/lib/test_azure.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/test_client.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/test_deepcopy.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/test_deepcopy.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/test_extract_files.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/test_extract_files.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/test_files.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/test_legacy_response.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/test_legacy_response.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/test_models.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/test_module_client.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/test_module_client.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/test_qs.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/test_qs.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/test_required_args.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/test_required_args.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/test_response.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/test_streaming.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/test_streaming.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/test_transform.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/test_utils/__pycache__/test_proxy.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/test_utils/__pycache__/test_proxy.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/test_utils/__pycache__/test_typing.cpython-310-pytest-8.0.0.pyc` & `notdiamond-0.1.0a9/notdiamond/openai/tests/test_utils/__pycache__/test_typing.cpython-310-pytest-8.0.0.pyc`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/test_utils/test_proxy.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/test_utils/test_proxy.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/test_utils/test_typing.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/test_utils/test_typing.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/openai/tests/utils.py` & `notdiamond-0.1.0a9/notdiamond/openai/tests/utils.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/prompts/prompt.py` & `notdiamond-0.1.0a9/notdiamond/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/settings.py` & `notdiamond-0.1.0a9/notdiamond/settings.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/notdiamond/types.py` & `notdiamond-0.1.0a9/notdiamond/types.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0a8/pyproject.toml` & `notdiamond-0.1.0a9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "notdiamond"
-version = "0.1.0-alpha.8"
+version = "0.1.0-alpha.9"
 description = "NotDiamond Python Library"
 authors = ["Tze-Yang Tung"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "3.10.12"
+python = ">=3.10.12, <4.0"
 langchain = "0.1.3"
 anthropic = "0.12.0"
 pydantic = "2.5.3"
 datasketch = "1.6.4"
 langchain-google-genai = "^0.0.6"
 litellm = "^1.22.3"
 langchain-openai = "^0.0.5"
```

### Comparing `notdiamond-0.1.0a8/PKG-INFO` & `notdiamond-0.1.0a9/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: notdiamond
-Version: 0.1.0a8
+Version: 0.1.0a9
 Summary: NotDiamond Python Library
 Author: Tze-Yang Tung
-Requires-Python: ==3.10.12
+Requires-Python: >=3.10.12,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: anthropic (==0.12.0)
 Requires-Dist: datasketch (==1.6.4)
 Requires-Dist: langchain (==0.1.3)
 Requires-Dist: langchain-community (>=0.0.19,<0.0.20)
 Requires-Dist: langchain-google-genai (>=0.0.6,<0.0.7)
 Requires-Dist: langchain-openai (>=0.0.5,<0.0.6)
 Requires-Dist: litellm (>=1.22.3,<2.0.0)
```

