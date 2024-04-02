# Comparing `tmp/hardpy-0.1.0.tar.gz` & `tmp/hardpy-0.2.0.tar.gz`

## Comparing `hardpy-0.1.0.tar` & `hardpy-0.2.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/__init__.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/api.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/runner.py
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/asset-manifest.json
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/favicon.ico
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/index.html
--rw-r--r--   0        0        0    34188 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/logo512.png
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/manifest.json
--rw-r--r--   0        0        0   318244 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/css/main.e8a862f1.css
--rw-r--r--   0        0        0   512750 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/css/main.e8a862f1.css.map
--rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/js/808.ce070002.chunk.js
--rw-r--r--   0        0        0    16938 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/js/808.ce070002.chunk.js.map
--rw-r--r--   0        0        0   248230 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-16px-paths.d605910e.chunk.js
--rw-r--r--   0        0        0   303052 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-16px-paths.d605910e.chunk.js.map
--rw-r--r--   0        0        0   256588 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-20px-paths.7ee05cc8.chunk.js
--rw-r--r--   0        0        0   311540 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-20px-paths.7ee05cc8.chunk.js.map
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-all-paths-loader.0aa89747.chunk.js
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-all-paths-loader.0aa89747.chunk.js.map
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-all-paths.f63155c9.chunk.js
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-all-paths.f63155c9.chunk.js.map
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-split-paths-by-size-loader.52a072d3.chunk.js
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-split-paths-by-size-loader.52a072d3.chunk.js.map
--rw-r--r--   0        0        0   982299 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/js/main.8ef63e9b.js
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/js/main.8ef63e9b.js.LICENSE.txt
--rw-r--r--   0        0        0  4943986 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/js/main.8ef63e9b.js.map
--rw-r--r--   0        0        0   117628 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-16.520846c6beb41df528c8.eot
--rw-r--r--   0        0        0   509417 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-16.5c52b39c697f2323ce8b.svg
--rw-r--r--   0        0        0    53344 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-16.84db1772f4bfb529f64f.woff
--rw-r--r--   0        0        0    41612 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-16.b67ee1736e20e37a3225.woff2
--rw-r--r--   0        0        0   117420 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-16.e02ecf515378db143652.ttf
--rw-r--r--   0        0        0   120472 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-20.429cacb8accf72488451.ttf
--rw-r--r--   0        0        0   546938 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-20.6ae3791ee2d86fc228a6.svg
--rw-r--r--   0        0        0    42808 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-20.8cecf62de42997e4d82f.woff2
--rw-r--r--   0        0        0   120680 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-20.afbadb627d43b7857223.eot
--rw-r--r--   0        0        0    55356 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-20.e857f5a5132b8bfa71a1.woff
--rw-r--r--   0        0        0    14485 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/media/logo_smol.5b16f92447a4a9e80331.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/pytest_hardpy/__init__.py
--rw-r--r--   0        0        0     8092 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/pytest_hardpy/plugin.py
--rw-r--r--   0        0        0     5910 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/pytest_hardpy/pytest_call.py
--rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/pytest_hardpy/pytest_wrapper.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/pytest_hardpy/db/__init__.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/pytest_hardpy/db/base_connector.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/pytest_hardpy/db/base_server.py
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/pytest_hardpy/db/base_store.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/pytest_hardpy/db/const.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/pytest_hardpy/db/runstore.py
--rw-r--r--   0        0        0     6859 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/pytest_hardpy/db/schema.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/pytest_hardpy/db/statestore.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/pytest_hardpy/reporter/__init__.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/pytest_hardpy/reporter/base.py
--rw-r--r--   0        0        0    10181 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/pytest_hardpy/reporter/hook_reporter.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/pytest_hardpy/reporter/runner_reporter.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/pytest_hardpy/result/__init__.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/pytest_hardpy/result/couchdb_config.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/pytest_hardpy/result/report_loader/__init__.py
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/pytest_hardpy/result/report_loader/couchdb_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/pytest_hardpy/result/report_reader/__init__.py
--rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/pytest_hardpy/result/report_reader/couchdb_reader.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/pytest_hardpy/utils/__init__.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/pytest_hardpy/utils/config_data.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/pytest_hardpy/utils/const.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/pytest_hardpy/utils/exception.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/pytest_hardpy/utils/node_info.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/pytest_hardpy/utils/progress_calculator.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 hardpy-0.1.0/hardpy/pytest_hardpy/utils/singleton.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hardpy-0.1.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 hardpy-0.1.0/LICENSE
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 hardpy-0.1.0/README.md
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 hardpy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 hardpy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/__init__.py
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/api.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/runner.py
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/asset-manifest.json
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/favicon.ico
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/index.html
+-rw-r--r--   0        0        0    34188 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/logo512.png
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/manifest.json
+-rw-r--r--   0        0        0   318244 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/css/main.e8a862f1.css
+-rw-r--r--   0        0        0   512750 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/css/main.e8a862f1.css.map
+-rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/js/808.ce070002.chunk.js
+-rw-r--r--   0        0        0    16938 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/js/808.ce070002.chunk.js.map
+-rw-r--r--   0        0        0   248230 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-16px-paths.d605910e.chunk.js
+-rw-r--r--   0        0        0   303052 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-16px-paths.d605910e.chunk.js.map
+-rw-r--r--   0        0        0   256588 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-20px-paths.7ee05cc8.chunk.js
+-rw-r--r--   0        0        0   311540 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-20px-paths.7ee05cc8.chunk.js.map
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-all-paths-loader.0aa89747.chunk.js
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-all-paths-loader.0aa89747.chunk.js.map
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-all-paths.f63155c9.chunk.js
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-all-paths.f63155c9.chunk.js.map
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-split-paths-by-size-loader.52a072d3.chunk.js
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-split-paths-by-size-loader.52a072d3.chunk.js.map
+-rw-r--r--   0        0        0   982299 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/js/main.8ef63e9b.js
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/js/main.8ef63e9b.js.LICENSE.txt
+-rw-r--r--   0        0        0  4943986 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/js/main.8ef63e9b.js.map
+-rw-r--r--   0        0        0   117628 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-16.520846c6beb41df528c8.eot
+-rw-r--r--   0        0        0   509417 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-16.5c52b39c697f2323ce8b.svg
+-rw-r--r--   0        0        0    53344 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-16.84db1772f4bfb529f64f.woff
+-rw-r--r--   0        0        0    41612 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-16.b67ee1736e20e37a3225.woff2
+-rw-r--r--   0        0        0   117420 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-16.e02ecf515378db143652.ttf
+-rw-r--r--   0        0        0   120472 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-20.429cacb8accf72488451.ttf
+-rw-r--r--   0        0        0   546938 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-20.6ae3791ee2d86fc228a6.svg
+-rw-r--r--   0        0        0    42808 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-20.8cecf62de42997e4d82f.woff2
+-rw-r--r--   0        0        0   120680 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-20.afbadb627d43b7857223.eot
+-rw-r--r--   0        0        0    55356 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-20.e857f5a5132b8bfa71a1.woff
+-rw-r--r--   0        0        0    14485 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/media/logo_smol.5b16f92447a4a9e80331.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/pytest_hardpy/__init__.py
+-rw-r--r--   0        0        0     8415 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/pytest_hardpy/plugin.py
+-rw-r--r--   0        0        0     5910 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/pytest_hardpy/pytest_call.py
+-rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/pytest_hardpy/pytest_wrapper.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/pytest_hardpy/db/__init__.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/pytest_hardpy/db/base_connector.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/pytest_hardpy/db/base_server.py
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/pytest_hardpy/db/base_store.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/pytest_hardpy/db/const.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/pytest_hardpy/db/runstore.py
+-rw-r--r--   0        0        0     6859 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/pytest_hardpy/db/schema.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/pytest_hardpy/db/statestore.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/pytest_hardpy/reporter/__init__.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/pytest_hardpy/reporter/base.py
+-rw-r--r--   0        0        0    10181 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/pytest_hardpy/reporter/hook_reporter.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/pytest_hardpy/reporter/runner_reporter.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/pytest_hardpy/result/__init__.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/pytest_hardpy/result/couchdb_config.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/pytest_hardpy/result/report_loader/__init__.py
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/pytest_hardpy/result/report_loader/couchdb_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/pytest_hardpy/result/report_reader/__init__.py
+-rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/pytest_hardpy/result/report_reader/couchdb_reader.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/pytest_hardpy/utils/__init__.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/pytest_hardpy/utils/config_data.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/pytest_hardpy/utils/const.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/pytest_hardpy/utils/exception.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/pytest_hardpy/utils/node_info.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/pytest_hardpy/utils/progress_calculator.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 hardpy-0.2.0/hardpy/pytest_hardpy/utils/singleton.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hardpy-0.2.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 hardpy-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 hardpy-0.2.0/README.md
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 hardpy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 hardpy-0.2.0/PKG-INFO
```

### Comparing `hardpy-0.1.0/hardpy/__init__.py` & `hardpy-0.2.0/hardpy/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Copyright (c) 2024 Everypin
 # GNU General Public License v3.0 (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
-from hardpy.pytest_hardpy.plugin import HardpyPlugin
 from hardpy.pytest_hardpy.result import CouchdbLoader
 from hardpy.pytest_hardpy.utils import DuplicateSerialNumberError
 from hardpy.pytest_hardpy.result.couchdb_config import CouchdbConfig
 from hardpy.pytest_hardpy.pytest_call import (
     get_current_report,
     set_dut_info,
     set_dut_serial_number,
@@ -14,15 +13,14 @@
     set_module_artifact,
     set_run_artifact,
     set_message,
     set_driver_info,
 )
 
 __all__ = [
-    "HardpyPlugin",
     "CouchdbLoader",
     "CouchdbConfig",
     "DuplicateSerialNumberError",
     "get_current_report",
     "set_dut_info",
     "set_dut_serial_number",
     "set_stand_info",
```

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/api.py` & `hardpy-0.2.0/hardpy/hardpy_panel/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,10 +62,10 @@
     return {
         "connection_str": config_data.connection_string,
     }
 
 
 app.mount(
     "/",
-    StaticFiles(directory=(os.path.dirname(__file__))+'/frontend/dist', html=True),
+    StaticFiles(directory=(os.path.dirname(__file__)) + "/frontend/dist", html=True),
     name="static",
 )
```

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/runner.py` & `hardpy-0.2.0/hardpy/hardpy_panel/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 def run():
     """Start server for frontend."""
     config = ConfigData()
     parser = ArgumentParser(description="Usage: hardpy-panel [OPTION]... [PATH]")
     # fmt: off
-    parser.add_argument("-dbu", "--db_user", default=config.db_user, help="database user")
+    parser.add_argument("-dbu", "--db_user", default=config.db_user, help="database user")  # noqa: E501
     parser.add_argument("-dbpw", "--db_pswd", default=config.db_pswd, help="database user password")  # noqa: E501
     parser.add_argument("-dbp", "--db_port", type=int, default=config.db_port, help="database port number")  # noqa: E501
     parser.add_argument("-dbh", "--db_host", type=str, default=config.db_host, help="database hostname")  # noqa: E501
     parser.add_argument("-wh", "--web_host", type=str, default=config.web_host, help="web operator panel hostname")  # noqa: E501
     parser.add_argument("-wp", "--web_port", type=str, default=config.web_port, help="web operator panel port")  # noqa: E501
     parser.add_argument("path", type=str, nargs='?', help="path to test directory")
     # fmt: on
```

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/asset-manifest.json` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/favicon.ico` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/index.html` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/index.html`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/logo512.png` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/logo512.png`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/css/main.e8a862f1.css` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/css/main.e8a862f1.css`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/css/main.e8a862f1.css.map` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/css/main.e8a862f1.css.map`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/js/808.ce070002.chunk.js` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/js/808.ce070002.chunk.js`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/js/808.ce070002.chunk.js.map` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/js/808.ce070002.chunk.js.map`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-16px-paths.d605910e.chunk.js` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-16px-paths.d605910e.chunk.js`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-16px-paths.d605910e.chunk.js.map` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-16px-paths.d605910e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-20px-paths.7ee05cc8.chunk.js` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-20px-paths.7ee05cc8.chunk.js`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-20px-paths.7ee05cc8.chunk.js.map` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-20px-paths.7ee05cc8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-all-paths-loader.0aa89747.chunk.js.map` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-all-paths-loader.0aa89747.chunk.js.map`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-all-paths.f63155c9.chunk.js.map` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-all-paths.f63155c9.chunk.js.map`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-split-paths-by-size-loader.52a072d3.chunk.js` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-split-paths-by-size-loader.52a072d3.chunk.js`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-split-paths-by-size-loader.52a072d3.chunk.js.map` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/js/blueprint-icons-split-paths-by-size-loader.52a072d3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/js/main.8ef63e9b.js` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/js/main.8ef63e9b.js`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/js/main.8ef63e9b.js.LICENSE.txt` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/js/main.8ef63e9b.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/js/main.8ef63e9b.js.map` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/js/main.8ef63e9b.js.map`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-16.520846c6beb41df528c8.eot` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-16.520846c6beb41df528c8.eot`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-16.5c52b39c697f2323ce8b.svg` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-16.5c52b39c697f2323ce8b.svg`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-16.84db1772f4bfb529f64f.woff` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-16.84db1772f4bfb529f64f.woff`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-16.b67ee1736e20e37a3225.woff2` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-16.b67ee1736e20e37a3225.woff2`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-16.e02ecf515378db143652.ttf` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-16.e02ecf515378db143652.ttf`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-20.429cacb8accf72488451.ttf` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-20.429cacb8accf72488451.ttf`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-20.6ae3791ee2d86fc228a6.svg` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-20.6ae3791ee2d86fc228a6.svg`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-20.8cecf62de42997e4d82f.woff2` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-20.8cecf62de42997e4d82f.woff2`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-20.afbadb627d43b7857223.eot` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-20.afbadb627d43b7857223.eot`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-20.e857f5a5132b8bfa71a1.woff` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/media/blueprint-icons-20.e857f5a5132b8bfa71a1.woff`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/hardpy_panel/frontend/dist/static/media/logo_smol.5b16f92447a4a9e80331.png` & `hardpy-0.2.0/hardpy/hardpy_panel/frontend/dist/static/media/logo_smol.5b16f92447a4a9e80331.png`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/pytest_hardpy/plugin.py` & `hardpy-0.2.0/hardpy/pytest_hardpy/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,16 +33,23 @@
     """Register argparse-style options."""
     config_data = ConfigData()
     # fmt: off
     parser.addoption("--hardpy-dbu", action="store", default=config_data.db_user, help="database user")  # noqa: E501
     parser.addoption("--hardpy-dbpw", action="store", default=config_data.db_pswd, help="database user password")  # noqa: E501
     parser.addoption("--hardpy-dbp", action="store", default=config_data.db_port, help="database port number")  # noqa: E501
     parser.addoption("--hardpy-dbh", action="store", default=config_data.db_host, help="database hostname")  # noqa: E501
+    parser.addoption("--hardpy-pt", action="store_true", default=False, help="enable pytest-hardpy plugin")  # noqa: E501
     # fmt: on
 
+# Bootstrapping hooks
+def pytest_load_initial_conftests(early_config, parser, args):
+    if "--hardpy-pt" in args:
+        plugin = HardpyPlugin()
+        early_config.pluginmanager.register(plugin)
+
 
 class HardpyPlugin(object):
     """HardPy integration plugin for pytest.
 
     Extends hook functions from pytest API.
     """
 
@@ -53,14 +60,15 @@
 
         if system() == "Linux":
             signal.signal(signal.SIGTERM, self._stop_handler)
         elif system() == "Windows":
             signal.signal(signal.SIGBREAK, self._stop_handler)
         self._log = getLogger(__name__)
 
+
     # Initialization hooks
 
     def pytest_configure(self, config: Config):
         """Configure pytest."""
         config_data = ConfigData()
         config_data.db_user = config.getoption("--hardpy-dbu")
         config_data.db_host = config.getoption("--hardpy-dbh")
```

### Comparing `hardpy-0.1.0/hardpy/pytest_hardpy/pytest_call.py` & `hardpy-0.2.0/hardpy/pytest_hardpy/pytest_call.py`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/pytest_hardpy/pytest_wrapper.py` & `hardpy-0.2.0/hardpy/pytest_hardpy/pytest_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
                     str(self.config.db_port),
                     "--hardpy-dbh",
                     self.config.db_host,
                     "--hardpy-dbu",
                     self.config.db_user,
                     "--hardpy-dbpw",
                     self.config.db_pswd,
+                    "--hardpy-pt",
                 ],
                 cwd=self.config.tests_dir.absolute(),
             )
         elif system() == "Windows":
             self._proc = subprocess.Popen(  # noqa: S603
                 [
                     self.python_executable,
@@ -59,14 +60,15 @@
                     str(self.config.db_port),
                     "--hardpy-dbh",
                     self.config.db_host,
                     "--hardpy-dbu",
                     self.config.db_user,
                     "--hardpy-dbpw",
                     self.config.db_pswd,
+                    "--hardpy-pt",
                 ],
                 cwd=self.config.tests_dir.absolute(),
                 creationflags=subprocess.CREATE_NEW_PROCESS_GROUP,
             )
 
         return True
 
@@ -103,14 +105,15 @@
                 str(self.config.db_port),
                 "--hardpy-dbh",
                 self.config.db_host,
                 "--hardpy-dbu",
                 self.config.db_user,
                 "--hardpy-dbpw",
                 self.config.db_pswd,
+                "--hardpy-pt",
             ],
             cwd=self.config.tests_dir.absolute(),
         )
         return True
 
     def is_running(self) -> bool | None:
         """Check if pytest is running."""
```

### Comparing `hardpy-0.1.0/hardpy/pytest_hardpy/db/__init__.py` & `hardpy-0.2.0/hardpy/pytest_hardpy/db/__init__.py`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/pytest_hardpy/db/base_connector.py` & `hardpy-0.2.0/hardpy/pytest_hardpy/db/base_connector.py`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/pytest_hardpy/db/base_store.py` & `hardpy-0.2.0/hardpy/pytest_hardpy/db/base_store.py`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/pytest_hardpy/db/const.py` & `hardpy-0.2.0/hardpy/pytest_hardpy/db/const.py`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/pytest_hardpy/db/runstore.py` & `hardpy-0.2.0/hardpy/pytest_hardpy/db/runstore.py`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/pytest_hardpy/db/schema.py` & `hardpy-0.2.0/hardpy/pytest_hardpy/db/schema.py`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/pytest_hardpy/db/statestore.py` & `hardpy-0.2.0/hardpy/pytest_hardpy/db/statestore.py`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/pytest_hardpy/reporter/base.py` & `hardpy-0.2.0/hardpy/pytest_hardpy/reporter/base.py`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/pytest_hardpy/reporter/hook_reporter.py` & `hardpy-0.2.0/hardpy/pytest_hardpy/reporter/hook_reporter.py`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/pytest_hardpy/reporter/runner_reporter.py` & `hardpy-0.2.0/hardpy/pytest_hardpy/reporter/runner_reporter.py`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/pytest_hardpy/result/couchdb_config.py` & `hardpy-0.2.0/hardpy/pytest_hardpy/result/couchdb_config.py`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/pytest_hardpy/result/report_loader/couchdb_loader.py` & `hardpy-0.2.0/hardpy/pytest_hardpy/result/report_loader/couchdb_loader.py`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/pytest_hardpy/result/report_reader/couchdb_reader.py` & `hardpy-0.2.0/hardpy/pytest_hardpy/result/report_reader/couchdb_reader.py`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/pytest_hardpy/utils/__init__.py` & `hardpy-0.2.0/hardpy/pytest_hardpy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/pytest_hardpy/utils/config_data.py` & `hardpy-0.2.0/hardpy/pytest_hardpy/utils/config_data.py`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/pytest_hardpy/utils/const.py` & `hardpy-0.2.0/hardpy/pytest_hardpy/utils/const.py`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/pytest_hardpy/utils/node_info.py` & `hardpy-0.2.0/hardpy/pytest_hardpy/utils/node_info.py`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/pytest_hardpy/utils/progress_calculator.py` & `hardpy-0.2.0/hardpy/pytest_hardpy/utils/progress_calculator.py`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/hardpy/pytest_hardpy/utils/singleton.py` & `hardpy-0.2.0/hardpy/pytest_hardpy/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/LICENSE` & `hardpy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hardpy-0.1.0/pyproject.toml` & `hardpy-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) 2024 Everypin
 # GNU General Public License v3.0 (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 [project]
     name = "hardpy"
-    version = "0.1.0"
+    version = "0.2.0"
     description = "HardPy library for device testing"
     authors = [{ name = "Everypin" }]
     readme = "README.md"
     classifiers = [
         "Development Status :: 4 - Beta",
         "Framework :: Pytest",
         "Intended Audience :: Developers",
```

