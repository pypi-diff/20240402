# Comparing `tmp/craft-application-2.2.0.tar.gz` & `tmp/craft-application-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "craft-application-2.2.0.tar", last modified: Thu Mar 28 20:35:39 2024, max compression
+gzip compressed data, was "craft-application-2.3.0.tar", last modified: Tue Apr  2 11:32:49 2024, max compression
```

## Comparing `craft-application-2.2.0.tar` & `craft-application-2.3.0.tar`

### file list

```diff
@@ -1,215 +1,215 @@
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:39.001208 craft-application-2.2.0/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      723 2023-09-29 14:32:21.000000 craft-application-2.2.0/.editorconfig
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.973208 craft-application-2.2.0/.github/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      518 2024-02-15 23:03:01.000000 craft-application-2.2.0/.github/.jira_sync_config.yaml
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.973208 craft-application-2.2.0/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1386 2023-09-29 14:32:21.000000 craft-application-2.2.0/.github/ISSUE_TEMPLATE/bug.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      389 2023-09-29 14:32:21.000000 craft-application-2.2.0/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      788 2023-09-29 14:32:21.000000 craft-application-2.2.0/.github/ISSUE_TEMPLATE/task.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      179 2023-09-29 14:32:21.000000 craft-application-2.2.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      506 2023-09-29 14:32:21.000000 craft-application-2.2.0/.github/release-drafter.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      506 2023-09-29 14:32:21.000000 craft-application-2.2.0/.github/release-drafter.yml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4699 2024-03-19 19:28:11.000000 craft-application-2.2.0/.github/renovate.json5
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.977208 craft-application-2.2.0/.github/workflows/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      179 2023-09-29 14:32:21.000000 craft-application-2.2.0/.github/workflows/cla-check.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      919 2024-02-15 23:03:01.000000 craft-application-2.2.0/.github/workflows/docs.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      346 2024-02-15 23:03:01.000000 craft-application-2.2.0/.github/workflows/release-drafter.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4541 2024-02-22 17:50:51.000000 craft-application-2.2.0/.github/workflows/tests.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1949 2023-09-29 14:32:21.000000 craft-application-2.2.0/.gitignore
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      921 2023-09-29 14:32:21.000000 craft-application-2.2.0/.pre-commit-config.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      395 2023-11-10 10:29:35.000000 craft-application-2.2.0/.readthedocs.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      188 2023-09-29 14:32:21.000000 craft-application-2.2.0/.yamllint.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4393 2024-03-12 17:53:13.000000 craft-application-2.2.0/HACKING.rst
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     7652 2023-09-29 14:32:21.000000 craft-application-2.2.0/LICENSE
--rw-r--r--   0 tiago     (1000) tiago     (1000)     3310 2024-03-28 20:35:39.001208 craft-application-2.2.0/PKG-INFO
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      552 2023-09-29 14:32:21.000000 craft-application-2.2.0/README.rst
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.977208 craft-application-2.2.0/craft_application/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1522 2024-03-28 20:33:36.000000 craft-application-2.2.0/craft_application/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      411 2024-03-28 20:35:38.000000 craft-application-2.2.0/craft_application/_version.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    28538 2024-03-28 20:33:36.000000 craft-application-2.2.0/craft_application/application.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.981208 craft-application-2.2.0/craft_application/commands/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1163 2023-12-06 11:10:45.000000 craft-application-2.2.0/craft_application/commands/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     7234 2024-03-12 17:53:13.000000 craft-application-2.2.0/craft_application/commands/base.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    12723 2024-03-12 17:53:13.000000 craft-application-2.2.0/craft_application/commands/lifecycle.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1608 2023-09-29 14:32:21.000000 craft-application-2.2.0/craft_application/commands/other.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     7040 2024-03-20 22:10:47.000000 craft-application-2.2.0/craft_application/errors.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2439 2024-02-22 17:50:51.000000 craft-application-2.2.0/craft_application/grammar.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.981208 craft-application-2.2.0/craft_application/launchpad/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1135 2024-02-15 23:03:01.000000 craft-application-2.2.0/craft_application/launchpad/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1000 2024-02-15 23:03:01.000000 craft-application-2.2.0/craft_application/launchpad/errors.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     8564 2024-02-26 17:15:25.000000 craft-application-2.2.0/craft_application/launchpad/launchpad.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.981208 craft-application-2.2.0/craft_application/launchpad/models/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      621 2024-02-26 17:15:16.000000 craft-application-2.2.0/craft_application/launchpad/models/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     6820 2024-02-26 17:15:16.000000 craft-application-2.2.0/craft_application/launchpad/models/base.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4927 2024-02-26 17:15:25.000000 craft-application-2.2.0/craft_application/launchpad/models/build.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     5292 2024-02-26 17:15:16.000000 craft-application-2.2.0/craft_application/launchpad/models/code.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2236 2024-02-26 17:15:16.000000 craft-application-2.2.0/craft_application/launchpad/models/distro.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3441 2024-02-28 16:38:56.000000 craft-application-2.2.0/craft_application/launchpad/models/project.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    16303 2024-03-21 21:55:13.000000 craft-application-2.2.0/craft_application/launchpad/models/recipe.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     6039 2024-02-22 17:50:51.000000 craft-application-2.2.0/craft_application/launchpad/util.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.981208 craft-application-2.2.0/craft_application/misc/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1637 2024-02-15 23:03:01.000000 craft-application-2.2.0/craft_application/misc/instance_bashrc
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.981208 craft-application-2.2.0/craft_application/models/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1421 2024-02-15 23:03:01.000000 craft-application-2.2.0/craft_application/models/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3725 2024-02-15 23:03:01.000000 craft-application-2.2.0/craft_application/models/base.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2935 2024-03-12 17:53:13.000000 craft-application-2.2.0/craft_application/models/constraints.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2507 2024-02-26 17:15:16.000000 craft-application-2.2.0/craft_application/models/grammar.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1175 2023-09-29 14:32:21.000000 craft-application-2.2.0/craft_application/models/metadata.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4752 2024-02-26 17:15:25.000000 craft-application-2.2.0/craft_application/models/project.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft-application-2.2.0/craft_application/py.typed
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.985208 craft-application-2.2.0/craft_application/remote/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1337 2024-03-12 17:53:13.000000 craft-application-2.2.0/craft_application/remote/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2329 2024-02-22 17:50:51.000000 craft-application-2.2.0/craft_application/remote/errors.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    11714 2024-02-19 13:41:42.000000 craft-application-2.2.0/craft_application/remote/git.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4206 2024-03-12 17:53:13.000000 craft-application-2.2.0/craft_application/remote/utils.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2070 2024-02-15 23:03:01.000000 craft-application-2.2.0/craft_application/remote/worktree.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     6731 2024-02-22 17:50:51.000000 craft-application-2.2.0/craft_application/secrets.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.985208 craft-application-2.2.0/craft_application/services/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1444 2024-02-15 23:03:01.000000 craft-application-2.2.0/craft_application/services/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2106 2024-02-15 23:03:01.000000 craft-application-2.2.0/craft_application/services/base.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    16057 2024-03-19 19:28:11.000000 craft-application-2.2.0/craft_application/services/lifecycle.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3128 2024-03-19 19:28:11.000000 craft-application-2.2.0/craft_application/services/package.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    12584 2024-03-12 17:53:13.000000 craft-application-2.2.0/craft_application/services/provider.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    12544 2024-02-26 17:15:25.000000 craft-application-2.2.0/craft_application/services/remotebuild.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4323 2024-02-15 23:03:01.000000 craft-application-2.2.0/craft_application/services/request.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4273 2024-02-15 23:03:01.000000 craft-application-2.2.0/craft_application/services/service_factory.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.985208 craft-application-2.2.0/craft_application/util/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1701 2024-03-12 17:53:13.000000 craft-application-2.2.0/craft_application/util/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2465 2024-02-22 17:50:51.000000 craft-application-2.2.0/craft_application/util/callbacks.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4170 2024-02-22 17:50:51.000000 craft-application-2.2.0/craft_application/util/error_formatting.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      950 2023-12-06 11:10:45.000000 craft-application-2.2.0/craft_application/util/logging.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1470 2024-02-15 23:03:01.000000 craft-application-2.2.0/craft_application/util/paths.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2494 2024-02-28 16:38:56.000000 craft-application-2.2.0/craft_application/util/platforms.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2065 2024-02-15 23:03:01.000000 craft-application-2.2.0/craft_application/util/repositories.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4110 2024-02-26 17:15:25.000000 craft-application-2.2.0/craft_application/util/snap_config.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2241 2024-03-12 17:53:13.000000 craft-application-2.2.0/craft_application/util/string.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4930 2024-03-19 19:28:11.000000 craft-application-2.2.0/craft_application/util/yaml.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:39.001208 craft-application-2.2.0/craft_application.egg-info/
--rw-r--r--   0 tiago     (1000) tiago     (1000)     3310 2024-03-28 20:35:38.000000 craft-application-2.2.0/craft_application.egg-info/PKG-INFO
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     5979 2024-03-28 20:35:38.000000 craft-application-2.2.0/craft_application.egg-info/SOURCES.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        1 2024-03-28 20:35:38.000000 craft-application-2.2.0/craft_application.egg-info/dependency_links.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      871 2024-03-28 20:35:38.000000 craft-application-2.2.0/craft_application.egg-info/requires.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       18 2024-03-28 20:35:38.000000 craft-application-2.2.0/craft_application.egg-info/top_level.txt
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.989208 craft-application-2.2.0/docs/
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.897205 craft-application-2.2.0/docs/_static/
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.989208 craft-application-2.2.0/docs/_static/css/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      481 2023-09-29 14:32:21.000000 craft-application-2.2.0/docs/_static/css/custom.css
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1684 2023-09-29 14:32:21.000000 craft-application-2.2.0/docs/conf.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.989208 craft-application-2.2.0/docs/explanation/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       72 2023-09-29 14:32:21.000000 craft-application-2.2.0/docs/explanation/index.rst
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.989208 craft-application-2.2.0/docs/howto/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       70 2023-09-29 14:32:21.000000 craft-application-2.2.0/docs/howto/index.rst
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1201 2023-09-29 14:32:21.000000 craft-application-2.2.0/docs/index.rst
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.989208 craft-application-2.2.0/docs/reference/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      142 2023-09-29 14:32:21.000000 craft-application-2.2.0/docs/reference/index.rst
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.989208 craft-application-2.2.0/docs/tutorials/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      238 2023-09-29 14:32:21.000000 craft-application-2.2.0/docs/tutorials/index.rst
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    10490 2024-03-28 20:33:36.000000 craft-application-2.2.0/pyproject.toml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       38 2024-03-28 20:35:39.001208 craft-application-2.2.0/setup.cfg
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.989208 craft-application-2.2.0/tests/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft-application-2.2.0/tests/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     8398 2024-02-28 16:38:56.000000 craft-application-2.2.0/tests/conftest.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.989208 craft-application-2.2.0/tests/integration/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft-application-2.2.0/tests/integration/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2733 2024-02-15 23:03:01.000000 craft-application-2.2.0/tests/integration/conftest.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.897205 craft-application-2.2.0/tests/integration/data/
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.989208 craft-application-2.2.0/tests/integration/data/build-secrets/
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.989208 craft-application-2.2.0/tests/integration/data/build-secrets/secret-source-folder/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       14 2023-10-19 21:00:44.000000 craft-application-2.2.0/tests/integration/data/build-secrets/secret-source-folder/source-file.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      442 2023-10-19 21:00:44.000000 craft-application-2.2.0/tests/integration/data/build-secrets/testcraft.yaml
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.897205 craft-application-2.2.0/tests/integration/data/invalid_projects/
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.989208 craft-application-2.2.0/tests/integration/data/invalid_projects/build-error/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      177 2023-10-25 15:47:00.000000 craft-application-2.2.0/tests/integration/data/invalid_projects/build-error/testcraft.yaml
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.897205 craft-application-2.2.0/tests/integration/data/valid_projects/
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.989208 craft-application-2.2.0/tests/integration/data/valid_projects/adoption/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       26 2024-02-26 17:15:25.000000 craft-application-2.2.0/tests/integration/data/valid_projects/adoption/stderr
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      209 2024-02-26 17:15:25.000000 craft-application-2.2.0/tests/integration/data/valid_projects/adoption/testcraft.yaml
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.989208 craft-application-2.2.0/tests/integration/data/valid_projects/basic/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       26 2024-02-26 17:15:25.000000 craft-application-2.2.0/tests/integration/data/valid_projects/basic/stderr
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      114 2024-02-26 17:15:25.000000 craft-application-2.2.0/tests/integration/data/valid_projects/basic/testcraft.yaml
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.989208 craft-application-2.2.0/tests/integration/data/valid_projects/environment/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       26 2024-02-26 17:15:25.000000 craft-application-2.2.0/tests/integration/data/valid_projects/environment/stderr
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      483 2024-02-26 17:15:25.000000 craft-application-2.2.0/tests/integration/data/valid_projects/environment/testcraft.yaml
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.989208 craft-application-2.2.0/tests/integration/data/valid_projects/grammar/
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.897205 craft-application-2.2.0/tests/integration/data/valid_projects/grammar/src/
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.989208 craft-application-2.2.0/tests/integration/data/valid_projects/grammar/src/on-amd64-to-amd64/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       18 2024-03-20 22:10:47.000000 craft-application-2.2.0/tests/integration/data/valid_projects/grammar/src/on-amd64-to-amd64/hello.txt
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.989208 craft-application-2.2.0/tests/integration/data/valid_projects/grammar/src/on-amd64-to-arm64/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       18 2024-03-20 22:10:47.000000 craft-application-2.2.0/tests/integration/data/valid_projects/grammar/src/on-amd64-to-arm64/hello.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       26 2024-03-20 22:10:47.000000 craft-application-2.2.0/tests/integration/data/valid_projects/grammar/stderr
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      229 2024-03-20 22:10:47.000000 craft-application-2.2.0/tests/integration/data/valid_projects/grammar/testcraft.yaml
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.989208 craft-application-2.2.0/tests/integration/launchpad/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2024-02-15 23:03:01.000000 craft-application-2.2.0/tests/integration/launchpad/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1021 2024-02-26 17:15:16.000000 craft-application-2.2.0/tests/integration/launchpad/conftest.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1647 2024-02-26 17:15:25.000000 craft-application-2.2.0/tests/integration/launchpad/test_anonymous_access.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.993208 craft-application-2.2.0/tests/integration/services/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft-application-2.2.0/tests/integration/services/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     5475 2024-02-28 16:38:56.000000 craft-application-2.2.0/tests/integration/services/test_lifecycle.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4287 2024-03-12 17:53:13.000000 craft-application-2.2.0/tests/integration/services/test_provider.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3445 2024-02-15 23:03:01.000000 craft-application-2.2.0/tests/integration/services/test_request.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1909 2024-02-28 16:38:56.000000 craft-application-2.2.0/tests/integration/services/test_service_factory.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    13467 2024-03-21 21:55:13.000000 craft-application-2.2.0/tests/integration/test_application.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2201 2023-09-29 14:32:21.000000 craft-application-2.2.0/tests/integration/test_version.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.993208 craft-application-2.2.0/tests/unit/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft-application-2.2.0/tests/unit/__init__.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.993208 craft-application-2.2.0/tests/unit/commands/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft-application-2.2.0/tests/unit/commands/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     6705 2023-12-06 11:10:45.000000 craft-application-2.2.0/tests/unit/commands/test_base.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    17375 2024-03-12 17:53:13.000000 craft-application-2.2.0/tests/unit/commands/test_lifecycle.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1363 2023-09-29 14:32:21.000000 craft-application-2.2.0/tests/unit/commands/test_other.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1673 2024-02-15 23:03:01.000000 craft-application-2.2.0/tests/unit/conftest.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.993208 craft-application-2.2.0/tests/unit/launchpad/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2024-02-15 23:03:01.000000 craft-application-2.2.0/tests/unit/launchpad/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1194 2024-02-26 17:15:16.000000 craft-application-2.2.0/tests/unit/launchpad/conftest.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.993208 craft-application-2.2.0/tests/unit/launchpad/models/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2024-02-15 23:03:01.000000 craft-application-2.2.0/tests/unit/launchpad/models/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     5159 2024-02-26 17:15:16.000000 craft-application-2.2.0/tests/unit/launchpad/models/test_base.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2562 2024-02-26 17:15:16.000000 craft-application-2.2.0/tests/unit/launchpad/models/test_code.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     9305 2024-03-21 21:55:13.000000 craft-application-2.2.0/tests/unit/launchpad/test_launchpad.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3500 2024-02-28 16:38:56.000000 craft-application-2.2.0/tests/unit/launchpad/test_util.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.993208 craft-application-2.2.0/tests/unit/models/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft-application-2.2.0/tests/unit/models/__init__.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.993208 craft-application-2.2.0/tests/unit/models/project_models/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       68 2023-09-29 14:32:21.000000 craft-application-2.2.0/tests/unit/models/project_models/basic_project.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      436 2023-09-29 14:32:21.000000 craft-application-2.2.0/tests/unit/models/project_models/full_project.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       24 2023-09-29 14:32:21.000000 craft-application-2.2.0/tests/unit/models/project_models/invalid_project.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4489 2024-02-15 23:03:01.000000 craft-application-2.2.0/tests/unit/models/test_constraints.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    10302 2024-02-26 17:15:16.000000 craft-application-2.2.0/tests/unit/models/test_project.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.997208 craft-application-2.2.0/tests/unit/remote/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2024-02-15 23:03:01.000000 craft-application-2.2.0/tests/unit/remote/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      855 2024-02-15 23:03:01.000000 craft-application-2.2.0/tests/unit/remote/conftest.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2116 2024-02-15 23:03:01.000000 craft-application-2.2.0/tests/unit/remote/test_errors.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    18388 2024-03-19 19:28:11.000000 craft-application-2.2.0/tests/unit/remote/test_git.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     5855 2024-03-12 17:53:13.000000 craft-application-2.2.0/tests/unit/remote/test_utils.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3034 2024-02-15 23:03:01.000000 craft-application-2.2.0/tests/unit/remote/test_worktree.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.997208 craft-application-2.2.0/tests/unit/services/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft-application-2.2.0/tests/unit/services/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3566 2024-02-15 23:03:01.000000 craft-application-2.2.0/tests/unit/services/conftest.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    20952 2024-03-19 19:28:11.000000 craft-application-2.2.0/tests/unit/services/test_lifecycle.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3413 2024-03-12 17:53:13.000000 craft-application-2.2.0/tests/unit/services/test_package.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    19466 2024-03-12 17:53:13.000000 craft-application-2.2.0/tests/unit/services/test_provider.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     7037 2024-02-26 17:15:16.000000 craft-application-2.2.0/tests/unit/services/test_remotebuild.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3629 2024-02-15 23:03:01.000000 craft-application-2.2.0/tests/unit/services/test_repositories.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4000 2024-02-15 23:03:01.000000 craft-application-2.2.0/tests/unit/services/test_request.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     5005 2024-02-26 17:15:25.000000 craft-application-2.2.0/tests/unit/services/test_service_factory.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    37411 2024-03-28 20:33:36.000000 craft-application-2.2.0/tests/unit/test_application.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2968 2024-02-15 23:03:01.000000 craft-application-2.2.0/tests/unit/test_errors.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     7670 2024-02-26 17:15:16.000000 craft-application-2.2.0/tests/unit/test_grammar.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       57 2023-09-29 14:32:21.000000 craft-application-2.2.0/tests/unit/test_nothing.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     5444 2023-10-19 21:00:44.000000 craft-application-2.2.0/tests/unit/test_secrets.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:38.997208 craft-application-2.2.0/tests/unit/util/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft-application-2.2.0/tests/unit/util/__init__.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:39.001208 craft-application-2.2.0/tests/unit/util/invalid_yaml/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      156 2023-09-29 14:32:21.000000 craft-application-2.2.0/tests/unit/util/invalid_yaml/_README
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       46 2023-09-29 14:32:21.000000 craft-application-2.2.0/tests/unit/util/invalid_yaml/duplicate_second_level.yaml-invalid
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       40 2023-09-29 14:32:21.000000 craft-application-2.2.0/tests/unit/util/invalid_yaml/duplicate_top_level.yaml-invalid
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       30 2023-09-29 14:32:21.000000 craft-application-2.2.0/tests/unit/util/invalid_yaml/unhashable.yaml-invalid
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3189 2023-12-07 17:42:39.000000 craft-application-2.2.0/tests/unit/util/test_error_formatting.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      603 2023-12-06 11:10:45.000000 craft-application-2.2.0/tests/unit/util/test_logging.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1573 2024-02-15 23:03:01.000000 craft-application-2.2.0/tests/unit/util/test_paths.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     5221 2024-02-26 17:15:25.000000 craft-application-2.2.0/tests/unit/util/test_snap_config.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3383 2024-03-12 17:53:13.000000 craft-application-2.2.0/tests/unit/util/test_string.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2992 2024-03-19 19:28:11.000000 craft-application-2.2.0/tests/unit/util/test_yaml.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-03-28 20:35:39.001208 craft-application-2.2.0/tests/unit/util/valid_yaml/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft-application-2.2.0/tests/unit/util/valid_yaml/empty.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4900 2024-02-28 18:07:23.000000 craft-application-2.2.0/tox.ini
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.563331 craft-application-2.3.0/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      723 2023-09-29 14:32:21.000000 craft-application-2.3.0/.editorconfig
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.535331 craft-application-2.3.0/.github/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      518 2024-02-15 23:03:01.000000 craft-application-2.3.0/.github/.jira_sync_config.yaml
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.535331 craft-application-2.3.0/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1386 2023-09-29 14:32:21.000000 craft-application-2.3.0/.github/ISSUE_TEMPLATE/bug.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      389 2023-09-29 14:32:21.000000 craft-application-2.3.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      788 2023-09-29 14:32:21.000000 craft-application-2.3.0/.github/ISSUE_TEMPLATE/task.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      179 2023-09-29 14:32:21.000000 craft-application-2.3.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      506 2023-09-29 14:32:21.000000 craft-application-2.3.0/.github/release-drafter.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      506 2023-09-29 14:32:21.000000 craft-application-2.3.0/.github/release-drafter.yml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4699 2024-03-19 19:28:11.000000 craft-application-2.3.0/.github/renovate.json5
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.539331 craft-application-2.3.0/.github/workflows/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      179 2023-09-29 14:32:21.000000 craft-application-2.3.0/.github/workflows/cla-check.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      919 2024-02-15 23:03:01.000000 craft-application-2.3.0/.github/workflows/docs.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      346 2024-02-15 23:03:01.000000 craft-application-2.3.0/.github/workflows/release-drafter.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4541 2024-02-22 17:50:51.000000 craft-application-2.3.0/.github/workflows/tests.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1949 2023-09-29 14:32:21.000000 craft-application-2.3.0/.gitignore
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      921 2023-09-29 14:32:21.000000 craft-application-2.3.0/.pre-commit-config.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      395 2023-11-10 10:29:35.000000 craft-application-2.3.0/.readthedocs.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      188 2023-09-29 14:32:21.000000 craft-application-2.3.0/.yamllint.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4393 2024-03-12 17:53:13.000000 craft-application-2.3.0/HACKING.rst
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     7652 2023-09-29 14:32:21.000000 craft-application-2.3.0/LICENSE
+-rw-r--r--   0 tiago     (1000) tiago     (1000)     3310 2024-04-02 11:32:49.563331 craft-application-2.3.0/PKG-INFO
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      552 2023-09-29 14:32:21.000000 craft-application-2.3.0/README.rst
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.539331 craft-application-2.3.0/craft_application/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1522 2024-03-28 20:33:36.000000 craft-application-2.3.0/craft_application/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      411 2024-04-02 11:32:49.000000 craft-application-2.3.0/craft_application/_version.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    29493 2024-04-02 11:30:59.000000 craft-application-2.3.0/craft_application/application.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.539331 craft-application-2.3.0/craft_application/commands/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1163 2023-12-06 11:10:45.000000 craft-application-2.3.0/craft_application/commands/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     7234 2024-03-12 17:53:13.000000 craft-application-2.3.0/craft_application/commands/base.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    12723 2024-03-12 17:53:13.000000 craft-application-2.3.0/craft_application/commands/lifecycle.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1608 2023-09-29 14:32:21.000000 craft-application-2.3.0/craft_application/commands/other.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     7040 2024-03-20 22:10:47.000000 craft-application-2.3.0/craft_application/errors.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2439 2024-02-22 17:50:51.000000 craft-application-2.3.0/craft_application/grammar.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.539331 craft-application-2.3.0/craft_application/launchpad/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1135 2024-02-15 23:03:01.000000 craft-application-2.3.0/craft_application/launchpad/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1000 2024-02-15 23:03:01.000000 craft-application-2.3.0/craft_application/launchpad/errors.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     8564 2024-02-26 17:15:25.000000 craft-application-2.3.0/craft_application/launchpad/launchpad.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.543331 craft-application-2.3.0/craft_application/launchpad/models/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      621 2024-02-26 17:15:16.000000 craft-application-2.3.0/craft_application/launchpad/models/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     6820 2024-02-26 17:15:16.000000 craft-application-2.3.0/craft_application/launchpad/models/base.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4927 2024-02-26 17:15:25.000000 craft-application-2.3.0/craft_application/launchpad/models/build.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5292 2024-02-26 17:15:16.000000 craft-application-2.3.0/craft_application/launchpad/models/code.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2236 2024-02-26 17:15:16.000000 craft-application-2.3.0/craft_application/launchpad/models/distro.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3441 2024-02-28 16:38:56.000000 craft-application-2.3.0/craft_application/launchpad/models/project.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    16303 2024-03-21 21:55:13.000000 craft-application-2.3.0/craft_application/launchpad/models/recipe.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     6039 2024-02-22 17:50:51.000000 craft-application-2.3.0/craft_application/launchpad/util.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.543331 craft-application-2.3.0/craft_application/misc/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1637 2024-02-15 23:03:01.000000 craft-application-2.3.0/craft_application/misc/instance_bashrc
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.543331 craft-application-2.3.0/craft_application/models/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1421 2024-02-15 23:03:01.000000 craft-application-2.3.0/craft_application/models/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3725 2024-02-15 23:03:01.000000 craft-application-2.3.0/craft_application/models/base.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2935 2024-03-12 17:53:13.000000 craft-application-2.3.0/craft_application/models/constraints.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2507 2024-02-26 17:15:16.000000 craft-application-2.3.0/craft_application/models/grammar.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1175 2023-09-29 14:32:21.000000 craft-application-2.3.0/craft_application/models/metadata.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4752 2024-02-26 17:15:25.000000 craft-application-2.3.0/craft_application/models/project.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft-application-2.3.0/craft_application/py.typed
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.543331 craft-application-2.3.0/craft_application/remote/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1337 2024-03-12 17:53:13.000000 craft-application-2.3.0/craft_application/remote/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2329 2024-02-22 17:50:51.000000 craft-application-2.3.0/craft_application/remote/errors.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    11714 2024-02-19 13:41:42.000000 craft-application-2.3.0/craft_application/remote/git.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4206 2024-03-12 17:53:13.000000 craft-application-2.3.0/craft_application/remote/utils.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2070 2024-02-15 23:03:01.000000 craft-application-2.3.0/craft_application/remote/worktree.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     6731 2024-02-22 17:50:51.000000 craft-application-2.3.0/craft_application/secrets.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.543331 craft-application-2.3.0/craft_application/services/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1444 2024-02-15 23:03:01.000000 craft-application-2.3.0/craft_application/services/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2106 2024-02-15 23:03:01.000000 craft-application-2.3.0/craft_application/services/base.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    16185 2024-04-02 11:30:59.000000 craft-application-2.3.0/craft_application/services/lifecycle.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3128 2024-03-19 19:28:11.000000 craft-application-2.3.0/craft_application/services/package.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    12545 2024-04-02 11:30:59.000000 craft-application-2.3.0/craft_application/services/provider.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    12544 2024-02-26 17:15:25.000000 craft-application-2.3.0/craft_application/services/remotebuild.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4323 2024-02-15 23:03:01.000000 craft-application-2.3.0/craft_application/services/request.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4273 2024-02-15 23:03:01.000000 craft-application-2.3.0/craft_application/services/service_factory.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.547331 craft-application-2.3.0/craft_application/util/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1701 2024-03-12 17:53:13.000000 craft-application-2.3.0/craft_application/util/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2465 2024-02-22 17:50:51.000000 craft-application-2.3.0/craft_application/util/callbacks.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4170 2024-02-22 17:50:51.000000 craft-application-2.3.0/craft_application/util/error_formatting.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      950 2023-12-06 11:10:45.000000 craft-application-2.3.0/craft_application/util/logging.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1470 2024-02-15 23:03:01.000000 craft-application-2.3.0/craft_application/util/paths.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2494 2024-02-28 16:38:56.000000 craft-application-2.3.0/craft_application/util/platforms.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2065 2024-02-15 23:03:01.000000 craft-application-2.3.0/craft_application/util/repositories.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4110 2024-02-26 17:15:25.000000 craft-application-2.3.0/craft_application/util/snap_config.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2241 2024-03-12 17:53:13.000000 craft-application-2.3.0/craft_application/util/string.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4930 2024-03-19 19:28:11.000000 craft-application-2.3.0/craft_application/util/yaml.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.559331 craft-application-2.3.0/craft_application.egg-info/
+-rw-r--r--   0 tiago     (1000) tiago     (1000)     3310 2024-04-02 11:32:49.000000 craft-application-2.3.0/craft_application.egg-info/PKG-INFO
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5979 2024-04-02 11:32:49.000000 craft-application-2.3.0/craft_application.egg-info/SOURCES.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        1 2024-04-02 11:32:49.000000 craft-application-2.3.0/craft_application.egg-info/dependency_links.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      871 2024-04-02 11:32:49.000000 craft-application-2.3.0/craft_application.egg-info/requires.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       18 2024-04-02 11:32:49.000000 craft-application-2.3.0/craft_application.egg-info/top_level.txt
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.547331 craft-application-2.3.0/docs/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.531331 craft-application-2.3.0/docs/_static/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.547331 craft-application-2.3.0/docs/_static/css/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      481 2023-09-29 14:32:21.000000 craft-application-2.3.0/docs/_static/css/custom.css
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1684 2023-09-29 14:32:21.000000 craft-application-2.3.0/docs/conf.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.547331 craft-application-2.3.0/docs/explanation/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       72 2023-09-29 14:32:21.000000 craft-application-2.3.0/docs/explanation/index.rst
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.547331 craft-application-2.3.0/docs/howto/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       70 2023-09-29 14:32:21.000000 craft-application-2.3.0/docs/howto/index.rst
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1201 2023-09-29 14:32:21.000000 craft-application-2.3.0/docs/index.rst
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.547331 craft-application-2.3.0/docs/reference/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      142 2023-09-29 14:32:21.000000 craft-application-2.3.0/docs/reference/index.rst
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.547331 craft-application-2.3.0/docs/tutorials/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      238 2023-09-29 14:32:21.000000 craft-application-2.3.0/docs/tutorials/index.rst
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    10490 2024-04-02 11:30:59.000000 craft-application-2.3.0/pyproject.toml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       38 2024-04-02 11:32:49.563331 craft-application-2.3.0/setup.cfg
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.547331 craft-application-2.3.0/tests/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft-application-2.3.0/tests/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     8870 2024-04-02 11:30:59.000000 craft-application-2.3.0/tests/conftest.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.547331 craft-application-2.3.0/tests/integration/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft-application-2.3.0/tests/integration/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2733 2024-02-15 23:03:01.000000 craft-application-2.3.0/tests/integration/conftest.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.531331 craft-application-2.3.0/tests/integration/data/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.547331 craft-application-2.3.0/tests/integration/data/build-secrets/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.547331 craft-application-2.3.0/tests/integration/data/build-secrets/secret-source-folder/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       14 2023-10-19 21:00:44.000000 craft-application-2.3.0/tests/integration/data/build-secrets/secret-source-folder/source-file.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      442 2023-10-19 21:00:44.000000 craft-application-2.3.0/tests/integration/data/build-secrets/testcraft.yaml
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.531331 craft-application-2.3.0/tests/integration/data/invalid_projects/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.547331 craft-application-2.3.0/tests/integration/data/invalid_projects/build-error/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      177 2023-10-25 15:47:00.000000 craft-application-2.3.0/tests/integration/data/invalid_projects/build-error/testcraft.yaml
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.531331 craft-application-2.3.0/tests/integration/data/valid_projects/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.547331 craft-application-2.3.0/tests/integration/data/valid_projects/adoption/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       26 2024-02-26 17:15:25.000000 craft-application-2.3.0/tests/integration/data/valid_projects/adoption/stderr
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      209 2024-02-26 17:15:25.000000 craft-application-2.3.0/tests/integration/data/valid_projects/adoption/testcraft.yaml
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.547331 craft-application-2.3.0/tests/integration/data/valid_projects/basic/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       26 2024-02-26 17:15:25.000000 craft-application-2.3.0/tests/integration/data/valid_projects/basic/stderr
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      114 2024-02-26 17:15:25.000000 craft-application-2.3.0/tests/integration/data/valid_projects/basic/testcraft.yaml
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.547331 craft-application-2.3.0/tests/integration/data/valid_projects/environment/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       26 2024-02-26 17:15:25.000000 craft-application-2.3.0/tests/integration/data/valid_projects/environment/stderr
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      483 2024-02-26 17:15:25.000000 craft-application-2.3.0/tests/integration/data/valid_projects/environment/testcraft.yaml
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.551331 craft-application-2.3.0/tests/integration/data/valid_projects/grammar/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.531331 craft-application-2.3.0/tests/integration/data/valid_projects/grammar/src/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.551331 craft-application-2.3.0/tests/integration/data/valid_projects/grammar/src/on-amd64-to-amd64/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       18 2024-03-20 22:10:47.000000 craft-application-2.3.0/tests/integration/data/valid_projects/grammar/src/on-amd64-to-amd64/hello.txt
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.551331 craft-application-2.3.0/tests/integration/data/valid_projects/grammar/src/on-amd64-to-arm64/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       18 2024-03-20 22:10:47.000000 craft-application-2.3.0/tests/integration/data/valid_projects/grammar/src/on-amd64-to-arm64/hello.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       26 2024-03-20 22:10:47.000000 craft-application-2.3.0/tests/integration/data/valid_projects/grammar/stderr
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      229 2024-03-20 22:10:47.000000 craft-application-2.3.0/tests/integration/data/valid_projects/grammar/testcraft.yaml
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.551331 craft-application-2.3.0/tests/integration/launchpad/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2024-02-15 23:03:01.000000 craft-application-2.3.0/tests/integration/launchpad/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1021 2024-02-26 17:15:16.000000 craft-application-2.3.0/tests/integration/launchpad/conftest.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1647 2024-02-26 17:15:25.000000 craft-application-2.3.0/tests/integration/launchpad/test_anonymous_access.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.551331 craft-application-2.3.0/tests/integration/services/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft-application-2.3.0/tests/integration/services/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5475 2024-02-28 16:38:56.000000 craft-application-2.3.0/tests/integration/services/test_lifecycle.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4287 2024-03-12 17:53:13.000000 craft-application-2.3.0/tests/integration/services/test_provider.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3445 2024-02-15 23:03:01.000000 craft-application-2.3.0/tests/integration/services/test_request.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1909 2024-02-28 16:38:56.000000 craft-application-2.3.0/tests/integration/services/test_service_factory.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    13467 2024-03-21 21:55:13.000000 craft-application-2.3.0/tests/integration/test_application.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2201 2023-09-29 14:32:21.000000 craft-application-2.3.0/tests/integration/test_version.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.551331 craft-application-2.3.0/tests/unit/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft-application-2.3.0/tests/unit/__init__.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.551331 craft-application-2.3.0/tests/unit/commands/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft-application-2.3.0/tests/unit/commands/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     6705 2023-12-06 11:10:45.000000 craft-application-2.3.0/tests/unit/commands/test_base.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    17375 2024-03-12 17:53:13.000000 craft-application-2.3.0/tests/unit/commands/test_lifecycle.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1363 2023-09-29 14:32:21.000000 craft-application-2.3.0/tests/unit/commands/test_other.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1673 2024-02-15 23:03:01.000000 craft-application-2.3.0/tests/unit/conftest.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.555331 craft-application-2.3.0/tests/unit/launchpad/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2024-02-15 23:03:01.000000 craft-application-2.3.0/tests/unit/launchpad/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1194 2024-02-26 17:15:16.000000 craft-application-2.3.0/tests/unit/launchpad/conftest.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.555331 craft-application-2.3.0/tests/unit/launchpad/models/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2024-02-15 23:03:01.000000 craft-application-2.3.0/tests/unit/launchpad/models/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5159 2024-02-26 17:15:16.000000 craft-application-2.3.0/tests/unit/launchpad/models/test_base.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2562 2024-02-26 17:15:16.000000 craft-application-2.3.0/tests/unit/launchpad/models/test_code.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     9305 2024-03-21 21:55:13.000000 craft-application-2.3.0/tests/unit/launchpad/test_launchpad.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3500 2024-02-28 16:38:56.000000 craft-application-2.3.0/tests/unit/launchpad/test_util.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.555331 craft-application-2.3.0/tests/unit/models/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft-application-2.3.0/tests/unit/models/__init__.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.555331 craft-application-2.3.0/tests/unit/models/project_models/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       68 2023-09-29 14:32:21.000000 craft-application-2.3.0/tests/unit/models/project_models/basic_project.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      436 2023-09-29 14:32:21.000000 craft-application-2.3.0/tests/unit/models/project_models/full_project.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       24 2023-09-29 14:32:21.000000 craft-application-2.3.0/tests/unit/models/project_models/invalid_project.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4489 2024-02-15 23:03:01.000000 craft-application-2.3.0/tests/unit/models/test_constraints.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    10302 2024-02-26 17:15:16.000000 craft-application-2.3.0/tests/unit/models/test_project.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.555331 craft-application-2.3.0/tests/unit/remote/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2024-02-15 23:03:01.000000 craft-application-2.3.0/tests/unit/remote/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      855 2024-02-15 23:03:01.000000 craft-application-2.3.0/tests/unit/remote/conftest.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2116 2024-02-15 23:03:01.000000 craft-application-2.3.0/tests/unit/remote/test_errors.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    18388 2024-03-19 19:28:11.000000 craft-application-2.3.0/tests/unit/remote/test_git.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5855 2024-03-12 17:53:13.000000 craft-application-2.3.0/tests/unit/remote/test_utils.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3034 2024-02-15 23:03:01.000000 craft-application-2.3.0/tests/unit/remote/test_worktree.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.555331 craft-application-2.3.0/tests/unit/services/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft-application-2.3.0/tests/unit/services/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3566 2024-02-15 23:03:01.000000 craft-application-2.3.0/tests/unit/services/conftest.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    21558 2024-04-02 11:30:59.000000 craft-application-2.3.0/tests/unit/services/test_lifecycle.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3413 2024-03-12 17:53:13.000000 craft-application-2.3.0/tests/unit/services/test_package.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    19346 2024-04-02 11:30:59.000000 craft-application-2.3.0/tests/unit/services/test_provider.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     7037 2024-02-26 17:15:16.000000 craft-application-2.3.0/tests/unit/services/test_remotebuild.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3629 2024-02-15 23:03:01.000000 craft-application-2.3.0/tests/unit/services/test_repositories.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4000 2024-02-15 23:03:01.000000 craft-application-2.3.0/tests/unit/services/test_request.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5005 2024-02-26 17:15:25.000000 craft-application-2.3.0/tests/unit/services/test_service_factory.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    39437 2024-04-02 11:30:59.000000 craft-application-2.3.0/tests/unit/test_application.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2968 2024-02-15 23:03:01.000000 craft-application-2.3.0/tests/unit/test_errors.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     7670 2024-02-26 17:15:16.000000 craft-application-2.3.0/tests/unit/test_grammar.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       57 2023-09-29 14:32:21.000000 craft-application-2.3.0/tests/unit/test_nothing.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5444 2023-10-19 21:00:44.000000 craft-application-2.3.0/tests/unit/test_secrets.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.559331 craft-application-2.3.0/tests/unit/util/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft-application-2.3.0/tests/unit/util/__init__.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.559331 craft-application-2.3.0/tests/unit/util/invalid_yaml/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      156 2023-09-29 14:32:21.000000 craft-application-2.3.0/tests/unit/util/invalid_yaml/_README
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       46 2023-09-29 14:32:21.000000 craft-application-2.3.0/tests/unit/util/invalid_yaml/duplicate_second_level.yaml-invalid
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       40 2023-09-29 14:32:21.000000 craft-application-2.3.0/tests/unit/util/invalid_yaml/duplicate_top_level.yaml-invalid
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       30 2023-09-29 14:32:21.000000 craft-application-2.3.0/tests/unit/util/invalid_yaml/unhashable.yaml-invalid
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3189 2023-12-07 17:42:39.000000 craft-application-2.3.0/tests/unit/util/test_error_formatting.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      603 2023-12-06 11:10:45.000000 craft-application-2.3.0/tests/unit/util/test_logging.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1573 2024-02-15 23:03:01.000000 craft-application-2.3.0/tests/unit/util/test_paths.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5221 2024-02-26 17:15:25.000000 craft-application-2.3.0/tests/unit/util/test_snap_config.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3383 2024-03-12 17:53:13.000000 craft-application-2.3.0/tests/unit/util/test_string.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2992 2024-03-19 19:28:11.000000 craft-application-2.3.0/tests/unit/util/test_yaml.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-02 11:32:49.559331 craft-application-2.3.0/tests/unit/util/valid_yaml/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft-application-2.3.0/tests/unit/util/valid_yaml/empty.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4900 2024-02-28 18:07:23.000000 craft-application-2.3.0/tox.ini
```

### Comparing `craft-application-2.2.0/.editorconfig` & `craft-application-2.3.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/.github/.jira_sync_config.yaml` & `craft-application-2.3.0/.github/.jira_sync_config.yaml`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/.github/ISSUE_TEMPLATE/bug.yaml` & `craft-application-2.3.0/.github/ISSUE_TEMPLATE/bug.yaml`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/.github/ISSUE_TEMPLATE/task.yaml` & `craft-application-2.3.0/.github/ISSUE_TEMPLATE/task.yaml`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/.github/renovate.json5` & `craft-application-2.3.0/.github/renovate.json5`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/.github/workflows/docs.yaml` & `craft-application-2.3.0/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/.github/workflows/tests.yaml` & `craft-application-2.3.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/.gitignore` & `craft-application-2.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/.pre-commit-config.yaml` & `craft-application-2.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/HACKING.rst` & `craft-application-2.3.0/HACKING.rst`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/LICENSE` & `craft-application-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/PKG-INFO` & `craft-application-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-application
-Version: 2.2.0
+Version: 2.3.0
 Summary: A framework for *craft applications.
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.10
@@ -26,32 +26,32 @@
 Requires-Dist: pydantic-yaml<1.0
 Requires-Dist: pygit2<1.15.0,>=1.13.0
 Requires-Dist: PyYaml>=6.0
 Requires-Dist: typing_extensions>=4.4.0
 Provides-Extra: remote
 Requires-Dist: launchpadlib>=1.10.16; extra == "remote"
 Provides-Extra: dev
-Requires-Dist: coverage[toml]==7.4.3; extra == "dev"
+Requires-Dist: coverage[toml]==7.4.4; extra == "dev"
 Requires-Dist: hypothesis>=6.0; extra == "dev"
 Requires-Dist: pyfakefs~=5.3; extra == "dev"
 Requires-Dist: pytest==8.1.1; extra == "dev"
 Requires-Dist: pytest-check==2.3.1; extra == "dev"
 Requires-Dist: pytest-cov==5.0.0; extra == "dev"
-Requires-Dist: pytest-mock==3.12.0; extra == "dev"
+Requires-Dist: pytest-mock==3.14.0; extra == "dev"
 Requires-Dist: pytest-rerunfailures==13.0; extra == "dev"
 Requires-Dist: pytest-time>=0.3.1; extra == "dev"
 Requires-Dist: responses~=0.25.0; extra == "dev"
 Requires-Dist: craft-application[remote]; extra == "dev"
 Provides-Extra: lint
 Requires-Dist: black~=24.0; extra == "lint"
 Requires-Dist: codespell[toml]==2.2.6; extra == "lint"
 Requires-Dist: yamllint==1.35.1; extra == "lint"
 Provides-Extra: types
 Requires-Dist: mypy[reports]==1.9.0; extra == "types"
-Requires-Dist: pyright==1.1.353; extra == "types"
+Requires-Dist: pyright==1.1.356; extra == "types"
 Requires-Dist: types-requests; extra == "types"
 Requires-Dist: types-urllib3; extra == "types"
 Provides-Extra: docs
 Requires-Dist: furo==2024.1.29; extra == "docs"
 Requires-Dist: sphinx<7.3,>=7.2.6; extra == "docs"
 Requires-Dist: sphinx-autobuild==2024.2.4; extra == "docs"
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "docs"
```

### Comparing `craft-application-2.2.0/README.rst` & `craft-application-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/__init__.py` & `craft-application-2.3.0/craft_application/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/application.py` & `craft-application-2.3.0/craft_application/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,15 @@
         self._global_arguments: list[craft_cli.GlobalArgument] = [GLOBAL_VERSION]
         self._cli_loggers = DEFAULT_CLI_LOGGERS | set(extra_loggers)
         self._full_build_plan: list[models.BuildInfo] = []
         self._build_plan: list[models.BuildInfo] = []
         # When build_secrets are enabled, this contains the secret info to pass to
         # managed instances.
         self._secrets: secrets.BuildSecrets | None = None
+        self._partitions: list[str] | None = None
         # Cached project object, allows only the first time we load the project
         # to specify things like the project directory.
         # This is set as a private attribute in order to discourage real application
         # implementations from accessing it directly. They should always use
         # ``get_project`` to access the project.
         self.__project: models.Project | None = None
         # Set a globally usable project directory for the application.
@@ -215,14 +216,15 @@
         provide a valid ``project`` to ``self.services``.
         """
         self.services.set_kwargs(
             "lifecycle",
             cache_dir=self.cache_dir,
             work_dir=self._work_dir,
             build_plan=self._build_plan,
+            partitions=self._partitions,
         )
         self.services.set_kwargs(
             "provider",
             work_dir=self._work_dir,
             build_plan=self._build_plan,
             provider_name=provider_name,
         )
@@ -284,14 +286,17 @@
                 raise errors.InvalidPlatformError(platform, list(all_platforms.keys()))
             build_for = all_platforms[platform].build_for
 
         # validate project grammar
         GrammarAwareProject.validate_grammar(yaml_data)
 
         build_on = host_arch
+
+        # Setup partitions, some projects require the yaml data, most will not
+        self._partitions = self._setup_partitions(yaml_data)
         yaml_data = self._transform_project_yaml(yaml_data, build_on, build_for)
         self.__project = self.app.ProjectClass.from_yaml_data(yaml_data, project_path)
 
         # check if mandatory adoptable fields exist if adopt-info not used
         for name in self.app.mandatory_adoptable_fields:
             if (
                 not getattr(self.__project, name, None)
@@ -340,22 +345,27 @@
                 f"Running {self.app.name}:{build_info.platform} in {build_info.build_for} instance..."
             )
             instance_path = pathlib.PosixPath("/root/project")
 
             with self.services.provider.instance(
                 build_info, work_dir=self._work_dir
             ) as instance:
+                cmd = [self.app.name, *sys.argv[1:]]
+                craft_cli.emit.debug(
+                    f"Executing {cmd} in instance location {instance_path} with {extra_args}."
+                )
                 try:
-                    # Pyright doesn't fully understand craft_providers's CompletedProcess.
-                    instance.execute_run(  # pyright: ignore[reportUnknownMemberType,reportUnknownVariableType]
-                        [self.app.name, *sys.argv[1:]],
-                        cwd=instance_path,
-                        check=True,
-                        **extra_args,
-                    )
+                    with craft_cli.emit.pause():
+                        # Pyright doesn't fully understand craft_providers's CompletedProcess.
+                        instance.execute_run(  # pyright: ignore[reportUnknownMemberType,reportUnknownVariableType]
+                            cmd,
+                            cwd=instance_path,
+                            check=True,
+                            **extra_args,
+                        )
                 except subprocess.CalledProcessError as exc:
                     raise craft_providers.ProviderError(
                         f"Failed to execute {self.app.name} in instance."
                     ) from exc
 
     def configure(self, global_args: dict[str, Any]) -> None:
         """Configure the application using any global arguments."""
@@ -599,26 +609,40 @@
         return self._extra_yaml_transform(
             yaml_data, build_on=build_on, build_for=build_for
         )
 
     def _expand_environment(self, yaml_data: dict[str, Any]) -> None:
         """Perform expansion of project environment variables."""
         environment_vars = self._get_project_vars(yaml_data)
+        project_dirs = craft_parts.ProjectDirs(
+            work_dir=self._work_dir, partitions=self._partitions
+        )
+
         info = craft_parts.ProjectInfo(
             application_name=self.app.name,  # not used in environment expansion
             cache_dir=pathlib.Path(),  # not used in environment expansion
             project_name=yaml_data.get("name", ""),
-            project_dirs=craft_parts.ProjectDirs(work_dir=self._work_dir),
+            project_dirs=project_dirs,
             project_vars=environment_vars,
+            partitions=self._partitions,
         )
 
         self._set_global_environment(info)
 
         craft_parts.expand_environment(yaml_data, info=info)
 
+    def _setup_partitions(self, yaml_data: dict[str, Any]) -> list[str] | None:
+        """Return partitions to be used.
+
+        When returning you will also need to ensure that the feature is enabled
+        on Application instantiation craft_parts.Features(partitions_enabled=True)
+        """
+        _ = yaml_data
+        return None
+
     def _get_project_vars(self, yaml_data: dict[str, Any]) -> dict[str, str]:
         """Return a dict with project variables to be expanded."""
         pvars: dict[str, str] = {}
         for var in self.app.project_variables:
             pvars[var] = yaml_data.get(var, "")
         return pvars
```

### Comparing `craft-application-2.2.0/craft_application/commands/__init__.py` & `craft-application-2.3.0/craft_application/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/commands/base.py` & `craft-application-2.3.0/craft_application/commands/base.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/commands/lifecycle.py` & `craft-application-2.3.0/craft_application/commands/lifecycle.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/commands/other.py` & `craft-application-2.3.0/craft_application/commands/other.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/errors.py` & `craft-application-2.3.0/craft_application/errors.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/grammar.py` & `craft-application-2.3.0/craft_application/grammar.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/launchpad/__init__.py` & `craft-application-2.3.0/craft_application/launchpad/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/launchpad/errors.py` & `craft-application-2.3.0/craft_application/launchpad/errors.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/launchpad/launchpad.py` & `craft-application-2.3.0/craft_application/launchpad/launchpad.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/launchpad/models/__init__.py` & `craft-application-2.3.0/craft_application/launchpad/models/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/launchpad/models/base.py` & `craft-application-2.3.0/craft_application/launchpad/models/base.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/launchpad/models/build.py` & `craft-application-2.3.0/craft_application/launchpad/models/build.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/launchpad/models/code.py` & `craft-application-2.3.0/craft_application/launchpad/models/code.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/launchpad/models/distro.py` & `craft-application-2.3.0/craft_application/launchpad/models/distro.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/launchpad/models/project.py` & `craft-application-2.3.0/craft_application/launchpad/models/project.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/launchpad/models/recipe.py` & `craft-application-2.3.0/craft_application/launchpad/models/recipe.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/launchpad/util.py` & `craft-application-2.3.0/craft_application/launchpad/util.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/misc/instance_bashrc` & `craft-application-2.3.0/craft_application/misc/instance_bashrc`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/models/__init__.py` & `craft-application-2.3.0/craft_application/models/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/models/base.py` & `craft-application-2.3.0/craft_application/models/base.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/models/constraints.py` & `craft-application-2.3.0/craft_application/models/constraints.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/models/grammar.py` & `craft-application-2.3.0/craft_application/models/grammar.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/models/metadata.py` & `craft-application-2.3.0/craft_application/models/metadata.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/models/project.py` & `craft-application-2.3.0/craft_application/models/project.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/remote/__init__.py` & `craft-application-2.3.0/craft_application/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/remote/errors.py` & `craft-application-2.3.0/craft_application/remote/errors.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/remote/git.py` & `craft-application-2.3.0/craft_application/remote/git.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/remote/utils.py` & `craft-application-2.3.0/craft_application/remote/utils.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/remote/worktree.py` & `craft-application-2.3.0/craft_application/remote/worktree.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/secrets.py` & `craft-application-2.3.0/craft_application/secrets.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/services/__init__.py` & `craft-application-2.3.0/craft_application/services/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/services/base.py` & `craft-application-2.3.0/craft_application/services/base.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/services/lifecycle.py` & `craft-application-2.3.0/craft_application/services/lifecycle.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,20 +130,22 @@
         app: AppMetadata,
         services: ServiceFactory,
         *,
         project: Project,
         work_dir: Path | str,
         cache_dir: Path | str,
         build_plan: list[models.BuildInfo],
+        partitions: list[str] | None = None,
         **lifecycle_kwargs: Any,  # noqa: ANN401 - eventually used in an Any
     ) -> None:
         super().__init__(app, services, project=project)
         self._work_dir = work_dir
         self._cache_dir = cache_dir
         self._build_plan = build_plan
+        self._partitions = partitions
         self._manager_kwargs = lifecycle_kwargs
         self._lcm: LifecycleManager = None  # type: ignore[assignment]
 
     @override
     def setup(self) -> None:
         """Initialize the LifecycleManager with previously-set arguments."""
         self._lcm = self._init_lifecycle_manager()
@@ -186,14 +188,15 @@
                 cache_dir=self._cache_dir,
                 work_dir=self._work_dir,
                 ignore_local_sources=self._app.source_ignore_patterns,
                 parallel_build_count=self._get_parallel_build_count(),
                 project_vars_part_name=self._project.adopt_info,
                 project_vars=self._project_vars,
                 track_stage_packages=True,
+                partitions=self._partitions,
                 **self._manager_kwargs,
             )
         except PartsError as err:
             raise errors.PartsLifecycleError.from_parts_error(err) from err
 
     @property
     def prime_dir(self) -> Path:
```

### Comparing `craft-application-2.2.0/craft_application/services/package.py` & `craft-application-2.3.0/craft_application/services/package.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/services/provider.py` & `craft-application-2.3.0/craft_application/services/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,16 +129,15 @@
                 # Ignore argument type until craft-providers accepts PurePosixPaths
                 # https://github.com/canonical/craft-providers/issues/315
                 target=self._app.managed_instance_project_path,  # type: ignore[arg-type]
             )
             emit.debug("Instance launched and working directory mounted")
             self._setup_instance_bashrc(instance)
             try:
-                with emit.pause():
-                    yield instance
+                yield instance
             finally:
                 self._capture_logs_from_instance(instance)
 
     def get_base(
         self,
         base_name: bases.BaseName | tuple[str, str],
         *,
```

### Comparing `craft-application-2.2.0/craft_application/services/remotebuild.py` & `craft-application-2.3.0/craft_application/services/remotebuild.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/services/request.py` & `craft-application-2.3.0/craft_application/services/request.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/services/service_factory.py` & `craft-application-2.3.0/craft_application/services/service_factory.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/util/__init__.py` & `craft-application-2.3.0/craft_application/util/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/util/callbacks.py` & `craft-application-2.3.0/craft_application/util/callbacks.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/util/error_formatting.py` & `craft-application-2.3.0/craft_application/util/error_formatting.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/util/logging.py` & `craft-application-2.3.0/craft_application/util/logging.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/util/paths.py` & `craft-application-2.3.0/craft_application/util/paths.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/util/platforms.py` & `craft-application-2.3.0/craft_application/util/platforms.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/util/repositories.py` & `craft-application-2.3.0/craft_application/util/repositories.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/util/snap_config.py` & `craft-application-2.3.0/craft_application/util/snap_config.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/util/string.py` & `craft-application-2.3.0/craft_application/util/string.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application/util/yaml.py` & `craft-application-2.3.0/craft_application/util/yaml.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application.egg-info/PKG-INFO` & `craft-application-2.3.0/craft_application.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-application
-Version: 2.2.0
+Version: 2.3.0
 Summary: A framework for *craft applications.
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.10
@@ -26,32 +26,32 @@
 Requires-Dist: pydantic-yaml<1.0
 Requires-Dist: pygit2<1.15.0,>=1.13.0
 Requires-Dist: PyYaml>=6.0
 Requires-Dist: typing_extensions>=4.4.0
 Provides-Extra: remote
 Requires-Dist: launchpadlib>=1.10.16; extra == "remote"
 Provides-Extra: dev
-Requires-Dist: coverage[toml]==7.4.3; extra == "dev"
+Requires-Dist: coverage[toml]==7.4.4; extra == "dev"
 Requires-Dist: hypothesis>=6.0; extra == "dev"
 Requires-Dist: pyfakefs~=5.3; extra == "dev"
 Requires-Dist: pytest==8.1.1; extra == "dev"
 Requires-Dist: pytest-check==2.3.1; extra == "dev"
 Requires-Dist: pytest-cov==5.0.0; extra == "dev"
-Requires-Dist: pytest-mock==3.12.0; extra == "dev"
+Requires-Dist: pytest-mock==3.14.0; extra == "dev"
 Requires-Dist: pytest-rerunfailures==13.0; extra == "dev"
 Requires-Dist: pytest-time>=0.3.1; extra == "dev"
 Requires-Dist: responses~=0.25.0; extra == "dev"
 Requires-Dist: craft-application[remote]; extra == "dev"
 Provides-Extra: lint
 Requires-Dist: black~=24.0; extra == "lint"
 Requires-Dist: codespell[toml]==2.2.6; extra == "lint"
 Requires-Dist: yamllint==1.35.1; extra == "lint"
 Provides-Extra: types
 Requires-Dist: mypy[reports]==1.9.0; extra == "types"
-Requires-Dist: pyright==1.1.353; extra == "types"
+Requires-Dist: pyright==1.1.356; extra == "types"
 Requires-Dist: types-requests; extra == "types"
 Requires-Dist: types-urllib3; extra == "types"
 Provides-Extra: docs
 Requires-Dist: furo==2024.1.29; extra == "docs"
 Requires-Dist: sphinx<7.3,>=7.2.6; extra == "docs"
 Requires-Dist: sphinx-autobuild==2024.2.4; extra == "docs"
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "docs"
```

### Comparing `craft-application-2.2.0/craft_application.egg-info/SOURCES.txt` & `craft-application-2.3.0/craft_application.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/craft_application.egg-info/requires.txt` & `craft-application-2.3.0/craft_application.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 
 [apt]
 
 [apt:sys_platform == "linux"]
 python-apt>=2.4.0
 
 [dev]
-coverage[toml]==7.4.3
+coverage[toml]==7.4.4
 hypothesis>=6.0
 pyfakefs~=5.3
 pytest==8.1.1
 pytest-check==2.3.1
 pytest-cov==5.0.0
-pytest-mock==3.12.0
+pytest-mock==3.14.0
 pytest-rerunfailures==13.0
 pytest-time>=0.3.1
 responses~=0.25.0
 craft-application[remote]
 
 [docs]
 furo==2024.1.29
@@ -45,10 +45,10 @@
 yamllint==1.35.1
 
 [remote]
 launchpadlib>=1.10.16
 
 [types]
 mypy[reports]==1.9.0
-pyright==1.1.353
+pyright==1.1.356
 types-requests
 types-urllib3
```

### Comparing `craft-application-2.2.0/docs/conf.py` & `craft-application-2.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/docs/index.rst` & `craft-application-2.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/pyproject.toml` & `craft-application-2.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -41,34 +41,34 @@
 
 [project.optional-dependencies]
 remote = [
     # Support for remote-build is optional.
     "launchpadlib>=1.10.16",
 ]
 dev = [
-    "coverage[toml]==7.4.3",
+    "coverage[toml]==7.4.4",
     "hypothesis>=6.0",
     "pyfakefs~=5.3",
     "pytest==8.1.1",
     "pytest-check==2.3.1",
     "pytest-cov==5.0.0",
-    "pytest-mock==3.12.0",
+    "pytest-mock==3.14.0",
     "pytest-rerunfailures==13.0",
     "pytest-time>=0.3.1",
     "responses~=0.25.0",
     "craft-application[remote]"
 ]
 lint = [
     "black~=24.0",
     "codespell[toml]==2.2.6",
     "yamllint==1.35.1"
 ]
 types = [
     "mypy[reports]==1.9.0",
-    "pyright==1.1.353",
+    "pyright==1.1.356",
     "types-requests",
     "types-urllib3",
 ]
 docs = [
     "furo==2024.1.29",
     "sphinx>=7.2.6,<7.3",
     "sphinx-autobuild==2024.2.4",
```

### Comparing `craft-application-2.2.0/tests/conftest.py` & `craft-application-2.3.0/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,20 +129,32 @@
             )
 
     mocker.patch.object(MyBuildPlanner, "get_build_plan", return_value=build_plan)
     return build_plan
 
 
 @pytest.fixture()
+def enable_partitions() -> Iterator[craft_parts.Features]:
+    """Enable the partitions feature in craft_parts for the relevant test."""
+    enable_overlay = craft_parts.Features().enable_overlay
+
+    craft_parts.Features.reset()
+    yield craft_parts.Features(enable_overlay=enable_overlay, enable_partitions=True)
+    craft_parts.Features.reset()
+
+
+@pytest.fixture()
 def enable_overlay() -> Iterator[craft_parts.Features]:
     """Enable the overlay feature in craft_parts for the relevant test."""
     if not os.getenv("CI") and not shutil.which("fuse-overlayfs"):
         pytest.skip("fuse-overlayfs not installed, skipping overlay tests.")
+
+    enable_partitions = craft_parts.Features().enable_partitions
     craft_parts.Features.reset()
-    yield craft_parts.Features(enable_overlay=True)
+    yield craft_parts.Features(enable_overlay=True, enable_partitions=enable_partitions)
     craft_parts.Features.reset()
 
 
 @pytest.fixture()
 def lifecycle_service(
     app_metadata, fake_project, fake_services, fake_build_plan, mocker, tmp_path
 ) -> services.LifecycleService:
```

### Comparing `craft-application-2.2.0/tests/integration/conftest.py` & `craft-application-2.3.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/integration/launchpad/conftest.py` & `craft-application-2.3.0/tests/integration/launchpad/conftest.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/integration/launchpad/test_anonymous_access.py` & `craft-application-2.3.0/tests/integration/launchpad/test_anonymous_access.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/integration/services/test_lifecycle.py` & `craft-application-2.3.0/tests/integration/services/test_lifecycle.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/integration/services/test_provider.py` & `craft-application-2.3.0/tests/integration/services/test_provider.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/integration/services/test_request.py` & `craft-application-2.3.0/tests/integration/services/test_request.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/integration/services/test_service_factory.py` & `craft-application-2.3.0/tests/integration/services/test_service_factory.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/integration/test_application.py` & `craft-application-2.3.0/tests/integration/test_application.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/integration/test_version.py` & `craft-application-2.3.0/tests/integration/test_version.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/commands/test_base.py` & `craft-application-2.3.0/tests/unit/commands/test_base.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/commands/test_lifecycle.py` & `craft-application-2.3.0/tests/unit/commands/test_lifecycle.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/commands/test_other.py` & `craft-application-2.3.0/tests/unit/commands/test_other.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/conftest.py` & `craft-application-2.3.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/launchpad/conftest.py` & `craft-application-2.3.0/tests/unit/launchpad/conftest.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/launchpad/models/test_base.py` & `craft-application-2.3.0/tests/unit/launchpad/models/test_base.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/launchpad/models/test_code.py` & `craft-application-2.3.0/tests/unit/launchpad/models/test_code.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/launchpad/test_launchpad.py` & `craft-application-2.3.0/tests/unit/launchpad/test_launchpad.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/launchpad/test_util.py` & `craft-application-2.3.0/tests/unit/launchpad/test_util.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/models/test_constraints.py` & `craft-application-2.3.0/tests/unit/models/test_constraints.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/models/test_project.py` & `craft-application-2.3.0/tests/unit/models/test_project.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/remote/conftest.py` & `craft-application-2.3.0/tests/unit/remote/conftest.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/remote/test_errors.py` & `craft-application-2.3.0/tests/unit/remote/test_errors.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/remote/test_git.py` & `craft-application-2.3.0/tests/unit/remote/test_git.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/remote/test_utils.py` & `craft-application-2.3.0/tests/unit/remote/test_utils.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/remote/test_worktree.py` & `craft-application-2.3.0/tests/unit/remote/test_worktree.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/services/conftest.py` & `craft-application-2.3.0/tests/unit/services/conftest.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/services/test_lifecycle.py` & `craft-application-2.3.0/tests/unit/services/test_lifecycle.py`

 * *Files 2% similar despite different names*

```diff
@@ -302,14 +302,34 @@
     )
     assert service._lcm is None
     service.setup()
     assert service._lcm is not None
     assert service._lcm._project_info.package_repositories == package_repositories
 
 
+@pytest.mark.usefixtures("enable_partitions")
+def test_init_with_partitions(
+    app_metadata, fake_project, fake_services, tmp_path, fake_build_plan
+):
+    service = lifecycle.LifecycleService(
+        app_metadata,
+        fake_services,
+        project=fake_project,
+        work_dir=tmp_path,
+        cache_dir=tmp_path,
+        platform=None,
+        build_plan=fake_build_plan,
+        partitions=["default", "mypartition"],
+    )
+    assert service._lcm is None
+    service.setup()
+    assert service._lcm is not None
+    assert service._lcm._project_info.partitions == ["default", "mypartition"]
+
+
 def test_prime_dir(lifecycle_service, tmp_path):
     prime_dir = lifecycle_service.prime_dir
 
     pytest_check.is_instance(prime_dir, Path)
     pytest_check.equal(prime_dir, tmp_path / "work/prime")
```

### Comparing `craft-application-2.2.0/tests/unit/services/test_package.py` & `craft-application-2.3.0/tests/unit/services/test_package.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/services/test_provider.py` & `craft-application-2.3.0/tests/unit/services/test_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,23 +286,21 @@
     emitter,
     tmp_path,
     app_metadata,
     fake_project,
     provider_service,
     base_name,
     allow_unstable,
-    mocker,
 ):
     mock_provider = mock.MagicMock(spec=craft_providers.Provider)
     monkeypatch.setattr(
         provider_service,
         "get_provider",
         lambda name: mock_provider,  # noqa: ARG005 (unused argument)
     )
-    spy_pause = mocker.spy(provider.emit, "pause")
     arch = util.get_host_architecture()
     build_info = models.BuildInfo("foo", arch, arch, base_name)
 
     with provider_service.instance(
         build_info, work_dir=tmp_path, allow_unstable=allow_unstable
     ) as instance:
         pass
@@ -322,16 +320,14 @@
         instance.push_file_io.assert_called_once_with(
             destination=pathlib.Path("/root/.bashrc"),
             content=mock.ANY,
             file_mode="644",
         )
     with check:
         emitter.assert_progress("Launching managed .+ instance...", regex=True)
-    with check:
-        assert spy_pause.call_count == 1
 
 
 def test_load_bashrc(emitter):
     """Test that we are able to load the bashrc file from the craft-application package."""
     bashrc = pkgutil.get_data("craft_application", "misc/instance_bashrc")
     assert bashrc is not None
     assert bashrc.decode("UTF-8").startswith("#!/bin/bash")
```

### Comparing `craft-application-2.2.0/tests/unit/services/test_remotebuild.py` & `craft-application-2.3.0/tests/unit/services/test_remotebuild.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/services/test_repositories.py` & `craft-application-2.3.0/tests/unit/services/test_repositories.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/services/test_request.py` & `craft-application-2.3.0/tests/unit/services/test_request.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/services/test_service_factory.py` & `craft-application-2.3.0/tests/unit/services/test_service_factory.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/test_application.py` & `craft-application-2.3.0/tests/unit/test_application.py`

 * *Files 4% similar despite different names*

```diff
@@ -233,30 +233,32 @@
     )
 
     actual = app.log_path
 
     assert actual == expected
 
 
-def test_run_managed_success(app, fake_project, fake_build_plan):
+def test_run_managed_success(mocker, app, fake_project, fake_build_plan):
     mock_provider = mock.MagicMock(spec_set=services.ProviderService)
     app.services.provider = mock_provider
     app.project = fake_project
     app._build_plan = fake_build_plan
+    mock_pause = mocker.spy(craft_cli.emit, "pause")
     arch = get_host_architecture()
 
     app.run_managed(None, arch)
 
     assert (
         mock.call(
             fake_build_plan[0],
             work_dir=mock.ANY,
         )
         in mock_provider.instance.mock_calls
     )
+    mock_pause.assert_called_once()
 
 
 def test_run_managed_failure(app, fake_project, fake_build_plan):
     mock_provider = mock.MagicMock(spec_set=services.ProviderService)
     instance = mock_provider.instance.return_value.__enter__.return_value
     instance.execute_run.side_effect = subprocess.CalledProcessError(1, [])
     app.services.provider = mock_provider
@@ -1172,7 +1174,68 @@
 
 def test_process_grammar_no_match(grammar_app, mocker):
     """Test that if the build plan is empty, the grammar uses the host as target arch."""
     mocker.patch("craft_application.util.get_host_architecture", return_value="i386")
     project = grammar_app.get_project()
     # "source" is empty because "i386" doesn't match any of the grammar statements.
     assert project.parts["mypart"]["source"] is None
+
+
+class FakePartitionsApplication(FakeApplication):
+    """A partition using FakeApplication."""
+
+    @override
+    def _setup_partitions(self, yaml_data) -> list[str]:
+        _ = yaml_data
+        return ["default", "mypartition"]
+
+
+@pytest.fixture()
+def environment_partitions_project(monkeypatch, tmp_path):
+    project_dir = tmp_path / "project"
+    project_dir.mkdir()
+    project_path = project_dir / "testcraft.yaml"
+    project_path.write_text(
+        dedent(
+            """
+        name: myproject
+        version: 1.2.3
+        parts:
+          mypart:
+            plugin: nil
+            source-tag: v$CRAFT_PROJECT_VERSION
+            override-stage: |
+              touch $CRAFT_STAGE/default
+              touch $CRAFT_MYPARTITION_STAGE/partition
+            override-prime: |
+              touch $CRAFT_PRIME/default
+              touch $CRAFT_MYPARTITION_PRIME/partition
+        """
+        )
+    )
+    monkeypatch.chdir(project_dir)
+
+    return project_path
+
+
+@pytest.mark.usefixtures("enable_partitions")
+@pytest.mark.usefixtures("environment_partitions_project")
+def test_partition_application_expand_environment(app_metadata, fake_services):
+    app = FakePartitionsApplication(app_metadata, fake_services)
+    project = app.get_project(build_for=get_host_architecture())
+
+    assert craft_parts.Features().enable_partitions is True
+    # Make sure the project is loaded correctly (from the cwd)
+    assert project is not None
+    assert project.parts["mypart"]["source-tag"] == "v1.2.3"
+    assert project.parts["mypart"]["override-stage"] == dedent(
+        f"""\
+        touch {app.project_dir}/stage/default
+        touch {app.project_dir}/partitions/mypartition/stage/partition
+    """
+    )
+    assert project.parts["mypart"]["override-prime"] == dedent(
+        f"""\
+        touch {app.project_dir}/prime/default
+        touch {app.project_dir}/partitions/mypartition/prime/partition
+    """
+    )
```

### Comparing `craft-application-2.2.0/tests/unit/test_errors.py` & `craft-application-2.3.0/tests/unit/test_errors.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/test_grammar.py` & `craft-application-2.3.0/tests/unit/test_grammar.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/test_secrets.py` & `craft-application-2.3.0/tests/unit/test_secrets.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/util/test_error_formatting.py` & `craft-application-2.3.0/tests/unit/util/test_error_formatting.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/util/test_logging.py` & `craft-application-2.3.0/tests/unit/util/test_logging.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/util/test_paths.py` & `craft-application-2.3.0/tests/unit/util/test_paths.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/util/test_snap_config.py` & `craft-application-2.3.0/tests/unit/util/test_snap_config.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/util/test_string.py` & `craft-application-2.3.0/tests/unit/util/test_string.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tests/unit/util/test_yaml.py` & `craft-application-2.3.0/tests/unit/util/test_yaml.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.2.0/tox.ini` & `craft-application-2.3.0/tox.ini`

 * *Files identical despite different names*

