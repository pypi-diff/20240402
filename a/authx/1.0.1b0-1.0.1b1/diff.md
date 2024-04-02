# Comparing `tmp/authx-1.0.1b0.tar.gz` & `tmp/authx-1.0.1b1.tar.gz`

## Comparing `authx-1.0.1b0.tar` & `authx-1.0.1b1.tar`

### file list

```diff
@@ -1,80 +1,81 @@
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 authx-1.0.1b0/.all-contributorsrc
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 authx-1.0.1b0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 authx-1.0.1b0/mkdocs.yml
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 authx-1.0.1b0/.github/FUNDING.yml
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 authx-1.0.1b0/.github/SECURITY.md
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 authx-1.0.1b0/.github/dependabot.yml
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 authx-1.0.1b0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 authx-1.0.1b0/.github/workflows/release.yml
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 authx-1.0.1b0/authx/__init__.py
--rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 authx-1.0.1b0/authx/config.py
--rw-r--r--   0        0        0     5002 2020-02-02 00:00:00.000000 authx-1.0.1b0/authx/core.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 authx-1.0.1b0/authx/dependencies.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 authx-1.0.1b0/authx/exceptions.py
--rw-r--r--   0        0        0    22999 2020-02-02 00:00:00.000000 authx-1.0.1b0/authx/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-1.0.1b0/authx/py.typed
--rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 authx-1.0.1b0/authx/schema.py
--rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 authx-1.0.1b0/authx/token.py
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 authx-1.0.1b0/authx/types.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 authx-1.0.1b0/authx/_internal/__init__.py
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 authx-1.0.1b0/authx/_internal/_callback.py
--rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 authx-1.0.1b0/authx/_internal/_error.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 authx-1.0.1b0/authx/_internal/_logger.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 authx-1.0.1b0/authx/_internal/_memory.py
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 authx-1.0.1b0/authx/_internal/_signature.py
--rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 authx-1.0.1b0/authx/_internal/_utils.py
--rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 authx-1.0.1b0/docs/code_of_conduct.md
--rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 authx-1.0.1b0/docs/contributing.md
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 authx-1.0.1b0/docs/faq.md
--rw-r--r--   0        0        0    86820 2020-02-02 00:00:00.000000 authx-1.0.1b0/docs/favicon.png
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 authx-1.0.1b0/docs/header.svg
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 authx-1.0.1b0/docs/help.md
--rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 authx-1.0.1b0/docs/index.md
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 authx-1.0.1b0/docs/installation.md
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 authx-1.0.1b0/docs/license.md
--rw-r--r--   0        0        0    65324 2020-02-02 00:00:00.000000 authx-1.0.1b0/docs/release.md
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 authx-1.0.1b0/docs/css/custom.css
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 authx-1.0.1b0/docs/css/termynal.css
--rw-r--r--   0        0        0     6385 2020-02-02 00:00:00.000000 authx-1.0.1b0/docs/extra/Cache.md
--rw-r--r--   0        0        0     4447 2020-02-02 00:00:00.000000 authx-1.0.1b0/docs/extra/Metrics.md
--rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 authx-1.0.1b0/docs/extra/OAuth2.md
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 authx-1.0.1b0/docs/extra/Sessions.md
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 authx-1.0.1b0/docs/extra/profiler.md
--rw-r--r--   0        0        0   495130 2020-02-02 00:00:00.000000 authx-1.0.1b0/docs/img/install.gif
--rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 authx-1.0.1b0/docs/js/custom.js
--rw-r--r--   0        0        0     9540 2020-02-02 00:00:00.000000 authx-1.0.1b0/docs/js/termynal.js
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 authx-1.0.1b0/requirements/all.txt
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 authx-1.0.1b0/requirements/docs.in
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 authx-1.0.1b0/requirements/docs.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 authx-1.0.1b0/requirements/linting.in
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 authx-1.0.1b0/requirements/linting.txt
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 authx-1.0.1b0/requirements/pyproject.txt
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 authx-1.0.1b0/requirements/testing.in
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 authx-1.0.1b0/requirements/testing.txt
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 authx-1.0.1b0/scripts/clean.sh
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 authx-1.0.1b0/scripts/docs_build.sh
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 authx-1.0.1b0/scripts/docs_serve.sh
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 authx-1.0.1b0/scripts/format.sh
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 authx-1.0.1b0/scripts/install.sh
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 authx-1.0.1b0/scripts/mypy.sh
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 authx-1.0.1b0/scripts/requirements.sh
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 authx-1.0.1b0/scripts/test.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-1.0.1b0/tests/__init__.py
--rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 authx-1.0.1b0/tests/test_authx.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 authx-1.0.1b0/tests/test_callback.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 authx-1.0.1b0/tests/test_config.py
--rw-r--r--   0        0        0    13102 2020-02-02 00:00:00.000000 authx-1.0.1b0/tests/test_core.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 authx-1.0.1b0/tests/test_dependencies.py
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 authx-1.0.1b0/tests/test_errors.py
--rw-r--r--   0        0        0     8840 2020-02-02 00:00:00.000000 authx-1.0.1b0/tests/test_schema.py
--rw-r--r--   0        0        0     9539 2020-02-02 00:00:00.000000 authx-1.0.1b0/tests/test_token.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-1.0.1b0/tests/internal/__init__.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 authx-1.0.1b0/tests/internal/test_logger.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 authx-1.0.1b0/tests/internal/test_memory.py
--rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 authx-1.0.1b0/tests/internal/test_signature.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 authx-1.0.1b0/tests/internal/test_utils.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 authx-1.0.1b0/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 authx-1.0.1b0/LICENSE
--rw-r--r--   0        0        0     9758 2020-02-02 00:00:00.000000 authx-1.0.1b0/README.md
--rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 authx-1.0.1b0/pyproject.toml
--rw-r--r--   0        0        0    11496 2020-02-02 00:00:00.000000 authx-1.0.1b0/PKG-INFO
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 authx-1.0.1b1/.all-contributorsrc
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 authx-1.0.1b1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 authx-1.0.1b1/mkdocs.yml
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 authx-1.0.1b1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 authx-1.0.1b1/.github/SECURITY.md
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 authx-1.0.1b1/.github/dependabot.yml
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 authx-1.0.1b1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 authx-1.0.1b1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/__init__.py
+-rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/config.py
+-rw-r--r--   0        0        0     5002 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/core.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/dependencies.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/exceptions.py
+-rw-r--r--   0        0        0    22999 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/py.typed
+-rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/schema.py
+-rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/token.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/types.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/_internal/__init__.py
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/_internal/_callback.py
+-rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/_internal/_error.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/_internal/_logger.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/_internal/_memory.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/_internal/_signature.py
+-rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/_internal/_utils.py
+-rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/code_of_conduct.md
+-rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/contributing.md
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/faq.md
+-rw-r--r--   0        0        0    86820 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/favicon.png
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/header.svg
+-rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/help.md
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/index.md
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/installation.md
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/license.md
+-rw-r--r--   0        0        0    65324 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/release.md
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/css/custom.css
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/css/termynal.css
+-rw-r--r--   0        0        0     6385 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/extra/Cache.md
+-rw-r--r--   0        0        0     4447 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/extra/Metrics.md
+-rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/extra/OAuth2.md
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/extra/Sessions.md
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/extra/profiler.md
+-rw-r--r--   0        0        0     6229 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/get-started/basic-usage.md
+-rw-r--r--   0        0        0   495130 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/img/install.gif
+-rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/js/custom.js
+-rw-r--r--   0        0        0     9540 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/js/termynal.js
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 authx-1.0.1b1/requirements/all.txt
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 authx-1.0.1b1/requirements/docs.in
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 authx-1.0.1b1/requirements/docs.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 authx-1.0.1b1/requirements/linting.in
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 authx-1.0.1b1/requirements/linting.txt
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 authx-1.0.1b1/requirements/pyproject.txt
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 authx-1.0.1b1/requirements/testing.in
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 authx-1.0.1b1/requirements/testing.txt
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 authx-1.0.1b1/scripts/clean.sh
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 authx-1.0.1b1/scripts/docs_build.sh
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 authx-1.0.1b1/scripts/docs_serve.sh
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 authx-1.0.1b1/scripts/format.sh
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 authx-1.0.1b1/scripts/install.sh
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 authx-1.0.1b1/scripts/mypy.sh
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 authx-1.0.1b1/scripts/requirements.sh
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 authx-1.0.1b1/scripts/test.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-1.0.1b1/tests/__init__.py
+-rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 authx-1.0.1b1/tests/test_authx.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 authx-1.0.1b1/tests/test_callback.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 authx-1.0.1b1/tests/test_config.py
+-rw-r--r--   0        0        0    13102 2020-02-02 00:00:00.000000 authx-1.0.1b1/tests/test_core.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 authx-1.0.1b1/tests/test_dependencies.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 authx-1.0.1b1/tests/test_errors.py
+-rw-r--r--   0        0        0     8840 2020-02-02 00:00:00.000000 authx-1.0.1b1/tests/test_schema.py
+-rw-r--r--   0        0        0     9539 2020-02-02 00:00:00.000000 authx-1.0.1b1/tests/test_token.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-1.0.1b1/tests/internal/__init__.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 authx-1.0.1b1/tests/internal/test_logger.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 authx-1.0.1b1/tests/internal/test_memory.py
+-rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 authx-1.0.1b1/tests/internal/test_signature.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 authx-1.0.1b1/tests/internal/test_utils.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 authx-1.0.1b1/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 authx-1.0.1b1/LICENSE
+-rw-r--r--   0        0        0     9980 2020-02-02 00:00:00.000000 authx-1.0.1b1/README.md
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 authx-1.0.1b1/pyproject.toml
+-rw-r--r--   0        0        0    11744 2020-02-02 00:00:00.000000 authx-1.0.1b1/PKG-INFO
```

### Comparing `authx-1.0.1b0/.all-contributorsrc` & `authx-1.0.1b1/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/mkdocs.yml` & `authx-1.0.1b1/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,16 @@
     alternate_style: true
   attr_list:
   md_in_html:
 
 nav:
   - About: index.md
   - installation.md
+  - Get Started:
+    - get-started/basic-usage.md
   - Extra:
     - extra/OAuth2.md
     - extra/Metrics.md
     - extra/Cache.md
     - extra/profiler.md
     - extra/Sessions.md
   - Help AuthX - Get Help: help.md
```

### Comparing `authx-1.0.1b0/.github/workflows/ci.yml` & `authx-1.0.1b1/.github/workflows/ci.yml`

 * *Files 18% similar despite different names*

```diff
@@ -16,19 +16,26 @@
 
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
-      - name: Install Dependencies
-        run: pip install -r requirements/pyproject.txt && pip install -r requirements/linting.txt
-      - uses: pre-commit/action@v3.0.0
+
+      - name: setup uv
+        uses: yezz123/setup-uv@v2
         with:
-          extra_args: --all-files --verbose
+          uv-version: "0.2.2"
+          uv-venv: ".venv"
+
+      - name: Install Dependencies
+        run: uv pip install -r requirements/pyproject.txt && uv pip install -r requirements/linting.txt
+
+      - name: Run Pre-commit
+        run: bash scripts/format.sh
 
   tests:
 
     name: test py${{ matrix.python-version }} on ${{ matrix.os }}
 
     runs-on: ${{ matrix.os }}-latest
 
@@ -45,25 +52,36 @@
       - uses: actions/checkout@v4
 
       - name: Set up Python
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
+      - name: setup UV
+        uses: yezz123/setup-uv@v2
+        with:
+          uv-version: "0.2.2"
+          uv-venv: ".venv"
+
       - name: Install Dependencies
-        run: pip install -r requirements/pyproject.txt && pip install -r requirements/testing.txt
+        run: uv pip install -r requirements/pyproject.txt && uv pip install -r requirements/testing.txt
 
       - name: Freeze Dependencies
-        run: pip freeze
+        run: uv pip freeze
 
-      - name: Test with pytest
+      - name: Test with pytest - ${{ matrix.os }} - py${{ matrix.python-version }}
         run: bash scripts/test.sh
+        env:
+          CONTEXT: ${{ runner.os }}-py${{ matrix.python-version }}-with-deps
 
-      - name: Upload coverage
+      - name: Upload coverage to Codecov
         uses: codecov/codecov-action@v4
+        with:
+          token: ${{ secrets.CODECOV_TOKEN }}
+          file: ./coverage.xml
 
   # https://github.com/marketplace/actions/alls-green#why used for branch protection checks
   check:
     if: always()
     needs: [lint, tests]
     runs-on: ubuntu-latest
     steps:
```

### Comparing `authx-1.0.1b0/.github/workflows/release.yml` & `authx-1.0.1b1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/authx/config.py` & `authx-1.0.1b1/authx/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from datetime import timedelta
 from typing import List, Optional, Sequence
 
 from jwt.algorithms import get_default_algorithms, requires_cryptography
-from pydantic import BaseSettings, Field
+from pydantic import Field
+from pydantic_settings import BaseSettings
 
 from authx.exceptions import BadConfigurationError
 from authx.types import (
     AlgorithmType,
     HTTPMethods,
     SameSitePolicy,
     StringOrSequence,
```

### Comparing `authx-1.0.1b0/authx/core.py` & `authx-1.0.1b1/authx/core.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/authx/dependencies.py` & `authx-1.0.1b1/authx/dependencies.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/authx/exceptions.py` & `authx-1.0.1b1/authx/exceptions.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/authx/main.py` & `authx-1.0.1b1/authx/main.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/authx/schema.py` & `authx-1.0.1b1/authx/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
 from hmac import compare_digest
 from typing import Any, Dict, List, Optional, Sequence
 
-from pydantic import BaseModel, Extra, Field, ValidationError, validator
+from pydantic import BaseModel, ConfigDict, Field, ValidationError, validator
 
 from authx._internal._utils import get_now, get_now_ts, get_uuid
 from authx.exceptions import (
     AccessTokenRequiredError,
     CSRFError,
     FreshTokenRequiredError,
     JWTDecodeError,
@@ -22,38 +22,36 @@
     TokenLocation,
     TokenType,
     Union,
 )
 
 
 class TokenPayload(BaseModel):
+    model_config = ConfigDict(extra="allow")
     jti: Optional[str] = Field(default_factory=get_uuid)
     iss: Optional[str] = None
     sub: Optional[str] = None
     aud: Optional[str] = None
     exp: Optional[Union[Numeric, DateTimeExpression]] = None
     nbf: Optional[Union[Numeric, DateTimeExpression]] = None
     iat: Optional[Union[Numeric, DateTimeExpression]] = Field(
         default_factory=lambda: int(get_now_ts())
     )
     type: Optional[str] = None
     csrf: Optional[str] = None
     scopes: Optional[List[str]] = None
     fresh: bool = False
 
-    class Config:
-        extra = Extra.allow
-
     @property
     def _additional_fields(self):
-        return set(self.__dict__) - set(self.__fields__)
+        return set(self.__dict__) - set(self.model_fields)
 
     @property
     def extra_dict(self):
-        return self.dict(include=self._additional_fields)
+        return self.model_dump(include=self._additional_fields)
 
     @property
     def issued_at(self) -> datetime.datetime:
         if isinstance(self.iat, (float, int)):
             return datetime.datetime.fromtimestamp(self.iat, tz=datetime.timezone.utc)
         elif isinstance(self.iat, datetime.datetime):
             return self.iat
@@ -132,15 +130,15 @@
             token=token,
             key=key,
             algorithms=algorithms,
             audience=audience,
             issuer=issuer,
             verify=verify,
         )
-        return cls.parse_obj(payload)
+        return cls.model_validate(payload)
 
 
 class RequestToken(BaseModel):
     token: Optional[str] = None
     csrf: Optional[str] = None
     type: TokenType = "access"
     location: TokenLocation
```

### Comparing `authx-1.0.1b0/authx/token.py` & `authx-1.0.1b1/authx/token.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/authx/types.py` & `authx-1.0.1b1/authx/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime
 from typing import Callable, Literal, Optional, Sequence, TypeVar, Union
 
 try:
     from typing import ParamSpecKwargs
-except Exception:
-    from typing_extensions import ParamSpecKwargs
+except Exception:  # pragma: no cover
+    from typing_extensions import ParamSpecKwargs  # pragma: no cover
 
 T = TypeVar("T")
 Numeric = Union[float, int]
 ObjectOrSequence = Union[T, Sequence[T]]
 StringOrSequence = ObjectOrSequence[str]
```

### Comparing `authx-1.0.1b0/authx/_internal/__init__.py` & `authx-1.0.1b1/authx/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/authx/_internal/_callback.py` & `authx-1.0.1b1/authx/_internal/_callback.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/authx/_internal/_error.py` & `authx-1.0.1b1/authx/_internal/_error.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/authx/_internal/_logger.py` & `authx-1.0.1b1/authx/_internal/_logger.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/authx/_internal/_memory.py` & `authx-1.0.1b1/authx/_internal/_memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         else:
             return None
 
     def save_store(self, session_id):
         self.get_store(session_id)
 
     def gc(self):
-        if len(self.raw_memory_store) >= 100:
+        if len(self.raw_memory_store) >= 100:  # pragma: no cover
             self.cleanup_old_sessions()
 
     def cleanup_old_sessions(self):
         current_time = int(time.time())
         sessions_to_delete = [
             session_id
             for session_id, session_info in self.raw_memory_store.items()
```

### Comparing `authx-1.0.1b0/authx/_internal/_signature.py` & `authx-1.0.1b1/authx/_internal/_signature.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,16 @@
                 decoded_obj = self.ser.loads(token)
             else:
                 decoded_obj = self.ser.loads(token, max_age=self.expired_in)
         except SignatureExpired:
             return None, "SignatureExpired"
         except BadTimeSignature:
             return None, "InvalidSignature"
-
+        except Exception:
+            return None, "BadSignature"  # Catch-all for other signature errors
         return decoded_obj, None
 
 
 if CASUAL_UT:
     serializer = SignatureSerializer("MY_SECRET_KEY", expired_in=1)
     session_id = 1
     dict_obj = {"session_id": session_id}
```

### Comparing `authx-1.0.1b0/authx/_internal/_utils.py` & `authx-1.0.1b1/authx/_internal/_utils.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/docs/code_of_conduct.md` & `authx-1.0.1b1/docs/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/docs/contributing.md` & `authx-1.0.1b1/docs/contributing.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,62 +4,64 @@
 [help AuthX and get help](help.md)
 
 ## Developing
 
 If you already cloned the repository and you know that you need to deep dive
 into the code, here is a guideline to set up your environment:
 
-### Virtual environment with `venv`
+### Virtual environment with `uv`
 
-You can create a virtual environment in a directory using Python's `venv`
+You can create a virtual environment in a directory using Python's [`uv`](https://github.com/astral-sh/uv)
 module:
 
 <div class="termy">
 
 ```console
-python -m venv env
+pip install uv
+
+uv venv
 ```
 
 </div>
 
-That will create a directory `./env/` with the python binaries and then you will
+That will create a directory `.venv` with the python binaries and then you will
 be able to install packages for that isolated environment.
 
 ### Activate the environment
 
 Activate the new environment with:
 
 === "Linux, macOS"
 
     <div class="termy">
 
     ```console
-    $ source ./env/bin/activate
+    $ source ./.venv/bin/activate
     ```
 
     </div>
 
 === "Windows PowerShell"
 
     <div class="termy">
 
     ```console
-    $ .\env\Scripts\Activate.ps1
+    $ .\.venv\Scripts\Activate.ps1
     ```
 
     </div>
 
 === "Windows Bash"
 
     Or if you use Bash for Windows (e.g. <a href="https://gitforwindows.org/" class="external-link" target="_blank">Git Bash</a>):
 
     <div class="termy">
 
     ```console
-    $ source ./env/Scripts/activate
+    $ source ./.venv/Scripts/activate
     ```
 
     </div>
 
 To check it worked, use:
 
 === "Linux, macOS, Windows Bash"
@@ -78,15 +80,15 @@
 
     ```console
     $ Get-Command pip
     ```
 
     </div>
 
-If it shows the `pip` binary at `env/bin/pip` then it worked. 🎉
+If it shows the `pip` binary at `venv/bin/pip` then it worked. 🎉
 
 !!! tip
 
     Every time you install a new package with `pip` under that environment,
     activate the environment again.
 
     This makes sure that if you use a terminal program installed by that package (like `pre-commit`), you use the one from your local environment and not any other that could be installed globally.
@@ -94,15 +96,15 @@
 ### pip
 
 After activating the environment as described above, Now lets install all the package that you need to develop authx:
 
 <div class="termy">
 
 ```console
-$ pip install -r requirements/all.txt
+$ uv pip install -r requirements/all.txt
 
 ---> 100%
 ```
 
 </div>
 
 It will install all the dependencies in your local environment.
```

#### html2text {}

```diff
@@ -1,33 +1,34 @@
 # Development - Contributing ð£ First, you might want to see the basic ways
 to [help AuthX and get help](help.md) ## Developing If you already cloned the
 repository and you know that you need to deep dive into the code, here is a
-guideline to set up your environment: ### Virtual environment with `venv` You
-can create a virtual environment in a directory using Python's `venv` module:
-```console python -m venv env ```
-That will create a directory `./env/` with the python binaries and then you
-will be able to install packages for that isolated environment. ### Activate
-the environment Activate the new environment with: === "Linux, macOS"
-```console $ source ./env/bin/activate ```
+guideline to set up your environment: ### Virtual environment with `uv` You can
+create a virtual environment in a directory using Python's [`uv`](https://
+github.com/astral-sh/uv) module:
+```console pip install uv uv venv ```
+That will create a directory `.venv` with the python binaries and then you will
+be able to install packages for that isolated environment. ### Activate the
+environment Activate the new environment with: === "Linux, macOS"
+```console $ source ./.venv/bin/activate ```
 === "Windows PowerShell"
-```console $ .\env\Scripts\Activate.ps1 ```
+```console $ .\.venv\Scripts\Activate.ps1 ```
 === "Windows Bash" Or if you use Bash for Windows (e.g. _G_i_t_ _B_a_s_h):
-```console $ source ./env/Scripts/activate ```
+```console $ source ./.venv/Scripts/activate ```
 To check it worked, use: === "Linux, macOS, Windows Bash"
 ```console $ which pip ```
 === "Windows PowerShell"
 ```console $ Get-Command pip ```
-If it shows the `pip` binary at `env/bin/pip` then it worked. ð !!! tip
+If it shows the `pip` binary at `venv/bin/pip` then it worked. ð !!! tip
 Every time you install a new package with `pip` under that environment,
 activate the environment again. This makes sure that if you use a terminal
 program installed by that package (like `pre-commit`), you use the one from
 your local environment and not any other that could be installed globally. ###
 pip After activating the environment as described above, Now lets install all
 the package that you need to develop authx:
-```console $ pip install -r requirements/all.txt ---> 100% ```
+```console $ uv pip install -r requirements/all.txt ---> 100% ```
 It will install all the dependencies in your local environment. #### Including
 The Dependencies file contains all the dependencies that you need to develop
 AuthX, which are: - The Base Dependencies - the ones that are needed to run
 AuthX. [See Installation](installation.md). ### Format For Providing a good and
 consistent experience, we recommend using [pre-commit](https://pre-commit.com/
 ) - a tool that runs a set of checks before you commit your code. #### Git
 Hooks First you need to install the [pre-commit](https://pre-commit.com/) tool,
```

### Comparing `authx-1.0.1b0/docs/faq.md` & `authx-1.0.1b1/docs/faq.md`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/docs/favicon.png` & `authx-1.0.1b1/docs/favicon.png`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/docs/header.svg` & `authx-1.0.1b1/docs/header.svg`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/docs/help.md` & `authx-1.0.1b1/docs/help.md`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/docs/index.md` & `authx-1.0.1b1/docs/index.md`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 </a>
 <a href="https://codecov.io/gh/yezz123/authx">
     <img src="https://codecov.io/gh/yezz123/authx/branch/main/graph/badge.svg"/>
 </a>
 <a href="https://pepy.tech/project/authx" target="_blank">
     <img src="https://static.pepy.tech/badge/authx" alt="Total Downloads">
 </a>
+<a href="https://pydantic.dev" target="_blank">
+    <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/main/docs/badge/v2.json" alt="Pydantic Version 2">
+</a>
 </p>
 </p>
 
 ---
 
 **Source Code**: <https://github.com/yezz123/authx>
 
@@ -51,15 +54,15 @@
 ---> 100%
 ```
 
 </div>
 
 ## Features 🔧
 
-- Support Python 3.8+.
+- Support Python 3.8+ & Pydantic 2.0+.
 - Multiple customizable authentication backend:
   - JWT authentication backend included
     - JWT encoding/decoding for application authentication
     - Automatic detection of JWTs in requests:
       - JWTs in headers
       - JWTs in cookies
       - JWTs in query parameters
```

### Comparing `authx-1.0.1b0/docs/installation.md` & `authx-1.0.1b1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/docs/license.md` & `authx-1.0.1b1/docs/license.md`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/docs/release.md` & `authx-1.0.1b1/docs/release.md`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/docs/css/termynal.css` & `authx-1.0.1b1/docs/css/termynal.css`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/docs/extra/Cache.md` & `authx-1.0.1b1/docs/extra/Cache.md`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/docs/extra/Metrics.md` & `authx-1.0.1b1/docs/extra/Metrics.md`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/docs/extra/OAuth2.md` & `authx-1.0.1b1/docs/extra/OAuth2.md`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/docs/extra/Sessions.md` & `authx-1.0.1b1/docs/extra/Sessions.md`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/docs/extra/profiler.md` & `authx-1.0.1b1/docs/extra/profiler.md`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/docs/img/install.gif` & `authx-1.0.1b1/docs/img/install.gif`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/docs/js/custom.js` & `authx-1.0.1b1/docs/js/custom.js`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/docs/js/termynal.js` & `authx-1.0.1b1/docs/js/termynal.js`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/requirements/docs.txt` & `authx-1.0.1b1/requirements/docs.txt`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --output-file=requirements/docs.txt requirements/docs.in
 #
 babel==2.14.0
     # via mkdocs-material
-beautifulsoup4==4.12.2
+beautifulsoup4==4.12.3
     # via mkdocs-mermaid2-plugin
 cairocffi==1.6.1
     # via cairosvg
 cairosvg==2.7.1
     # via -r requirements/docs.in
-certifi==2023.11.17
+certifi==2024.2.2
     # via requests
 cffi==1.16.0
     # via cairocffi
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
@@ -53,15 +53,15 @@
     #   markdown-include
     #   mdx-include
     #   mkdocs
     #   mkdocs-material
     #   pymdown-extensions
 markdown-include==0.8.1
     # via -r requirements/docs.in
-markupsafe==2.1.3
+markupsafe==2.1.5
     # via
     #   jinja2
     #   mkdocs
 mdx-include==1.4.2
     # via -r requirements/docs.in
 mergedeep==1.3.4
     # via mkdocs
@@ -69,15 +69,15 @@
     # via
     #   -r requirements/docs.in
     #   mkdocs-markdownextradata-plugin
     #   mkdocs-material
     #   mkdocs-mermaid2-plugin
 mkdocs-markdownextradata-plugin==0.2.5
     # via -r requirements/docs.in
-mkdocs-material==9.5.7
+mkdocs-material==9.5.9
     # via -r requirements/docs.in
 mkdocs-material-extensions==1.3.1
     # via mkdocs-material
 mkdocs-mermaid2-plugin==1.1.1
     # via -r requirements/docs.in
 packaging==23.2
     # via mkdocs
@@ -85,15 +85,15 @@
     # via mkdocs-material
 pathspec==0.12.1
     # via mkdocs
 pillow==10.2.0
     # via
     #   -r requirements/docs.in
     #   cairosvg
-platformdirs==4.1.0
+platformdirs==4.2.0
     # via mkdocs
 pycparser==2.21
     # via cffi
 pygments==2.17.2
     # via
     #   mkdocs-material
     #   rich
@@ -139,17 +139,17 @@
     #   cssselect2
 typer[all]==0.7.0
     # via
     #   -r requirements/docs.in
     #   typer-cli
 typer-cli==0.0.13
     # via -r requirements/docs.in
-urllib3==2.1.0
+urllib3==2.2.0
     # via requests
-watchdog==3.0.0
+watchdog==4.0.0
     # via mkdocs
 webencodings==0.5.1
     # via
     #   cssselect2
     #   tinycss2
 
 # The following packages are considered to be unsafe in a requirements file:
```

### Comparing `authx-1.0.1b0/requirements/linting.txt` & `authx-1.0.1b1/requirements/linting.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --output-file=requirements/linting.txt requirements/linting.in
 #
-black==24.1.1
+black==24.2.0
     # via -r requirements/linting.in
 cfgv==3.4.0
     # via pre-commit
 click==8.1.7
     # via black
 distlib==0.3.8
     # via virtualenv
@@ -24,25 +24,25 @@
     #   mypy
 nodeenv==1.8.0
     # via pre-commit
 packaging==23.2
     # via black
 pathspec==0.12.1
     # via black
-platformdirs==4.1.0
+platformdirs==4.2.0
     # via
     #   black
     #   virtualenv
-pre-commit==3.6.0
+pre-commit==3.6.2
     # via -r requirements/linting.in
-pyupgrade==3.15.0
+pyupgrade==3.15.1
     # via -r requirements/linting.in
 pyyaml==6.0.1
     # via pre-commit
-ruff==0.2.0
+ruff==0.2.2
     # via -r requirements/linting.in
 tokenize-rt==5.2.0
     # via pyupgrade
 typing-extensions==4.9.0
     # via mypy
 virtualenv==20.25.0
     # via pre-commit
```

### Comparing `authx-1.0.1b0/requirements/testing.txt` & `authx-1.0.1b1/requirements/testing.txt`

 * *Files 18% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --output-file=requirements/testing.txt requirements/testing.in
 #
 anyio==4.2.0
     # via httpx
-certifi==2023.11.17
+certifi==2024.2.2
     # via
     #   httpcore
     #   httpx
     #   requests
 charset-normalizer==3.3.2
     # via requests
-coverage[toml]==7.4.0
+coverage[toml]==7.4.1
     # via
     #   coverage
     #   pytest-cov
 freezegun==1.4.0
     # via -r requirements/testing.in
 greenlet==3.0.3
     # via sqlalchemy
@@ -34,36 +34,36 @@
     #   requests
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via -r requirements/testing.in
 packaging==23.2
     # via pytest
-pluggy==1.3.0
+pluggy==1.4.0
     # via pytest
-pytest==7.4.4
+pytest==8.0.1
     # via
     #   -r requirements/testing.in
     #   pytest-asyncio
     #   pytest-cov
-pytest-asyncio==0.23.4
+pytest-asyncio==0.23.5
     # via -r requirements/testing.in
 pytest-cov==4.1.0
     # via -r requirements/testing.in
 python-dateutil==2.8.2
     # via freezegun
 requests==2.31.0
     # via -r requirements/testing.in
 six==1.16.0
     # via python-dateutil
 sniffio==1.3.0
     # via
     #   anyio
     #   httpx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.27
     # via -r requirements/testing.in
 typing-extensions==4.9.0
     # via sqlalchemy
-urllib3==2.1.0
+urllib3==2.2.0
     # via requests
 websockets==12.0
     # via -r requirements/testing.in
```

### Comparing `authx-1.0.1b0/scripts/clean.sh` & `authx-1.0.1b1/scripts/clean.sh`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env bash
 
 rm -f `find . -type f -name '*.py[co]' `
 rm -f `find . -type f -name '*~' `
 rm -f `find . -type f -name '.*~' `
 rm -f `find . -type f -name .coverage`
+rm -f `find . -type f -name coverage.xml`
 rm -f `find . -type f -name ".coverage.*"`
 rm -rf `find . -name __pycache__`
 rm -rf `find . -name authx_profiling_results.html`
 rm -rf `find . -name authx_profiling_results.json`
 rm -rf `find . -name users.db`
 rm -rf `find . -type d -name '*.egg-info' `
 rm -rf `find . -type d -name 'pip-wheel-metadata' `
```

### Comparing `authx-1.0.1b0/scripts/requirements.sh` & `authx-1.0.1b1/scripts/requirements.sh`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/tests/test_authx.py` & `authx-1.0.1b1/tests/test_authx.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/tests/test_callback.py` & `authx-1.0.1b1/tests/test_callback.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/tests/test_config.py` & `authx-1.0.1b1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/tests/test_core.py` & `authx-1.0.1b1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/tests/test_dependencies.py` & `authx-1.0.1b1/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/tests/test_errors.py` & `authx-1.0.1b1/tests/test_errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,7 +63,13 @@
     assert exc.TokenTypeError in app.exception_handlers
     assert exc.RevokedTokenError in app.exception_handlers
     assert exc.TokenRequiredError in app.exception_handlers
     assert exc.FreshTokenRequiredError in app.exception_handlers
     assert exc.AccessTokenRequiredError in app.exception_handlers
     assert exc.RefreshTokenRequiredError in app.exception_handlers
     assert exc.CSRFError in app.exception_handlers
+
+
+def test_invalid_token_init():
+    errors = ["Invalid signature", "Expired token"]
+    exception = exc.InvalidToken(errors)
+    assert exception.errors == errors
```

### Comparing `authx-1.0.1b0/tests/test_schema.py` & `authx-1.0.1b1/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/tests/test_token.py` & `authx-1.0.1b1/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/tests/internal/test_memory.py` & `authx-1.0.1b1/tests/internal/test_memory.py`

 * *Files 20% similar despite different names*

```diff
@@ -66,7 +66,32 @@
 
 
 def test_get_store():
     store = MemoryIO()
     store.create_store("test-id")
     assert store.get_store("test-id") == {}
     assert store.get_store("nonexistent-id") is None
+
+
+def test_gc_cleanup_old_sessions(memory_io):
+    # Populate raw_memory_store with 100 sessions older than 12 hours
+    current_time = int(time())
+    twelve_hours_ago = current_time - 3600 * 12
+    for i in range(100):
+        memory_io.raw_memory_store[str(i)] = {
+            "created_at": twelve_hours_ago,
+            "store": {},
+        }
+
+    # Add one more session within 12 hours
+    extra_session_id = "1000"
+    memory_io.raw_memory_store[extra_session_id] = {
+        "created_at": current_time,
+        "store": {},
+    }
+
+    # Ensure gc triggers cleanup
+    memory_io.gc()
+
+    # Ensure old sessions are cleaned up
+    assert len(memory_io.raw_memory_store) == 101
+    assert extra_session_id in memory_io.raw_memory_store
```

### Comparing `authx-1.0.1b0/tests/internal/test_signature.py` & `authx-1.0.1b1/tests/internal/test_signature.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,31 +12,40 @@
         token = serializer.encode(dict_obj)
         data, err = serializer.decode(token)
         self.assertIsNotNone(data)
         self.assertIsNone(err)
         self.assertEqual(data["session_id"], session_id)
 
     def test_decode_with_no_token(self):
-        serializer = SignatureSerializer("MY_SECRET_KEY", expired_in=1)
-        token = None
-        data, err = serializer.decode(token)
-        self.assertIsNone(data)
-        self.assertEqual(err, "NoTokenSpecified")
+        self.decode_serializer(None, "NoTokenSpecified")
 
     def test_decode_with_expired_token(self):
         serializer = SignatureSerializer("MY_SECRET_KEY", expired_in=1)
         session_id = 1
         dict_obj = {"session_id": session_id}
         token = serializer.encode(dict_obj)
         # Sleep for more than 1 second to simulate an expired token
         time.sleep(2)
         data, err = serializer.decode(token)
         self.assertIsNone(data)
         self.assertEqual(err, "SignatureExpired")
 
+    def test_decode_with_invalid_signature(self):
+        self.decode_serializer("tampered_token", "BadSignature")
+
+    def test_decode_with_malformed_token(self):
+        self.decode_serializer("malformedtoken", "BadSignature")
+
+    def decode_serializer(self, token, expected_data):
+        serializer = SignatureSerializer("MY_SECRET_KEY", expired_in=1)
+        token = token
+        data, err = serializer.decode(token)
+        self.assertIsNone(data)
+        self.assertEqual(err, expected_data)
+
 
 def test_token_expiration():
     serializer = SignatureSerializer("MY_SECRET_KEY", expired_in=1)
     dict_obj = {"session_id": 999}
     token = serializer.encode(dict_obj)
 
     time.sleep(2)
@@ -54,18 +63,39 @@
     time.sleep(2)
     data, err = serializer.decode(token)
     assert (
         data is not None and err is None and data["session_id"] == 999
     ), "Failed to decode or session_id does not match."
 
 
-@unittest.skip("Dropping tampering test for now.")
+@unittest.skip("Tampered token did not cause an error as expected.")
 def test_token_tampering():
     serializer = SignatureSerializer("MY_SECRET_KEY", expired_in=3600)
     dict_obj = {"session_id": 999}
     token = serializer.encode(dict_obj)
 
     tampered_token = f"{token[:-1]}a"
     data, err = serializer.decode(tampered_token)
     assert (
         data is None and err == "InvalidSignature"
     ), "Tampered token did not cause an error as expected."
+
+
+def test_casual_ut():
+    secret_key = "MY_SECRET_KEY"
+    expired_in = 1
+    session_id = 1
+    dict_obj = {"session_id": session_id}
+
+    # Instantiate SignatureSerializer
+    serializer = SignatureSerializer(secret_key, expired_in=expired_in)
+
+    # Encode the dictionary object into a token
+    token = serializer.encode(dict_obj)
+
+    # Decode the token
+    data, err = serializer.decode(token)
+
+    # Assert the results
+    assert (
+        data is not None and err is None and data["session_id"] == session_id
+    ), "Failed to decode or session_id does not match."
```

### Comparing `authx-1.0.1b0/tests/internal/test_utils.py` & `authx-1.0.1b1/tests/internal/test_utils.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/.gitignore` & `authx-1.0.1b1/.gitignore`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/LICENSE` & `authx-1.0.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b0/README.md` & `authx-1.0.1b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 </a>
 <a href="https://codecov.io/gh/yezz123/authx">
     <img src="https://codecov.io/gh/yezz123/authx/branch/main/graph/badge.svg"/>
 </a>
 <a href="https://pepy.tech/project/authx" target="_blank">
     <img src="https://static.pepy.tech/badge/authx" alt="Test">
 </a>
+<a href="https://pydantic.dev" target="_blank">
+    <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/main/docs/badge/v2.json" alt="Pydantic Version 2">
+</a>
 </p>
 </p>
 
 ---
 
 **Source Code**: <https://github.com/yezz123/authx>
 
@@ -39,15 +42,15 @@
 >
 > [Authx V0.9.x](https://authx-v0.yezz.me/) This branch relates to development of authx V1 which is not yet ready for production use.
 >
 >If you're a Authx user, you probably want either Authx V0.9 [Documentation](https://authx-v0.yezz.me/) or, [0.X.X-fix](https://github.com/yezz123/authx/tree/0.X.X-fix) git branch.
 
 ## Features 🔧
 
-- [x] Support Python 3.8+.
+- [x] Support Python 3.8+ & Pydantic 2.0+.
 - [x] Multiple customizable authentication backend:
   - [x] JWT authentication backend included
     - [x] JWT encoding/decoding for application authentication
     - [x] Automatic detection of JWTs in requests:
       - [x] JWTs in headers
       - [x] JWTs in cookies
       - [x] JWTs in query parameters
```

### Comparing `authx-1.0.1b0/pyproject.toml` & `authx-1.0.1b1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,16 @@
     "Topic :: Internet",
     "Typing :: Typed",
 ]
 
 dependencies = [
     "fastapi >=0.65.2,<0.110.0",
     "pyjwt[crypto] >=2.6.0,<3.0.0",
-    "pydantic >=1.7.4,!=1.8,!=1.8.1,<2.0.0",
+    "pydantic >=2.0.0,<2.6.1",
+    "pydantic-settings >=2.1.0",
     "python-dateutil>=2.8,<3.0.0",
     "pytz>=2023.3,<2025.0",
     "python-jose>=3.3.0,<4.0.0",
 ]
 
 dynamic = ["version"]
 
@@ -94,22 +95,23 @@
 [tool.ruff.lint.isort]
 known-third-party = ["pydantic", "typing_extensions", "sqlalchemy"]
 
 [tool.ruff.lint.pyupgrade]
 keep-runtime-typing = true
 
 [tool.coverage.run]
-source = ["authx", "tests"]
+source = ["authx"]
 branch = true
 context = '${CONTEXT}'
 
 [tool.coverage.paths]
 source = [
-    "authx/",
-    "tests/",
+    'authx/',
+    '/Users/runner/work/authx/authx/authx/',
+    'D:\a\authx\authx\authx',
 ]
 
 [tool.coverage.report]
 precision = 2
 exclude_lines = [
     'pragma: no cover',
     'raise NotImplementedError',
```

### Comparing `authx-1.0.1b0/PKG-INFO` & `authx-1.0.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authx
-Version: 1.0.1b0
+Version: 1.0.1b1
 Summary: Ready to use and customizable Authentications and Oauth2 management for FastAPI
 Project-URL: Homepage, https://github.com/yezz123/authx
 Project-URL: Documentation, https://authx.yezz.me/
 Project-URL: Funding, https://github.com/sponsors/yezz123
 Author-email: Yasser Tahiri <hello@yezz.me>
 License-Expression: MIT
 License-File: LICENSE
@@ -28,15 +28,16 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: fastapi<0.110.0,>=0.65.2
-Requires-Dist: pydantic!=1.8,!=1.8.1,<2.0.0,>=1.7.4
+Requires-Dist: pydantic-settings>=2.1.0
+Requires-Dist: pydantic<2.6.1,>=2.0.0
 Requires-Dist: pyjwt[crypto]<3.0.0,>=2.6.0
 Requires-Dist: python-dateutil<3.0.0,>=2.8
 Requires-Dist: python-jose<4.0.0,>=3.3.0
 Requires-Dist: pytz<2025.0,>=2023.3
 Description-Content-Type: text/markdown
 
 # AuthenticationX 💫
@@ -57,14 +58,17 @@
 </a>
 <a href="https://codecov.io/gh/yezz123/authx">
     <img src="https://codecov.io/gh/yezz123/authx/branch/main/graph/badge.svg"/>
 </a>
 <a href="https://pepy.tech/project/authx" target="_blank">
     <img src="https://static.pepy.tech/badge/authx" alt="Test">
 </a>
+<a href="https://pydantic.dev" target="_blank">
+    <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/main/docs/badge/v2.json" alt="Pydantic Version 2">
+</a>
 </p>
 </p>
 
 ---
 
 **Source Code**: <https://github.com/yezz123/authx>
 
@@ -80,15 +84,15 @@
 >
 > [Authx V0.9.x](https://authx-v0.yezz.me/) This branch relates to development of authx V1 which is not yet ready for production use.
 >
 >If you're a Authx user, you probably want either Authx V0.9 [Documentation](https://authx-v0.yezz.me/) or, [0.X.X-fix](https://github.com/yezz123/authx/tree/0.X.X-fix) git branch.
 
 ## Features 🔧
 
-- [x] Support Python 3.8+.
+- [x] Support Python 3.8+ & Pydantic 2.0+.
 - [x] Multiple customizable authentication backend:
   - [x] JWT authentication backend included
     - [x] JWT encoding/decoding for application authentication
     - [x] Automatic detection of JWTs in requests:
       - [x] JWTs in headers
       - [x] JWTs in cookies
       - [x] JWTs in query parameters
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: authx Version: 1.0.1b0 Summary: Ready to use and
+Metadata-Version: 2.1 Name: authx Version: 1.0.1b1 Summary: Ready to use and
 customizable Authentications and Oauth2 management for FastAPI Project-URL:
 Homepage, https://github.com/yezz123/authx Project-URL: Documentation, https://
 authx.yezz.me/ Project-URL: Funding, https://github.com/sponsors/yezz123
 Author-email: Yasser Tahiri
 yezz.me> License-Expression: MIT License-File: LICENSE Keywords:
 Authentication,Cookie,FastAPI,JWT,Oauth2,Pydantic Classifier: Development
 Status :: 4 - Beta Classifier: Framework :: AsyncIO Classifier: Framework ::
@@ -14,39 +14,39 @@
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Internet Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed Requires-Python: >=3.8 Requires-Dist:
-fastapi<0.110.0,>=0.65.2 Requires-Dist: pydantic!=1.8,!=1.8.1,<2.0.0,>=1.7.4
-Requires-Dist: pyjwt[crypto]<3.0.0,>=2.6.0 Requires-Dist: python-
-dateutil<3.0.0,>=2.8 Requires-Dist: python-jose<4.0.0,>=3.3.0 Requires-Dist:
-pytz<2025.0,>=2023.3 Description-Content-Type: text/markdown # AuthenticationX
-ð«
+fastapi<0.110.0,>=0.65.2 Requires-Dist: pydantic-settings>=2.1.0 Requires-Dist:
+pydantic<2.6.1,>=2.0.0 Requires-Dist: pyjwt[crypto]<3.0.0,>=2.6.0 Requires-
+Dist: python-dateutil<3.0.0,>=2.8 Requires-Dist: python-jose<4.0.0,>=3.3.0
+Requires-Dist: pytz<2025.0,>=2023.3 Description-Content-Type: text/markdown #
+AuthenticationX ð«
                                     _[_A_u_t_h_X_]
 RReeaaddyy--ttoo--uussee aanndd ccuussttoommiizzaabbllee AAuutthheennttiiccaattiioonnss aanndd OOaauutthh22 mmaannaaggeemmeenntt ffoorr FFaassttAAPPII
                                       ?â??¡
 _[_l_i_n_t_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_y_e_z_z_1_2_3_/_a_u_t_h_x_/_b_r_a_n_c_h_/_m_a_i_n_/_g_r_a_p_h_/
-                               _b_a_d_g_e_._s_v_g_]_[_T_e_s_t_]
+                     _b_a_d_g_e_._s_v_g_]_[_T_e_s_t_]_[_P_y_d_a_n_t_i_c_ _V_e_r_s_i_o_n_ _2_]
 --- **Source Code**:
 github.com/yezz123/authx> **Documentation**:
 authx.yezz.me/> --- Add a Fully registration and authentication or
 authorization system to your [FastAPI](https://fastapi.tiangolo.com/) project.
 **AuthX** is designed to be as customizable and adaptable as possible. >
 **Notes**: > > [Authx V0.9.x](https://authx-v0.yezz.me/) This branch relates to
 development of authx V1 which is not yet ready for production use. > >If you're
 a Authx user, you probably want either Authx V0.9 [Documentation](https://
 authx-v0.yezz.me/) or, [0.X.X-fix](https://github.com/yezz123/authx/tree/0.X.X-
-fix) git branch. ## Features ð§ - [x] Support Python 3.8+. - [x] Multiple
-customizable authentication backend: - [x] JWT authentication backend included
-- [x] JWT encoding/decoding for application authentication - [x] Automatic
-detection of JWTs in requests: - [x] JWTs in headers - [x] JWTs in cookies -
-[x] JWTs in query parameters - [x] JWTs in request bodies - [x] Cookie
-authentication backend included - [x] middleware for authentication and
+fix) git branch. ## Features ð§ - [x] Support Python 3.8+ & Pydantic 2.0+. -
+[x] Multiple customizable authentication backend: - [x] JWT authentication
+backend included - [x] JWT encoding/decoding for application authentication -
+[x] Automatic detection of JWTs in requests: - [x] JWTs in headers - [x] JWTs
+in cookies - [x] JWTs in query parameters - [x] JWTs in request bodies - [x]
+Cookie authentication backend included - [x] middleware for authentication and
 authorization through JWT. - [x] Extensible Error Handling System. ### Extra
 Features ð AuthX is designed to be as customizable and adaptable as
 possible. So you need to install [`authx-extra`](https://github.com/yezz123/
 authx-extra) to get extra features. - [x] Using Redis as a session store &
 cache. - [x] Support HTTPCache. - [x] Support Sessions and Pre-built CRUD
 functions and Instance to launch Redis. - [x] Support Middleware of
 [pyinstrument](https://pyinstrument.readthedocs.io/) to check your service
```

