# Comparing `tmp/documenteer-1.2.0.tar.gz` & `tmp/documenteer-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "documenteer-1.2.0.tar", last modified: Tue Mar 26 18:15:58 2024, max compression
+gzip compressed data, was "documenteer-1.2.1.tar", last modified: Tue Apr  2 17:09:35 2024, max compression
```

## Comparing `documenteer-1.2.0.tar` & `documenteer-1.2.1.tar`

### file list

```diff
@@ -1,307 +1,314 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.984459 documenteer-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-26 18:15:42.000000 documenteer-1.2.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.936459 documenteer-1.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-26 18:15:42.000000 documenteer-1.2.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-26 18:15:42.000000 documenteer-1.2.0/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-26 18:15:42.000000 documenteer-1.2.0/.github/SUPPORT.md
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-26 18:15:42.000000 documenteer-1.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.936459 documenteer-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-03-26 18:15:42.000000 documenteer-1.2.0/.github/workflows/ci-cron.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-03-26 18:15:42.000000 documenteer-1.2.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-26 18:15:42.000000 documenteer-1.2.0/.github/workflows/dependencies.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-26 18:15:42.000000 documenteer-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-26 18:15:42.000000 documenteer-1.2.0/.npmrc
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-26 18:15:42.000000 documenteer-1.2.0/.nvmrc
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-26 18:15:42.000000 documenteer-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-26 18:15:42.000000 documenteer-1.2.0/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-26 18:15:42.000000 documenteer-1.2.0/.prettierrc.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.936459 documenteer-1.2.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-26 18:15:42.000000 documenteer-1.2.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-26 18:15:42.000000 documenteer-1.2.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)    38113 2024-03-26 18:15:42.000000 documenteer-1.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-03-26 18:15:42.000000 documenteer-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-26 18:15:42.000000 documenteer-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-26 18:15:42.000000 documenteer-1.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-03-26 18:15:58.984459 documenteer-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-03-26 18:15:42.000000 documenteer-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.936459 documenteer-1.2.0/changelog.d/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-26 18:15:42.000000 documenteer-1.2.0/changelog.d/_template.md.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.924459 documenteer-1.2.0/demo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.940459 documenteer-1.2.0/demo/ipynb-technote/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 18:15:42.000000 documenteer-1.2.0/demo/ipynb-technote/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-26 18:15:42.000000 documenteer-1.2.0/demo/ipynb-technote/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-26 18:15:42.000000 documenteer-1.2.0/demo/ipynb-technote/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-26 18:15:42.000000 documenteer-1.2.0/demo/ipynb-technote/diagram.py
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-03-26 18:15:42.000000 documenteer-1.2.0/demo/ipynb-technote/index.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-26 18:15:42.000000 documenteer-1.2.0/demo/ipynb-technote/technote.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.940459 documenteer-1.2.0/demo/rst-technote/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 18:15:42.000000 documenteer-1.2.0/demo/rst-technote/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-26 18:15:42.000000 documenteer-1.2.0/demo/rst-technote/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-26 18:15:42.000000 documenteer-1.2.0/demo/rst-technote/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-26 18:15:42.000000 documenteer-1.2.0/demo/rst-technote/diagram.py
--rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-03-26 18:15:42.000000 documenteer-1.2.0/demo/rst-technote/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-26 18:15:42.000000 documenteer-1.2.0/demo/rst-technote/technote.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.940459 documenteer-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/_rst_epilog.rst
--rw-r--r--   0 runner    (1001) docker     (127)    38113 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.944459 documenteer-1.2.0/docs/dev/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.944459 documenteer-1.2.0/docs/dev/api/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/dev/api/documenteer.conf.rst
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/dev/api/documenteer.ext.rst
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/dev/api/documenteer.requestsutils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/dev/api/documenteer.sphinxrunner.rst
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/dev/api/documenteer.stackdocs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/dev/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/dev/development.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/dev/html-templates.rst
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/dev/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/dev/release.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/dev/theme-assets.rst
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/dev/theme.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/documenteer.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.948459 documenteer-1.2.0/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/guides/badges.rst
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/guides/configuration-preset.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/guides/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/guides/diagrams.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/guides/extend-conf-py.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/guides/including-notebooks.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/guides/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/guides/markdown-primer.md
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/guides/openapi.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/guides/organization.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/guides/overview.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.948459 documenteer-1.2.0/docs/guides/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/guides/pipelines/build-overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/guides/pipelines/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/guides/pipelines/cpp-api-linking.rst
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/guides/pipelines/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/guides/pipelines/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/guides/pipelines/package-docs-cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/guides/pipelines/stack-docs-cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/guides/pyproject-configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/guides/rst-epilog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/guides/tabsets.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11961 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/guides/toml-reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.948459 documenteer-1.2.0/docs/sphinx-extensions/
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/sphinx-extensions/autocppapi.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/sphinx-extensions/autodocreset.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/sphinx-extensions/docushare-reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/sphinx-extensions/githubbibcache.rst
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/sphinx-extensions/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/sphinx-extensions/jira-reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/sphinx-extensions/lsst-pybtex-style.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12795 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/sphinx-extensions/lssttasks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/sphinx-extensions/openapi.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/sphinx-extensions/package-toctree.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/sphinx-extensions/remote-code-block.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.952459 documenteer-1.2.0/docs/technotes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.952459 documenteer-1.2.0/docs/technotes/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/technotes/_templates/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/technotes/_templates/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/technotes/author-metadata.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/technotes/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/technotes/document-status.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/technotes/edit-locally.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/technotes/edit-on-github.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/technotes/extensions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/technotes/how-your-technote-gets-published.rst
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/technotes/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    18578 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/technotes/migrate.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-03-26 18:15:42.000000 documenteer-1.2.0/docs/technotes/start-a-technote.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.952459 documenteer-1.2.0/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-26 18:15:42.000000 documenteer-1.2.0/licenses/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-03-26 18:15:42.000000 documenteer-1.2.0/licenses/astropy-helpers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-03-26 18:15:42.000000 documenteer-1.2.0/licenses/sphinx-issue.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13362 2024-03-26 18:15:42.000000 documenteer-1.2.0/licenses/sphinx.txt
--rw-r--r--   0 runner    (1001) docker     (127)   212497 2024-03-26 18:15:51.000000 documenteer-1.2.0/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-26 18:15:42.000000 documenteer-1.2.0/package.json
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-26 18:15:42.000000 documenteer-1.2.0/postcss.config.js
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-03-26 18:15:42.000000 documenteer-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 18:15:58.984459 documenteer-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.928459 documenteer-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.928459 documenteer-1.2.0/src/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.928459 documenteer-1.2.0/src/assets/rubin-technote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.952459 documenteer-1.2.0/src/assets/rubin-technote/styles/
--rw-r--r--   0 runner    (1001) docker     (127)   137996 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/assets/rubin-technote/styles/SourceSans3VF-Italic.ttf.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   170188 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/assets/rubin-technote/styles/SourceSans3VF-Upright.ttf.woff2
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/assets/rubin-technote/styles/_hacks.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/assets/rubin-technote/styles/_properties.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.956459 documenteer-1.2.0/src/assets/rubin-technote/styles/components/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/assets/rubin-technote/styles/components/_article-header.scss
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/assets/rubin-technote/styles/components/_authors.scss
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/assets/rubin-technote/styles/components/_global-breadcrumbs.scss
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/assets/rubin-technote/styles/components/_index.scss
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/assets/rubin-technote/styles/components/_sidebar-section.scss
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/assets/rubin-technote/styles/components/_version-info.scss
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/assets/rubin-technote/styles/rubin-technote.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.956459 documenteer-1.2.0/src/documenteer/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.960459 documenteer-1.2.0/src/documenteer/assets/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/assets/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)   137996 2024-03-26 18:15:53.000000 documenteer-1.2.0/src/documenteer/assets/731c8feefe13e72a8691.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   170188 2024-03-26 18:15:53.000000 documenteer-1.2.0/src/documenteer/assets/b8bc3440ba2145e132f5.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/assets/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.960459 documenteer-1.2.0/src/documenteer/assets/rsd-assets/
--rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-03-26 18:15:53.000000 documenteer-1.2.0/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-black-crop.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-03-26 18:15:53.000000 documenteer-1.2.0/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-white-crop.svg
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/assets/rubin-favicon-transparent-32px.png
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/assets/rubin-favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/assets/rubin-pydata-theme.css
--rw-r--r--   0 runner    (1001) docker     (127)     9750 2024-03-26 18:15:53.000000 documenteer-1.2.0/src/documenteer/assets/rubin-technote.css
--rw-r--r--   0 runner    (1001) docker     (127)    11497 2024-03-26 18:15:53.000000 documenteer-1.2.0/src/documenteer/assets/rubin-technote.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/assets/rubin-titlebar-imagotype-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/assets/rubin-titlebar-imagotype-light.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.960459 documenteer-1.2.0/src/documenteer/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-03-26 18:15:53.000000 documenteer-1.2.0/src/documenteer/assets/scripts/rubin-technote.js
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-03-26 18:15:53.000000 documenteer-1.2.0/src/documenteer/assets/scripts/rubin-technote.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.960459 documenteer-1.2.0/src/documenteer/conf/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17509 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/conf/_toml.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/conf/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13892 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/conf/guide.py
--rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/conf/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/conf/pipelinespkg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/conf/technote.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.964459 documenteer-1.2.0/src/documenteer/ext/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/ext/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/ext/autocppapi.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/ext/autodocreset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/ext/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/ext/githubbibcache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/ext/jira.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/ext/lsstdocushare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.964459 documenteer-1.2.0/src/documenteer/ext/lssttasks/
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/ext/lssttasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39797 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/ext/lssttasks/configfieldlists.py
--rw-r--r--   0 runner    (1001) docker     (127)    12374 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/ext/lssttasks/crossrefs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10419 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/ext/lssttasks/pyapisummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/ext/lssttasks/taskutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/ext/lssttasks/topiclists.py
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/ext/lssttasks/topics.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/ext/mockcoderefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/ext/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7497 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/ext/packagetoctree.py
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/ext/remotecodeblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/packagemetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/requestsutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.964459 documenteer-1.2.0/src/documenteer/services/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/services/technoteauthor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/services/technotemigration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/sphinxrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.968459 documenteer-1.2.0/src/documenteer/stackdocs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/stackdocs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11975 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/stackdocs/build.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.968459 documenteer-1.2.0/src/documenteer/stackdocs/data/
--rw-r--r--   0 runner    (1001) docker     (127)  1063166 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/stackdocs/data/cppreference-doxygen-web.tag.xml
--rw-r--r--   0 runner    (1001) docker     (127)   105749 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/stackdocs/data/doxygen.defaults.conf
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/stackdocs/data/mainpage.dox
--rw-r--r--   0 runner    (1001) docker     (127)    23844 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/stackdocs/doxygen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/stackdocs/doxygentag.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/stackdocs/packagecli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9948 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/stackdocs/pkgdiscovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/stackdocs/rootdiscovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/stackdocs/stackcli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.968459 documenteer-1.2.0/src/documenteer/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/storage/authordb.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/storage/latex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.928459 documenteer-1.2.0/src/documenteer/storage/localtemplates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.972459 documenteer-1.2.0/src/documenteer/storage/localtemplates/technote/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/storage/localtemplates/technote/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/storage/localtemplates/technote/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/storage/localtemplates/technote/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/storage/localtemplates/technote/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/storage/localtemplates/technote/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/storage/localtemplates/technote/gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/storage/localtemplates/technote/pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/storage/localtemplates/technote/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/storage/localtemplates/technote/tox.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/storage/localtemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/storage/technotetoml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.928459 documenteer-1.2.0/src/documenteer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.972459 documenteer-1.2.0/src/documenteer/templates/pydata/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/templates/pydata/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.972459 documenteer-1.2.0/src/documenteer/templates/technote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/templates/technote/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.972459 documenteer-1.2.0/src/documenteer/templates/technote/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/templates/technote/components/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/templates/technote/components/sidebar-source.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.972459 documenteer-1.2.0/src/documenteer/templates/technote/sections/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/templates/technote/sections/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/templates/technote/sections/header-article.html
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/templates/technote/sections/sidebar-primary.html
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-26 18:15:42.000000 documenteer-1.2.0/src/documenteer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.980459 documenteer-1.2.0/src/documenteer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-03-26 18:15:58.000000 documenteer-1.2.0/src/documenteer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8795 2024-03-26 18:15:58.000000 documenteer-1.2.0/src/documenteer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 18:15:58.000000 documenteer-1.2.0/src/documenteer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-26 18:15:58.000000 documenteer-1.2.0/src/documenteer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-26 18:15:58.000000 documenteer-1.2.0/src/documenteer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-26 18:15:58.000000 documenteer-1.2.0/src/documenteer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.976459 documenteer-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.976459 documenteer-1.2.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/data/afw.doxygen.conf
--rw-r--r--   0 runner    (1001) docker     (127)    82475 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/data/authordb.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   199942 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/data/doxygen.tag.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.932459 documenteer-1.2.0/tests/data/package_alpha/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.976459 documenteer-1.2.0/tests/data/package_alpha/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.932459 documenteer-1.2.0/tests/data/package_alpha/doc/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.976459 documenteer-1.2.0/tests/data/package_alpha/doc/_static/package_alpha/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/data/package_alpha/doc/_static/package_alpha/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/data/package_alpha/doc/doxygen.conf.in
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/data/package_alpha/doc/manifest.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.976459 documenteer-1.2.0/tests/data/package_alpha/doc/package.alpha/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/data/package_alpha/doc/package.alpha/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.976459 documenteer-1.2.0/tests/data/package_alpha/doc/package_alpha/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/data/package_alpha/doc/package_alpha/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.976459 documenteer-1.2.0/tests/data/package_alpha/include/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/data/package_alpha/include/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.976459 documenteer-1.2.0/tests/data/package_alpha/src/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/data/package_alpha/src/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.932459 documenteer-1.2.0/tests/data/package_beta/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.976459 documenteer-1.2.0/tests/data/package_beta/doc/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/data/package_beta/doc/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.980459 documenteer-1.2.0/tests/ext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/ext/autocppapi_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/ext/jira_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/ext/lsstdocushare_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.980459 documenteer-1.2.0/tests/ext/lssttasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/ext/lssttasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/ext/lssttasks/taskutils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/ext/mockcoderefs_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/ext/packagetoctree_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/ext/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/packagemetadata_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.932459 documenteer-1.2.0/tests/roots/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.980459 documenteer-1.2.0/tests/roots/test-autocppapi/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/roots/test-autocppapi/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)   199942 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/roots/test-autocppapi/doxygen.tag.zip
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/roots/test-autocppapi/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.980459 documenteer-1.2.0/tests/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/services/technotemigration_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:58.980459 documenteer-1.2.0/tests/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/storage/authordb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/storage/technotetoml_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/test_conf_toml.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/test_conf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/test_stackdocs_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/test_stackdocs_doxygen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/test_stackdocs_doxygentag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/test_stackdocs_pkgdiscovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-03-26 18:15:42.000000 documenteer-1.2.0/tests/test_stackdocs_rootdiscovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-03-26 18:15:42.000000 documenteer-1.2.0/tox.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-03-26 18:15:42.000000 documenteer-1.2.0/webpack.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.975126 documenteer-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-02 17:09:08.000000 documenteer-1.2.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.931126 documenteer-1.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-02 17:09:08.000000 documenteer-1.2.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-02 17:09:08.000000 documenteer-1.2.1/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-02 17:09:08.000000 documenteer-1.2.1/.github/SUPPORT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-02 17:09:08.000000 documenteer-1.2.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.931126 documenteer-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-02 17:09:08.000000 documenteer-1.2.1/.github/workflows/ci-cron.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-02 17:09:08.000000 documenteer-1.2.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-02 17:09:08.000000 documenteer-1.2.1/.github/workflows/dependencies.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-02 17:09:08.000000 documenteer-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-02 17:09:08.000000 documenteer-1.2.1/.npmrc
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 17:09:08.000000 documenteer-1.2.1/.nvmrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-02 17:09:08.000000 documenteer-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-02 17:09:08.000000 documenteer-1.2.1/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-02 17:09:08.000000 documenteer-1.2.1/.prettierrc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.931126 documenteer-1.2.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-02 17:09:08.000000 documenteer-1.2.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-02 17:09:08.000000 documenteer-1.2.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)    38485 2024-04-02 17:09:08.000000 documenteer-1.2.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-02 17:09:08.000000 documenteer-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-02 17:09:08.000000 documenteer-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-02 17:09:08.000000 documenteer-1.2.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-04-02 17:09:35.975126 documenteer-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-02 17:09:08.000000 documenteer-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.931126 documenteer-1.2.1/changelog.d/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-02 17:09:08.000000 documenteer-1.2.1/changelog.d/_template.md.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.919126 documenteer-1.2.1/demo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.931126 documenteer-1.2.1/demo/ipynb-technote/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/ipynb-technote/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/ipynb-technote/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/ipynb-technote/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/ipynb-technote/diagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/ipynb-technote/index.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/ipynb-technote/technote.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.931126 documenteer-1.2.1/demo/md-technote/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/md-technote/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/md-technote/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/md-technote/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/md-technote/diagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/md-technote/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/md-technote/technote.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.935126 documenteer-1.2.1/demo/rst-technote/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/rst-technote/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/rst-technote/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/rst-technote/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/rst-technote/diagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/rst-technote/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/rst-technote/technote.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.935126 documenteer-1.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/_rst_epilog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    38485 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.935126 documenteer-1.2.1/docs/dev/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.935126 documenteer-1.2.1/docs/dev/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/dev/api/documenteer.conf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/dev/api/documenteer.ext.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/dev/api/documenteer.requestsutils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/dev/api/documenteer.sphinxrunner.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/dev/api/documenteer.stackdocs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/dev/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/dev/development.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/dev/html-templates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/dev/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/dev/release.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/dev/theme-assets.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/dev/theme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/documenteer.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.939126 documenteer-1.2.1/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/configuration-preset.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/diagrams.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/extend-conf-py.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/including-notebooks.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/markdown-primer.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/openapi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/organization.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/overview.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.939126 documenteer-1.2.1/docs/guides/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/pipelines/build-overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/pipelines/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/pipelines/cpp-api-linking.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/pipelines/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/pipelines/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/pipelines/package-docs-cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/pipelines/stack-docs-cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/pyproject-configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/rst-epilog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/tabsets.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11961 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/toml-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.943126 documenteer-1.2.1/docs/sphinx-extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/sphinx-extensions/autocppapi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/sphinx-extensions/autodocreset.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/sphinx-extensions/docushare-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/sphinx-extensions/githubbibcache.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/sphinx-extensions/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/sphinx-extensions/jira-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/sphinx-extensions/lsst-pybtex-style.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12795 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/sphinx-extensions/lssttasks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/sphinx-extensions/openapi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/sphinx-extensions/package-toctree.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/sphinx-extensions/remote-code-block.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.943126 documenteer-1.2.1/docs/technotes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.943126 documenteer-1.2.1/docs/technotes/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/technotes/_templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/technotes/_templates/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/technotes/author-metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/technotes/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/technotes/document-status.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/technotes/edit-locally.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/technotes/edit-on-github.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/technotes/extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/technotes/how-your-technote-gets-published.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/technotes/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    18578 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/technotes/migrate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/technotes/start-a-technote.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.943126 documenteer-1.2.1/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-02 17:09:08.000000 documenteer-1.2.1/licenses/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-02 17:09:08.000000 documenteer-1.2.1/licenses/astropy-helpers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-02 17:09:08.000000 documenteer-1.2.1/licenses/sphinx-issue.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13362 2024-04-02 17:09:08.000000 documenteer-1.2.1/licenses/sphinx.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   212497 2024-04-02 17:09:15.000000 documenteer-1.2.1/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-02 17:09:08.000000 documenteer-1.2.1/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 17:09:08.000000 documenteer-1.2.1/postcss.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-02 17:09:08.000000 documenteer-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 17:09:35.975126 documenteer-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.919126 documenteer-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.919126 documenteer-1.2.1/src/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.919126 documenteer-1.2.1/src/assets/rubin-technote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.947126 documenteer-1.2.1/src/assets/rubin-technote/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)   137996 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/assets/rubin-technote/styles/SourceSans3VF-Italic.ttf.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   170188 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/assets/rubin-technote/styles/SourceSans3VF-Upright.ttf.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/assets/rubin-technote/styles/_hacks.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/assets/rubin-technote/styles/_properties.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.947126 documenteer-1.2.1/src/assets/rubin-technote/styles/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/assets/rubin-technote/styles/components/_article-header.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/assets/rubin-technote/styles/components/_authors.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/assets/rubin-technote/styles/components/_global-breadcrumbs.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/assets/rubin-technote/styles/components/_index.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/assets/rubin-technote/styles/components/_sidebar-section.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/assets/rubin-technote/styles/components/_version-info.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/assets/rubin-technote/styles/rubin-technote.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.947126 documenteer-1.2.1/src/documenteer/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.951126 documenteer-1.2.1/src/documenteer/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/assets/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)   137996 2024-04-02 17:09:17.000000 documenteer-1.2.1/src/documenteer/assets/731c8feefe13e72a8691.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   170188 2024-04-02 17:09:17.000000 documenteer-1.2.1/src/documenteer/assets/b8bc3440ba2145e132f5.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/assets/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.951126 documenteer-1.2.1/src/documenteer/assets/rsd-assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-04-02 17:09:17.000000 documenteer-1.2.1/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-black-crop.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-04-02 17:09:17.000000 documenteer-1.2.1/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-white-crop.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/assets/rubin-favicon-transparent-32px.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/assets/rubin-favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/assets/rubin-pydata-theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9750 2024-04-02 17:09:17.000000 documenteer-1.2.1/src/documenteer/assets/rubin-technote.css
+-rw-r--r--   0 runner    (1001) docker     (127)    11497 2024-04-02 17:09:17.000000 documenteer-1.2.1/src/documenteer/assets/rubin-technote.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/assets/rubin-titlebar-imagotype-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/assets/rubin-titlebar-imagotype-light.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.951126 documenteer-1.2.1/src/documenteer/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-02 17:09:17.000000 documenteer-1.2.1/src/documenteer/assets/scripts/rubin-technote.js
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-02 17:09:17.000000 documenteer-1.2.1/src/documenteer/assets/scripts/rubin-technote.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.955126 documenteer-1.2.1/src/documenteer/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17509 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/conf/_toml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/conf/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13892 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/conf/guide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/conf/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/conf/pipelinespkg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/conf/technote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.955126 documenteer-1.2.1/src/documenteer/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/autocppapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/autodocreset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/githubbibcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/jira.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/lsstdocushare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.955126 documenteer-1.2.1/src/documenteer/ext/lssttasks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/lssttasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39797 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/lssttasks/configfieldlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12374 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/lssttasks/crossrefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10419 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/lssttasks/pyapisummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/lssttasks/taskutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/lssttasks/topiclists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/lssttasks/topics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/mockcoderefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7497 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/packagetoctree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/remotecodeblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/packagemetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/requestsutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.959126 documenteer-1.2.1/src/documenteer/services/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/services/technoteauthor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/services/technotemigration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/sphinxrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.959126 documenteer-1.2.1/src/documenteer/stackdocs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/stackdocs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11975 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/stackdocs/build.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.959126 documenteer-1.2.1/src/documenteer/stackdocs/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  1063166 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/stackdocs/data/cppreference-doxygen-web.tag.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   105749 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/stackdocs/data/doxygen.defaults.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/stackdocs/data/mainpage.dox
+-rw-r--r--   0 runner    (1001) docker     (127)    23844 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/stackdocs/doxygen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/stackdocs/doxygentag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/stackdocs/packagecli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9948 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/stackdocs/pkgdiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/stackdocs/rootdiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/stackdocs/stackcli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.963126 documenteer-1.2.1/src/documenteer/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/storage/authordb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/storage/latex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.923126 documenteer-1.2.1/src/documenteer/storage/localtemplates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.963126 documenteer-1.2.1/src/documenteer/storage/localtemplates/technote/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/storage/localtemplates/technote/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/storage/localtemplates/technote/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/storage/localtemplates/technote/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/storage/localtemplates/technote/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/storage/localtemplates/technote/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/storage/localtemplates/technote/gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/storage/localtemplates/technote/pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/storage/localtemplates/technote/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/storage/localtemplates/technote/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/storage/localtemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/storage/technotetoml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.923126 documenteer-1.2.1/src/documenteer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.963126 documenteer-1.2.1/src/documenteer/templates/pydata/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/templates/pydata/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.963126 documenteer-1.2.1/src/documenteer/templates/technote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/templates/technote/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.963126 documenteer-1.2.1/src/documenteer/templates/technote/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/templates/technote/components/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/templates/technote/components/sidebar-source.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.963126 documenteer-1.2.1/src/documenteer/templates/technote/sections/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/templates/technote/sections/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/templates/technote/sections/header-article.html
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/templates/technote/sections/sidebar-primary.html
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.971126 documenteer-1.2.1/src/documenteer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-04-02 17:09:35.000000 documenteer-1.2.1/src/documenteer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-04-02 17:09:35.000000 documenteer-1.2.1/src/documenteer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 17:09:35.000000 documenteer-1.2.1/src/documenteer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-02 17:09:35.000000 documenteer-1.2.1/src/documenteer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-02 17:09:35.000000 documenteer-1.2.1/src/documenteer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 17:09:35.000000 documenteer-1.2.1/src/documenteer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.967126 documenteer-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.967126 documenteer-1.2.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/data/afw.doxygen.conf
+-rw-r--r--   0 runner    (1001) docker     (127)    82475 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/data/authordb.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   199942 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/data/doxygen.tag.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.923126 documenteer-1.2.1/tests/data/package_alpha/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.967126 documenteer-1.2.1/tests/data/package_alpha/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.923126 documenteer-1.2.1/tests/data/package_alpha/doc/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.967126 documenteer-1.2.1/tests/data/package_alpha/doc/_static/package_alpha/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/data/package_alpha/doc/_static/package_alpha/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/data/package_alpha/doc/doxygen.conf.in
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/data/package_alpha/doc/manifest.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.967126 documenteer-1.2.1/tests/data/package_alpha/doc/package.alpha/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/data/package_alpha/doc/package.alpha/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.967126 documenteer-1.2.1/tests/data/package_alpha/doc/package_alpha/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/data/package_alpha/doc/package_alpha/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.967126 documenteer-1.2.1/tests/data/package_alpha/include/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/data/package_alpha/include/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.967126 documenteer-1.2.1/tests/data/package_alpha/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/data/package_alpha/src/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.923126 documenteer-1.2.1/tests/data/package_beta/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.967126 documenteer-1.2.1/tests/data/package_beta/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/data/package_beta/doc/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.967126 documenteer-1.2.1/tests/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/ext/autocppapi_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/ext/jira_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/ext/lsstdocushare_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.971126 documenteer-1.2.1/tests/ext/lssttasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/ext/lssttasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/ext/lssttasks/taskutils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/ext/mockcoderefs_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/ext/packagetoctree_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/ext/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/packagemetadata_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.923126 documenteer-1.2.1/tests/roots/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.971126 documenteer-1.2.1/tests/roots/test-autocppapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/roots/test-autocppapi/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)   199942 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/roots/test-autocppapi/doxygen.tag.zip
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/roots/test-autocppapi/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.971126 documenteer-1.2.1/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/services/technotemigration_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.971126 documenteer-1.2.1/tests/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/storage/authordb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/storage/technotetoml_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/test_conf_toml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/test_conf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/test_stackdocs_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/test_stackdocs_doxygen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/test_stackdocs_doxygentag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/test_stackdocs_pkgdiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/test_stackdocs_rootdiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-02 17:09:08.000000 documenteer-1.2.1/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-02 17:09:08.000000 documenteer-1.2.1/webpack.config.js
```

### Comparing `documenteer-1.2.0/.github/workflows/ci-cron.yaml` & `documenteer-1.2.1/.github/workflows/ci-cron.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -37,19 +37,24 @@
           NPM_PKG_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
       - name: npm install and build
         run: |
           npm install
           npm run build
 
+      - name: Install graphviz
+        run: |
+          sudo apt-get update
+          sudo apt-get install graphviz
+
       - name: Run tests in tox
         uses: lsst-sqre/run-tox@v1
         with:
           python-version: ${{ matrix.python-version }}
-          tox-envs: "lint,typing-sphinx${{ matrix.sphinx-version }},py-test-sphinx${{ matrix.sphinx-version }}"
+          tox-envs: "lint,typing-sphinx${{ matrix.sphinx-version }},py-test-sphinx${{ matrix.sphinx-version }},demo"
           use-cache: false
 
   docs:
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v4
```

### Comparing `documenteer-1.2.0/.github/workflows/ci.yaml` & `documenteer-1.2.1/.github/workflows/ci.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -57,19 +57,24 @@
           NPM_PKG_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
       - name: npm install and build
         run: |
           npm install
           npm run build
 
+      - name: Install graphviz
+        run: |
+          sudo apt-get update
+          sudo apt-get install graphviz
+
       - name: Run tox
         uses: lsst-sqre/run-tox@v1
         with:
           python-version: ${{ matrix.python-version }}
-          tox-envs: 'py-test-sphinx${{ matrix.sphinx-version }},typing-sphinx${{ matrix.sphinx-version }}'
+          tox-envs: 'py-test-sphinx${{ matrix.sphinx-version }},typing-sphinx${{ matrix.sphinx-version }},demo'
 
   docs:
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
         with:
```

### Comparing `documenteer-1.2.0/.github/workflows/dependencies.yaml` & `documenteer-1.2.1/.github/workflows/dependencies.yaml`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/.gitignore` & `documenteer-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/.pre-commit-config.yaml` & `documenteer-1.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/.vscode/tasks.json` & `documenteer-1.2.1/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/CHANGELOG.md` & `documenteer-1.2.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Change Log
 
 <!-- scriv-insert-here -->
 
+<a id='changelog-1.2.1'></a>
+## 1.2.1 (2024-04-02)
+
+### Bug fixes
+
+- Fix the "Source parser for markdown not registered" error for Markdown-based technotes. With the MyST-NB extension the Markdown parser is automatically registered, so the `documenteer.conf.technote` configuration now resets the `source_suffix` configuration originally created by the Technote package.
+
 <a id='changelog-1.2.0'></a>
 ## 1.2.0 (2024-03-26)
 
 ### New features
 
 - Rubin user guides (`documenteer.conf.guide`) and technotes (`documenteer.conf.technote`) now include [MyST-NB](https://myst-nb.readthedocs.io/en/latest/) to support Jupyter Notebooks in Sphinx documentation. The MyST-NB extension also supersedes MyST-Parser for Markdown syntax support. For guides, Jupyter Notebook files can be intermixed with Markdown (`.md`) and reStructuredText (`.rst`) files. An `ipynb` file is considered as a page in the documentation. For technotes, the Jupyter Notebook must be named `index.ipynb`. By default, these configurations use MyST-NB's "auto" mode for notebook execution: only if a notebook is missing outputs will it be executed.
```

### Comparing `documenteer-1.2.0/LICENSE` & `documenteer-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/PKG-INFO` & `documenteer-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: documenteer
-Version: 1.2.0
+Version: 1.2.1
 Summary: Rubin Observatory / LSST Sphinx documentation tools, extensions, and configurations.
 License: The MIT License (MIT)
         
         Copyright (c) 2015-2022 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `documenteer-1.2.0/README.md` & `documenteer-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/demo/ipynb-technote/index.ipynb` & `documenteer-1.2.1/demo/ipynb-technote/index.ipynb`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/demo/ipynb-technote/technote.toml` & `documenteer-1.2.1/demo/ipynb-technote/technote.toml`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/demo/rst-technote/index.rst` & `documenteer-1.2.1/demo/rst-technote/index.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/demo/rst-technote/technote.toml` & `documenteer-1.2.1/demo/md-technote/technote.toml`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/Makefile` & `documenteer-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/_rst_epilog.rst` & `documenteer-1.2.1/docs/_rst_epilog.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/changelog.md` & `documenteer-1.2.1/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Change Log
 
 <!-- scriv-insert-here -->
 
+<a id='changelog-1.2.1'></a>
+## 1.2.1 (2024-04-02)
+
+### Bug fixes
+
+- Fix the "Source parser for markdown not registered" error for Markdown-based technotes. With the MyST-NB extension the Markdown parser is automatically registered, so the `documenteer.conf.technote` configuration now resets the `source_suffix` configuration originally created by the Technote package.
+
 <a id='changelog-1.2.0'></a>
 ## 1.2.0 (2024-03-26)
 
 ### New features
 
 - Rubin user guides (`documenteer.conf.guide`) and technotes (`documenteer.conf.technote`) now include [MyST-NB](https://myst-nb.readthedocs.io/en/latest/) to support Jupyter Notebooks in Sphinx documentation. The MyST-NB extension also supersedes MyST-Parser for Markdown syntax support. For guides, Jupyter Notebook files can be intermixed with Markdown (`.md`) and reStructuredText (`.rst`) files. An `ipynb` file is considered as a page in the documentation. For technotes, the Jupyter Notebook must be named `index.ipynb`. By default, these configurations use MyST-NB's "auto" mode for notebook execution: only if a notebook is missing outputs will it be executed.
```

### Comparing `documenteer-1.2.0/docs/conf.py` & `documenteer-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/dev/api/documenteer.ext.rst` & `documenteer-1.2.1/docs/dev/api/documenteer.ext.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/dev/api/documenteer.stackdocs.rst` & `documenteer-1.2.1/docs/dev/api/documenteer.stackdocs.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/dev/development.rst` & `documenteer-1.2.1/docs/dev/development.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/dev/html-templates.rst` & `documenteer-1.2.1/docs/dev/html-templates.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/dev/release.rst` & `documenteer-1.2.1/docs/dev/release.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/dev/theme-assets.rst` & `documenteer-1.2.1/docs/dev/theme-assets.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/documenteer.toml` & `documenteer-1.2.1/docs/documenteer.toml`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/guides/badges.rst` & `documenteer-1.2.1/docs/guides/badges.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/guides/configuration.rst` & `documenteer-1.2.1/docs/guides/configuration.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/guides/diagrams.rst` & `documenteer-1.2.1/docs/guides/diagrams.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/guides/extend-conf-py.rst` & `documenteer-1.2.1/docs/guides/extend-conf-py.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/guides/including-notebooks.ipynb` & `documenteer-1.2.1/docs/guides/including-notebooks.ipynb`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/guides/index.rst` & `documenteer-1.2.1/docs/guides/index.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/guides/markdown-primer.md` & `documenteer-1.2.1/docs/guides/markdown-primer.md`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/guides/openapi.rst` & `documenteer-1.2.1/docs/guides/openapi.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/guides/organization.rst` & `documenteer-1.2.1/docs/guides/organization.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/guides/overview.rst` & `documenteer-1.2.1/docs/guides/overview.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/guides/pipelines/build-overview.rst` & `documenteer-1.2.1/docs/guides/pipelines/build-overview.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/guides/pipelines/configuration.rst` & `documenteer-1.2.1/docs/guides/pipelines/configuration.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/guides/pipelines/cpp-api-linking.rst` & `documenteer-1.2.1/docs/guides/pipelines/cpp-api-linking.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/guides/pipelines/index.rst` & `documenteer-1.2.1/docs/guides/pipelines/index.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/guides/pipelines/install.rst` & `documenteer-1.2.1/docs/guides/pipelines/install.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/guides/pipelines/package-docs-cli.rst` & `documenteer-1.2.1/docs/guides/pipelines/package-docs-cli.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/guides/pipelines/stack-docs-cli.rst` & `documenteer-1.2.1/docs/guides/pipelines/stack-docs-cli.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/guides/pyproject-configuration.rst` & `documenteer-1.2.1/docs/guides/pyproject-configuration.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/guides/rst-epilog.rst` & `documenteer-1.2.1/docs/guides/rst-epilog.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/guides/tabsets.rst` & `documenteer-1.2.1/docs/guides/tabsets.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/guides/toml-reference.rst` & `documenteer-1.2.1/docs/guides/toml-reference.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/index.rst` & `documenteer-1.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/sphinx-extensions/autocppapi.rst` & `documenteer-1.2.1/docs/sphinx-extensions/autocppapi.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/sphinx-extensions/autodocreset.rst` & `documenteer-1.2.1/docs/sphinx-extensions/autodocreset.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/sphinx-extensions/docushare-reference.rst` & `documenteer-1.2.1/docs/sphinx-extensions/docushare-reference.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/sphinx-extensions/githubbibcache.rst` & `documenteer-1.2.1/docs/sphinx-extensions/githubbibcache.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/sphinx-extensions/jira-reference.rst` & `documenteer-1.2.1/docs/sphinx-extensions/jira-reference.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/sphinx-extensions/lsst-pybtex-style.rst` & `documenteer-1.2.1/docs/sphinx-extensions/lsst-pybtex-style.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/sphinx-extensions/lssttasks.rst` & `documenteer-1.2.1/docs/sphinx-extensions/lssttasks.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/sphinx-extensions/openapi.rst` & `documenteer-1.2.1/docs/sphinx-extensions/openapi.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/sphinx-extensions/package-toctree.rst` & `documenteer-1.2.1/docs/sphinx-extensions/package-toctree.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/sphinx-extensions/remote-code-block.rst` & `documenteer-1.2.1/docs/sphinx-extensions/remote-code-block.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/technotes/_templates/README.md` & `documenteer-1.2.1/docs/technotes/_templates/README.md`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/technotes/_templates/README.rst` & `documenteer-1.2.1/docs/technotes/_templates/README.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/technotes/author-metadata.rst` & `documenteer-1.2.1/docs/technotes/author-metadata.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/technotes/configuration.rst` & `documenteer-1.2.1/docs/technotes/configuration.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/technotes/document-status.rst` & `documenteer-1.2.1/docs/technotes/document-status.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/technotes/edit-locally.rst` & `documenteer-1.2.1/docs/technotes/edit-locally.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/technotes/edit-on-github.rst` & `documenteer-1.2.1/docs/technotes/edit-on-github.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/technotes/extensions.rst` & `documenteer-1.2.1/docs/technotes/extensions.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/technotes/how-your-technote-gets-published.rst` & `documenteer-1.2.1/docs/technotes/how-your-technote-gets-published.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/technotes/index.rst` & `documenteer-1.2.1/docs/technotes/index.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/technotes/migrate.rst` & `documenteer-1.2.1/docs/technotes/migrate.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/docs/technotes/start-a-technote.rst` & `documenteer-1.2.1/docs/technotes/start-a-technote.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/licenses/astropy-helpers.txt` & `documenteer-1.2.1/licenses/astropy-helpers.txt`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/licenses/sphinx-issue.txt` & `documenteer-1.2.1/licenses/sphinx-issue.txt`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/licenses/sphinx.txt` & `documenteer-1.2.1/licenses/sphinx.txt`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/package-lock.json` & `documenteer-1.2.1/package-lock.json`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/package.json` & `documenteer-1.2.1/package.json`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/pyproject.toml` & `documenteer-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/assets/rubin-technote/styles/SourceSans3VF-Italic.ttf.woff2` & `documenteer-1.2.1/src/assets/rubin-technote/styles/SourceSans3VF-Italic.ttf.woff2`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/assets/rubin-technote/styles/SourceSans3VF-Upright.ttf.woff2` & `documenteer-1.2.1/src/assets/rubin-technote/styles/SourceSans3VF-Upright.ttf.woff2`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/assets/rubin-technote/styles/_hacks.scss` & `documenteer-1.2.1/src/assets/rubin-technote/styles/_hacks.scss`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/assets/rubin-technote/styles/_properties.scss` & `documenteer-1.2.1/src/assets/rubin-technote/styles/_properties.scss`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/assets/731c8feefe13e72a8691.woff2` & `documenteer-1.2.1/src/documenteer/assets/731c8feefe13e72a8691.woff2`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/assets/b8bc3440ba2145e132f5.woff2` & `documenteer-1.2.1/src/documenteer/assets/b8bc3440ba2145e132f5.woff2`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/assets/favicon.ico` & `documenteer-1.2.1/src/documenteer/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-black-crop.svg` & `documenteer-1.2.1/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-black-crop.svg`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-white-crop.svg` & `documenteer-1.2.1/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-white-crop.svg`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/assets/rubin-favicon-transparent-32px.png` & `documenteer-1.2.1/src/documenteer/assets/rubin-favicon-transparent-32px.png`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/assets/rubin-favicon.svg` & `documenteer-1.2.1/src/documenteer/assets/rubin-favicon.svg`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/assets/rubin-pydata-theme.css` & `documenteer-1.2.1/src/documenteer/assets/rubin-pydata-theme.css`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/assets/rubin-technote.css` & `documenteer-1.2.1/src/documenteer/assets/rubin-technote.css`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/assets/rubin-technote.css.map` & `documenteer-1.2.1/src/documenteer/assets/rubin-technote.css.map`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/assets/rubin-titlebar-imagotype-dark.svg` & `documenteer-1.2.1/src/documenteer/assets/rubin-titlebar-imagotype-dark.svg`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/assets/rubin-titlebar-imagotype-light.svg` & `documenteer-1.2.1/src/documenteer/assets/rubin-titlebar-imagotype-light.svg`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/assets/scripts/rubin-technote.js` & `documenteer-1.2.1/src/documenteer/assets/scripts/rubin-technote.js`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/assets/scripts/rubin-technote.js.map` & `documenteer-1.2.1/src/documenteer/assets/scripts/rubin-technote.js.map`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/cli.py` & `documenteer-1.2.1/src/documenteer/cli.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/conf/_toml.py` & `documenteer-1.2.1/src/documenteer/conf/_toml.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/conf/_utils.py` & `documenteer-1.2.1/src/documenteer/conf/_utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/conf/guide.py` & `documenteer-1.2.1/src/documenteer/conf/guide.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/conf/pipelines.py` & `documenteer-1.2.1/src/documenteer/conf/pipelines.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/conf/pipelinespkg.py` & `documenteer-1.2.1/src/documenteer/conf/pipelinespkg.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/conf/technote.py` & `documenteer-1.2.1/src/documenteer/conf/technote.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,20 @@
         "sphinx_diagrams",
         "sphinxcontrib.mermaid",
         "sphinx_prompt",
         "sphinx_design",
     ]
 )
 
+# The source file suffixes for .md and .ipynb are automatically managed by
+# myst-nb.
+source_suffix = {
+    ".rst": "restructuredtext",
+}
+
 html_static_path: list[str] = [
     get_asset_path("rubin-favicon-transparent-32px.png"),
     get_asset_path("rubin-favicon.svg"),
     get_asset_path("rubin-technote.css"),
     get_asset_path("rubin-technote.css.map"),
     get_asset_path("rsd-assets/rubin-imagotype-color-on-white-crop.svg"),
     get_asset_path("rsd-assets/rubin-imagotype-color-on-black-crop.svg"),
```

### Comparing `documenteer-1.2.0/src/documenteer/ext/_utils.py` & `documenteer-1.2.1/src/documenteer/ext/_utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/ext/autocppapi.py` & `documenteer-1.2.1/src/documenteer/ext/autocppapi.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/ext/autodocreset.py` & `documenteer-1.2.1/src/documenteer/ext/autodocreset.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/ext/bibtex.py` & `documenteer-1.2.1/src/documenteer/ext/bibtex.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/ext/githubbibcache.py` & `documenteer-1.2.1/src/documenteer/ext/githubbibcache.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/ext/jira.py` & `documenteer-1.2.1/src/documenteer/ext/jira.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/ext/lsstdocushare.py` & `documenteer-1.2.1/src/documenteer/ext/lsstdocushare.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/ext/lssttasks/__init__.py` & `documenteer-1.2.1/src/documenteer/ext/lssttasks/__init__.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/ext/lssttasks/configfieldlists.py` & `documenteer-1.2.1/src/documenteer/ext/lssttasks/configfieldlists.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/ext/lssttasks/crossrefs.py` & `documenteer-1.2.1/src/documenteer/ext/lssttasks/crossrefs.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/ext/lssttasks/pyapisummary.py` & `documenteer-1.2.1/src/documenteer/ext/lssttasks/pyapisummary.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/ext/lssttasks/taskutils.py` & `documenteer-1.2.1/src/documenteer/ext/lssttasks/taskutils.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/ext/lssttasks/topiclists.py` & `documenteer-1.2.1/src/documenteer/ext/lssttasks/topiclists.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/ext/lssttasks/topics.py` & `documenteer-1.2.1/src/documenteer/ext/lssttasks/topics.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/ext/mockcoderefs.py` & `documenteer-1.2.1/src/documenteer/ext/mockcoderefs.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/ext/openapi.py` & `documenteer-1.2.1/src/documenteer/ext/openapi.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/ext/packagetoctree.py` & `documenteer-1.2.1/src/documenteer/ext/packagetoctree.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/ext/remotecodeblock.py` & `documenteer-1.2.1/src/documenteer/ext/remotecodeblock.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/packagemetadata.py` & `documenteer-1.2.1/src/documenteer/packagemetadata.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/requestsutils.py` & `documenteer-1.2.1/src/documenteer/requestsutils.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/services/technoteauthor.py` & `documenteer-1.2.1/src/documenteer/services/technoteauthor.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/services/technotemigration.py` & `documenteer-1.2.1/src/documenteer/services/technotemigration.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/sphinxrunner.py` & `documenteer-1.2.1/src/documenteer/sphinxrunner.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/stackdocs/build.py` & `documenteer-1.2.1/src/documenteer/stackdocs/build.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/stackdocs/data/cppreference-doxygen-web.tag.xml` & `documenteer-1.2.1/src/documenteer/stackdocs/data/cppreference-doxygen-web.tag.xml`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/stackdocs/data/doxygen.defaults.conf` & `documenteer-1.2.1/src/documenteer/stackdocs/data/doxygen.defaults.conf`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/stackdocs/doxygen.py` & `documenteer-1.2.1/src/documenteer/stackdocs/doxygen.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/stackdocs/doxygentag.py` & `documenteer-1.2.1/src/documenteer/stackdocs/doxygentag.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/stackdocs/packagecli.py` & `documenteer-1.2.1/src/documenteer/stackdocs/packagecli.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/stackdocs/pkgdiscovery.py` & `documenteer-1.2.1/src/documenteer/stackdocs/pkgdiscovery.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/stackdocs/rootdiscovery.py` & `documenteer-1.2.1/src/documenteer/stackdocs/rootdiscovery.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/stackdocs/stackcli.py` & `documenteer-1.2.1/src/documenteer/stackdocs/stackcli.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/storage/authordb.py` & `documenteer-1.2.1/src/documenteer/storage/authordb.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/storage/latex.py` & `documenteer-1.2.1/src/documenteer/storage/latex.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/storage/localtemplates/technote/README.rst` & `documenteer-1.2.1/src/documenteer/storage/localtemplates/technote/README.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/storage/localtemplates/technote/tox.ini` & `documenteer-1.2.1/src/documenteer/storage/localtemplates/technote/tox.ini`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/storage/localtemplates.py` & `documenteer-1.2.1/src/documenteer/storage/localtemplates.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/storage/technotetoml.py` & `documenteer-1.2.1/src/documenteer/storage/technotetoml.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/templates/technote/components/sidebar-source.html` & `documenteer-1.2.1/src/documenteer/templates/technote/components/sidebar-source.html`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/templates/technote/sections/header-article.html` & `documenteer-1.2.1/src/documenteer/templates/technote/sections/header-article.html`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer/utils.py` & `documenteer-1.2.1/src/documenteer/utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/src/documenteer.egg-info/PKG-INFO` & `documenteer-1.2.1/src/documenteer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: documenteer
-Version: 1.2.0
+Version: 1.2.1
 Summary: Rubin Observatory / LSST Sphinx documentation tools, extensions, and configurations.
 License: The MIT License (MIT)
         
         Copyright (c) 2015-2022 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `documenteer-1.2.0/src/documenteer.egg-info/SOURCES.txt` & `documenteer-1.2.1/src/documenteer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,20 @@
 changelog.d/_template.md.jinja
 demo/ipynb-technote/.gitignore
 demo/ipynb-technote/Makefile
 demo/ipynb-technote/conf.py
 demo/ipynb-technote/diagram.py
 demo/ipynb-technote/index.ipynb
 demo/ipynb-technote/technote.toml
+demo/md-technote/.gitignore
+demo/md-technote/Makefile
+demo/md-technote/conf.py
+demo/md-technote/diagram.py
+demo/md-technote/index.md
+demo/md-technote/technote.toml
 demo/rst-technote/.gitignore
 demo/rst-technote/Makefile
 demo/rst-technote/conf.py
 demo/rst-technote/diagram.py
 demo/rst-technote/index.rst
 demo/rst-technote/technote.toml
 docs/.gitignore
```

### Comparing `documenteer-1.2.0/src/documenteer.egg-info/requires.txt` & `documenteer-1.2.1/src/documenteer.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/tests/conftest.py` & `documenteer-1.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/tests/data/afw.doxygen.conf` & `documenteer-1.2.1/tests/data/afw.doxygen.conf`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/tests/data/authordb.yaml` & `documenteer-1.2.1/tests/data/authordb.yaml`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/tests/data/doxygen.tag.zip` & `documenteer-1.2.1/tests/data/doxygen.tag.zip`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/tests/ext/autocppapi_test.py` & `documenteer-1.2.1/tests/ext/autocppapi_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/tests/ext/jira_test.py` & `documenteer-1.2.1/tests/ext/jira_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/tests/ext/lsstdocushare_test.py` & `documenteer-1.2.1/tests/ext/lsstdocushare_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/tests/ext/lssttasks/taskutils_test.py` & `documenteer-1.2.1/tests/ext/lssttasks/taskutils_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/tests/ext/mockcoderefs_test.py` & `documenteer-1.2.1/tests/ext/mockcoderefs_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/tests/ext/packagetoctree_test.py` & `documenteer-1.2.1/tests/ext/packagetoctree_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/tests/ext/utils_test.py` & `documenteer-1.2.1/tests/ext/utils_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/tests/packagemetadata_test.py` & `documenteer-1.2.1/tests/packagemetadata_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/tests/roots/test-autocppapi/conf.py` & `documenteer-1.2.1/tests/roots/test-autocppapi/conf.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/tests/roots/test-autocppapi/doxygen.tag.zip` & `documenteer-1.2.1/tests/roots/test-autocppapi/doxygen.tag.zip`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/tests/services/technotemigration_test.py` & `documenteer-1.2.1/tests/services/technotemigration_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/tests/storage/authordb_test.py` & `documenteer-1.2.1/tests/storage/authordb_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/tests/storage/technotetoml_test.py` & `documenteer-1.2.1/tests/storage/technotetoml_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/tests/test_conf_toml.py` & `documenteer-1.2.1/tests/test_conf_toml.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/tests/test_conf_utils.py` & `documenteer-1.2.1/tests/test_conf_utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/tests/test_stackdocs_build.py` & `documenteer-1.2.1/tests/test_stackdocs_build.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/tests/test_stackdocs_doxygen.py` & `documenteer-1.2.1/tests/test_stackdocs_doxygen.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/tests/test_stackdocs_doxygentag.py` & `documenteer-1.2.1/tests/test_stackdocs_doxygentag.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/tests/test_stackdocs_pkgdiscovery.py` & `documenteer-1.2.1/tests/test_stackdocs_pkgdiscovery.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/tests/test_stackdocs_rootdiscovery.py` & `documenteer-1.2.1/tests/test_stackdocs_rootdiscovery.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.0/tox.ini` & `documenteer-1.2.1/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -80,9 +80,11 @@
 [testenv:demo]
 description = Build demo projects.
 allowlist_externals =
     rm
 commands =
     rm -rf demo/rst-technote/_build
     sphinx-build --keep-going -n -W -T -b html -d {envtmpdir}/doctrees demo/rst-technote demo/rst-technote/_build/html
+    rm -rf demo/md-technote/_build
+    sphinx-build --keep-going -n -W -T -b html -d {envtmpdir}/doctrees demo/md-technote demo/md-technote/_build/html
     rm -rf demo/ipynb-technote/_build
     sphinx-build --keep-going -n -W -T -b html -d {envtmpdir}/doctrees demo/ipynb-technote demo/ipynb-technote/_build/html
```

### Comparing `documenteer-1.2.0/webpack.config.js` & `documenteer-1.2.1/webpack.config.js`

 * *Files identical despite different names*

