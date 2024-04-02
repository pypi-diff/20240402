# Comparing `tmp/ssb_datadoc-0.8.1.tar.gz` & `tmp/ssb_datadoc-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_datadoc-0.8.1.tar", max compression
+gzip compressed data, was "ssb_datadoc-0.8.2.tar", max compression
```

## Comparing `ssb_datadoc-0.8.1.tar` & `ssb_datadoc-0.8.2.tar`

### file list

```diff
@@ -1,47 +1,51 @@
--rw-r--r--   0        0        0     1073 2024-03-14 09:48:53.891064 ssb_datadoc-0.8.1/LICENSE
--rw-r--r--   0        0        0     3034 2024-03-14 09:48:53.891064 ssb_datadoc-0.8.1/README.md
--rw-r--r--   0        0        0     5188 2024-03-14 09:49:05.011244 ssb_datadoc-0.8.1/pyproject.toml
--rw-r--r--   0        0        0       85 2024-03-14 09:48:53.891064 ssb_datadoc-0.8.1/src/datadoc/__init__.py
--rw-r--r--   0        0        0     5185 2024-03-14 09:48:53.891064 ssb_datadoc-0.8.1/src/datadoc/app.py
--rw-r--r--   0        0        0    80523 2024-03-14 09:48:53.891064 ssb_datadoc-0.8.1/src/datadoc/assets/bootstrap-icons.css
--rw-r--r--   0        0        0   163874 2024-03-14 09:48:53.891064 ssb_datadoc-0.8.1/src/datadoc/assets/bootstrap.min.css
--rw-r--r--   0        0        0    52127 2024-03-14 09:48:53.891064 ssb_datadoc-0.8.1/src/datadoc/assets/bundle.css
--rw-r--r--   0        0        0   137124 2024-03-14 09:48:53.891064 ssb_datadoc-0.8.1/src/datadoc/assets/fonts/bootstrap-icons.woff
--rw-r--r--   0        0        0   102536 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/assets/fonts/bootstrap-icons.woff2
--rw-r--r--   0        0        0     1464 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/assets/variables_style.css
--rw-r--r--   0        0        0       56 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/backend/__init__.py
--rw-r--r--   0        0        0     5524 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/backend/code_list.py
--rw-r--r--   0        0        0    13540 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/backend/dapla_dataset_path_info.py
--rw-r--r--   0        0        0    11054 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/backend/datadoc_metadata.py
--rw-r--r--   0        0        0     7239 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/backend/dataset_parser.py
--rw-r--r--   0        0        0       83 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/backend/external_sources/__init__.py
--rw-r--r--   0        0        0     1738 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/backend/external_sources/external_sources.py
--rw-r--r--   0        0        0     5321 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/backend/model_backwards_compatibility.py
--rw-r--r--   0        0        0     5666 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/backend/statistic_subject_mapping.py
--rw-r--r--   0        0        0     2500 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/backend/user_info.py
--rw-r--r--   0        0        0     3730 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/config.py
--rw-r--r--   0        0        0     6184 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/enums.py
--rw-r--r--   0        0        0       52 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/frontend/__init__.py
--rw-r--r--   0        0        0      310 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/frontend/callbacks/__init__.py
--rw-r--r--   0        0        0     6861 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/frontend/callbacks/dataset.py
--rw-r--r--   0        0        0    11124 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/frontend/callbacks/register_callbacks.py
--rw-r--r--   0        0        0     5623 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/frontend/callbacks/utils.py
--rw-r--r--   0        0        0     5417 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/frontend/callbacks/variables.py
--rw-r--r--   0        0        0      190 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/frontend/components/__init__.py
--rw-r--r--   0        0        0     1063 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/frontend/components/alerts.py
--rw-r--r--   0        0        0     4711 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/frontend/components/builders.py
--rw-r--r--   0        0        0     3675 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/frontend/components/control_bars.py
--rw-r--r--   0        0        0     3103 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/frontend/components/dataset_tab.py
--rw-r--r--   0        0        0     1595 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/frontend/components/variables_tab.py
--rw-r--r--   0        0        0       74 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/frontend/fields/__init__.py
--rw-r--r--   0        0        0     7850 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/frontend/fields/display_base.py
--rw-r--r--   0        0        0    13361 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/frontend/fields/display_dataset.py
--rw-r--r--   0        0        0     8185 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/frontend/fields/display_variables.py
--rw-r--r--   0        0        0       72 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/logging/__init__.py
--rw-r--r--   0        0        0     1586 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/logging/json_formatter.py
--rw-r--r--   0        0        0     1733 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/logging/logging_config.py
--rw-r--r--   0        0        0        0 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/py.typed
--rw-r--r--   0        0        0      898 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/state.py
--rw-r--r--   0        0        0     2153 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/utils.py
--rw-r--r--   0        0        0      113 2024-03-14 09:48:53.895064 ssb_datadoc-0.8.1/src/datadoc/wsgi.py
--rw-r--r--   0        0        0     4583 1970-01-01 00:00:00.000000 ssb_datadoc-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-02 10:56:19.575211 ssb_datadoc-0.8.2/LICENSE
+-rw-r--r--   0        0        0     3034 2024-04-02 10:56:19.575211 ssb_datadoc-0.8.2/README.md
+-rw-r--r--   0        0        0     5188 2024-04-02 10:56:27.959211 ssb_datadoc-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0       85 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/__init__.py
+-rw-r--r--   0        0        0     5885 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/app.py
+-rw-r--r--   0        0        0      133 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/assets/app_style.css
+-rw-r--r--   0        0        0    80523 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/assets/bootstrap-icons.css
+-rw-r--r--   0        0        0   163874 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/assets/bootstrap.min.css
+-rw-r--r--   0        0        0    52127 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/assets/bundle.css
+-rw-r--r--   0        0        0      346 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/assets/controlbar_style.css
+-rw-r--r--   0        0        0   137124 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/assets/fonts/bootstrap-icons.woff
+-rw-r--r--   0        0        0   102536 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/assets/fonts/bootstrap-icons.woff2
+-rw-r--r--   0        0        0      213 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/assets/header.css
+-rw-r--r--   0        0        0     1405 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/assets/workspace_style.css
+-rw-r--r--   0        0        0      131 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/assets/workspace_tab.css
+-rw-r--r--   0        0        0       56 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/backend/__init__.py
+-rw-r--r--   0        0        0     5635 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/backend/code_list.py
+-rw-r--r--   0        0        0    13540 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/backend/dapla_dataset_path_info.py
+-rw-r--r--   0        0        0    11054 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/backend/datadoc_metadata.py
+-rw-r--r--   0        0        0     7491 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/backend/dataset_parser.py
+-rw-r--r--   0        0        0       83 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/backend/external_sources/__init__.py
+-rw-r--r--   0        0        0     1681 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/backend/external_sources/external_sources.py
+-rw-r--r--   0        0        0     5321 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/backend/model_backwards_compatibility.py
+-rw-r--r--   0        0        0     5828 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/backend/statistic_subject_mapping.py
+-rw-r--r--   0        0        0     2500 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/backend/user_info.py
+-rw-r--r--   0        0        0     3730 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/config.py
+-rw-r--r--   0        0        0     6184 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/enums.py
+-rw-r--r--   0        0        0       52 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/__init__.py
+-rw-r--r--   0        0        0      310 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/callbacks/__init__.py
+-rw-r--r--   0        0        0     7865 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/callbacks/dataset.py
+-rw-r--r--   0        0        0    13456 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/callbacks/register_callbacks.py
+-rw-r--r--   0        0        0     5623 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/callbacks/utils.py
+-rw-r--r--   0        0        0     5466 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/callbacks/variables.py
+-rw-r--r--   0        0        0      190 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/components/__init__.py
+-rw-r--r--   0        0        0     1063 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/components/alerts.py
+-rw-r--r--   0        0        0     5414 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/components/builders.py
+-rw-r--r--   0        0        0     2502 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/components/control_bars.py
+-rw-r--r--   0        0        0     1101 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/components/dataset_tab.py
+-rw-r--r--   0        0        0     1734 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/components/variables_tab.py
+-rw-r--r--   0        0        0       74 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/fields/__init__.py
+-rw-r--r--   0        0        0     8725 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/fields/display_base.py
+-rw-r--r--   0        0        0    13438 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/fields/display_dataset.py
+-rw-r--r--   0        0        0     8336 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/fields/display_variables.py
+-rw-r--r--   0        0        0       72 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/logging_configuration/__init__.py
+-rw-r--r--   0        0        0     1586 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/logging_configuration/json_formatter.py
+-rw-r--r--   0        0        0     1747 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/logging_configuration/logging_config.py
+-rw-r--r--   0        0        0        0 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/py.typed
+-rw-r--r--   0        0        0      898 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/state.py
+-rw-r--r--   0        0        0     2153 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/utils.py
+-rw-r--r--   0        0        0      220 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/wsgi.py
+-rw-r--r--   0        0        0     4583 1970-01-01 00:00:00.000000 ssb_datadoc-0.8.2/PKG-INFO
```

### Comparing `ssb_datadoc-0.8.1/LICENSE` & `ssb_datadoc-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.1/README.md` & `ssb_datadoc-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.1/pyproject.toml` & `ssb_datadoc-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-datadoc"
-version = "0.8.1"
+version = "0.8.2"
 description = "Document dataset metadata. For use in Statistics Norway's metadata system."
 authors = ["Statistics Norway <stat-dev@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/datadoc"
 repository = "https://github.com/statisticsnorway/datadoc"
 documentation = "https://statisticsnorway.github.io/datadoc"
```

### Comparing `ssb_datadoc-0.8.1/src/datadoc/app.py` & `ssb_datadoc-0.8.2/src/datadoc/app.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Top-level entrypoint, configuration and layout for the datadoc app.
 
 Members of this module should not be imported into any sub-modules, this will cause circular imports.
 """
 
 from __future__ import annotations
 
+import concurrent
 import logging
 from pathlib import Path
 
 import dash_bootstrap_components as dbc
 from dash import Dash
+from dash import html
 from flask_healthz import healthz
 
 from datadoc import config
 from datadoc import state
 from datadoc.backend.code_list import CodeList
 from datadoc.backend.datadoc_metadata import DataDocMetadata
 from datadoc.backend.statistic_subject_mapping import StatisticSubjectMapping
@@ -26,15 +28,15 @@
 from datadoc.frontend.components.alerts import variables_validation_error
 from datadoc.frontend.components.control_bars import build_controls_bar
 from datadoc.frontend.components.control_bars import build_language_dropdown
 from datadoc.frontend.components.control_bars import header
 from datadoc.frontend.components.control_bars import progress_bar
 from datadoc.frontend.components.dataset_tab import build_dataset_tab
 from datadoc.frontend.components.variables_tab import build_variables_tab
-from datadoc.logging.logging_config import configure_logging
+from datadoc.logging_configuration.logging_config import configure_logging
 from datadoc.utils import get_app_version
 from datadoc.utils import pick_random_port
 from datadoc.utils import running_in_notebook
 
 configure_logging()
 logger = logging.getLogger(__name__)
 
@@ -42,48 +44,56 @@
 def build_app(app: type[Dash]) -> Dash:
     """Define the layout, register callbacks."""
     tabs_children = [
         build_dataset_tab(),
         build_variables_tab(),
     ]
 
-    app.layout = dbc.Container(
-        style={"padding": "4px"},
+    app.layout = html.Div(
         children=[
-            header,
-            progress_bar,
-            build_controls_bar(),
-            variables_validation_error,
-            dataset_validation_error,
-            opened_dataset_error,
-            saved_metadata_success,
-            opened_dataset_success,
-            dbc.CardBody(
-                style={"padding": "4px"},
-                children=[
+            html.Header(
+                [
+                    header,
+                ],
+                className="header-wrapper",
+            ),
+            html.Main(
+                [
+                    progress_bar,
+                    build_controls_bar(),
+                    variables_validation_error,
+                    dataset_validation_error,
+                    opened_dataset_error,
+                    saved_metadata_success,
+                    opened_dataset_success,
                     dbc.Tabs(
                         id="tabs",
                         class_name="ssb-tabs",
                         children=tabs_children,
                     ),
                 ],
+                className="main-content-app",
             ),
             build_language_dropdown(),
         ],
+        className="app-wrapper",
     )
 
     register_callbacks(app)
 
     return app
 
 
-def get_app(dataset_path: str | None = None) -> tuple[Dash, int]:
+def get_app(
+    executor: concurrent.futures.ThreadPoolExecutor,
+    dataset_path: str | None = None,
+) -> tuple[Dash, int]:
     """Centralize all the ugliness around initializing the app."""
     logger.info("Datadoc version v%s", get_app_version())
-    collect_data_from_external_sources()
+    collect_data_from_external_sources(executor)
     state.current_metadata_language = SupportedLanguages.NORSK_BOKMÅL
     state.metadata = DataDocMetadata(
         state.statistic_subject_mapping,
         dataset_path=dataset_path,
     )
 
     # The service prefix must be set to run correctly on Dapla Jupyter
@@ -110,48 +120,57 @@
         "startup": lambda: True,
     }
     logger.info("Built app with endpoints configured on /healthz")
 
     return app, port
 
 
-def collect_data_from_external_sources() -> None:
+def collect_data_from_external_sources(
+    executor: concurrent.futures.ThreadPoolExecutor,
+) -> None:
     """Call classes and methods which collect data from external sources.
 
     Must be non-blocking to prevent delays in app startup.
     """
+    logger.debug("Start threads - Collecting data from external sources")
     state.statistic_subject_mapping = StatisticSubjectMapping(
+        executor,
         config.get_statistical_subject_source_url(),
     )
 
     state.unit_types = CodeList(
+        executor,
         config.get_unit_code(),
     )
 
     state.organisational_units = CodeList(
+        executor,
         config.get_organisational_unit_code(),
     )
+    logger.debug("Finished blocking - Collecting data from external sources")
 
 
 def main(dataset_path: str | None = None) -> None:
     """Entrypoint when running as a script."""
     if dataset_path:
         logger.info("Starting app with dataset_path = %s", dataset_path)
-    app, port = get_app(dataset_path)
-    if running_in_notebook():
-        logger.info("Running in notebook")
-        app.run(
-            jupyter_mode="tab",
-            jupyter_server_url=config.get_jupyterhub_http_referrer(),
-            jupyter_height=1000,
-            port=port,
-        )
-    else:
-        if dev_mode := config.get_dash_development_mode():
-            logger.warning(
-                "Starting in Development Mode. NOT SUITABLE FOR PRODUCTION.",
+
+    with concurrent.futures.ThreadPoolExecutor(max_workers=12) as executor:
+        app, port = get_app(executor, dataset_path)
+        if running_in_notebook():
+            logger.info("Running in notebook")
+            app.run(
+                jupyter_mode="tab",
+                jupyter_server_url=config.get_jupyterhub_http_referrer(),
+                jupyter_height=1000,
+                port=port,
             )
-        app.run(debug=dev_mode, port=port)
+        else:
+            if dev_mode := config.get_dash_development_mode():
+                logger.warning(
+                    "Starting in Development Mode. NOT SUITABLE FOR PRODUCTION.",
+                )
+            app.run(debug=dev_mode, port=port)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ssb_datadoc-0.8.1/src/datadoc/assets/bootstrap-icons.css` & `ssb_datadoc-0.8.2/src/datadoc/assets/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.1/src/datadoc/assets/bootstrap.min.css` & `ssb_datadoc-0.8.2/src/datadoc/assets/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.1/src/datadoc/assets/bundle.css` & `ssb_datadoc-0.8.2/src/datadoc/assets/bundle.css`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.1/src/datadoc/assets/fonts/bootstrap-icons.woff` & `ssb_datadoc-0.8.2/src/datadoc/assets/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.1/src/datadoc/assets/fonts/bootstrap-icons.woff2` & `ssb_datadoc-0.8.2/src/datadoc/assets/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.1/src/datadoc/assets/variables_style.css` & `ssb_datadoc-0.8.2/src/datadoc/assets/workspace_style.css`

 * *Files 13% similar despite different names*

```diff
@@ -1,92 +1,87 @@
-.page-wrapper{
+.workspace-page-wrapper{
     display: flex;
     flex-wrap: wrap;
     flex-direction: row;
     padding: 0;
 }
 
-.content-wrapper{
-    display: flex;
-    width: 100%;
-    gap: 1rem;
-}
-
-.main-content{
-    width: 100%;
-    display: flex;
-    flex-direction: column;
-    gap: 1rem;
-}
-
-
-.variables-header{
+.workspace-header{
     width: 100%;
     display:flex;
     flex-wrap: wrap;
     justify-content: space-between;
     align-items: center;
+    margin-bottom: 1rem;
 }
 
-.ssb-title.variables-title{
+.ssb-title.workspace-title{
     margin-top: 1rem;
     width: 100%;
 }
 
-.ssb-input{
-    margin-bottom: 1rem;
-}
-.accordion-wrapper{
+.workspace-content{
+    width: 100%;
     display: flex;
     flex-direction: column;
     gap: 1rem;
 }
 
-.ssb-accordion.variable-accordion{
-    border: 2px solid #62919A;
-    padding: 0.5rem;
+.ssb-accordion.variable-accordion > .accordion-body {
+    padding: 1rem;
 }
 
-.ssb-accordion.variable-accordion > .accordion-body {
+.edit-section{
+    display: flex;
+    flex-direction: column;
+    gap: 1rem;
+    width: 100%;
+}
+
+.edit-section.dataset-edit-section{
     padding: 1rem;
 }
 
-.variables-input-group{
+.edit-section-form{
     display: flex;
     flex-wrap: wrap;
-    justify-content: flex-start;
-    align-items: flex-start;
-    gap: 1rem;
+    gap: 2rem;
     padding-top: 1rem;
 }
 
-/*.input-section{
-    margin: 1rem;
-}*/
-
 .alert-section{
     display: flex;
     flex-wrap: wrap;
     justify-content: space-around;
     gap: 1rem;
     padding-top: 1rem;
 }
 
-.ssb-title.input-section-title{
+.ssb-title.edit-section-title{
     border-bottom: 2px solid #62919A;
     margin-bottom: 1rem;
+    padding-bottom: 1rem;
+
+}
 
+.ssb-input.input-component{
+    max-width: 500px;
+    width: 100%;
 }
 
-.ssb-input.variable-input{
+.ssb-dropdown.dropdown-component {
     max-width: 500px;
     width: 100%;
 }
 
 .form-check.ssb-checkbox{
     align-self: center;
 }
 
+.form-check{
+    padding-left: 0;
+}
+
 /*Target child selector (label) of variable-dropdown*/
 .ssb-dropdown.variable-dropdown > .dropdown-label{
     margin-bottom: 0.6rem;
 }
```

### Comparing `ssb_datadoc-0.8.1/src/datadoc/backend/code_list.py` & `ssb_datadoc-0.8.2/src/datadoc/backend/code_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from dataclasses import dataclass
 from typing import TYPE_CHECKING
 
 from datadoc.backend.external_sources.external_sources import GetExternalSource
 from datadoc.enums import SupportedLanguages
 
 if TYPE_CHECKING:
+    import concurrent
+
     import pandas as pd
 
 from klass.classes.classification import KlassClassification
 
 logger = logging.getLogger(__name__)
 
 
@@ -47,27 +49,31 @@
                 )
                 return ""
 
 
 class CodeList(GetExternalSource):
     """Class for retrieving classifications from Klass."""
 
-    def __init__(self, classification_id: int | None) -> None:
+    def __init__(
+        self,
+        executor: concurrent.futures.ThreadPoolExecutor,
+        classification_id: int | None,
+    ) -> None:
         """Retrieves a list of classifications given a classification id.
 
         Initializes the classifications list and starts fetching the classifications.
         """
         self.supported_languages = [
             SupportedLanguages.NORSK_BOKMÅL.value,
             SupportedLanguages.ENGLISH.value,
         ]
         self._classifications: list[CodeListItem] = []
         self.classification_id = classification_id
         self.classifications_dataframes: dict[str, pd.DataFrame] | None = None
-        super().__init__()
+        super().__init__(executor)
 
     def _fetch_data_from_external_source(
         self,
     ) -> dict[str, pd.DataFrame] | None:
         """Fetches the classifications from Klass by classification id.
 
         returns a pandas dataframe with the class data for the given classification id.
```

### Comparing `ssb_datadoc-0.8.1/src/datadoc/backend/dapla_dataset_path_info.py` & `ssb_datadoc-0.8.2/src/datadoc/backend/dapla_dataset_path_info.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.1/src/datadoc/backend/datadoc_metadata.py` & `ssb_datadoc-0.8.2/src/datadoc/backend/datadoc_metadata.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.1/src/datadoc/backend/dataset_parser.py` & `ssb_datadoc-0.8.2/src/datadoc/backend/dataset_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 import pathlib  # noqa: TCH003 import is needed for docs build
 import re
 import typing as t
 from abc import ABC
 from abc import abstractmethod
 
 import pandas as pd
-import pyarrow.parquet as pq
 from datadoc_model.model import LanguageStringType
 from datadoc_model.model import Variable
+from pyarrow import parquet as pq
 
 from datadoc import state
 from datadoc.enums import DataType
 
 if t.TYPE_CHECKING:
+    import pyarrow as pa
     from cloudpathlib import CloudPath
 
 KNOWN_INTEGER_TYPES = (
     "int",
     "int_",
     "int8",
     "int16",
@@ -165,21 +166,24 @@
     def __init__(self, dataset: pathlib.Path | CloudPath) -> None:
         """Use the super init method."""
         super().__init__(dataset)
 
     def get_fields(self) -> list[Variable]:
         """Extract the fields from this dataset."""
         with self.dataset.open(mode="rb") as f:
-            data_table = pq.read_table(f)  # type: ignore [arg-type]
+            # Type stubs for pyarrow are incorrect see https://github.com/zen-xu/pyarrow-stubs/issues/4
+            schema: pa.Schema = pq.read_schema(f)  # type: ignore  # noqa: PGH003
         return [
             Variable(
-                short_name=data_field.name,
+                short_name=data_field.name.strip(),
                 data_type=self.transform_data_type(str(data_field.type)),
             )
-            for data_field in data_table.schema
+            for data_field in schema
+            if data_field.name
+            != "__index_level_0__"  # Index columns should not be documented
         ]
 
 
 class DatasetParserSas7Bdat(DatasetParser):
     """Concrete implementation for parsing SAS7BDAT files."""
 
     def __init__(self, dataset: pathlib.Path | CloudPath) -> None:
```

### Comparing `ssb_datadoc-0.8.1/src/datadoc/backend/external_sources/external_sources.py` & `ssb_datadoc-0.8.2/src/datadoc/backend/external_sources/external_sources.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 from __future__ import annotations
 
-import concurrent.futures
 import logging
 from abc import ABC
 from abc import abstractmethod
+from typing import TYPE_CHECKING
 from typing import Generic
 from typing import TypeVar
 
+if TYPE_CHECKING:
+    import concurrent.futures
+
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
 
 
 class GetExternalSource(ABC, Generic[T]):
     """Abstract base class for getting data from external sources."""
 
-    def __init__(self) -> None:
+    def __init__(self, executor: concurrent.futures.ThreadPoolExecutor) -> None:
         """Retrieves data from an external source asynchronously.
 
         Initializes the future object.
         """
-        self.future: concurrent.futures.Future[T | None] | None = None
-        with concurrent.futures.ThreadPoolExecutor(max_workers=1) as executor:
-            self.future = executor.submit(
-                self._fetch_data_from_external_source,
-            )
+        self.future = executor.submit(
+            self._fetch_data_from_external_source,
+        )
 
     def wait_for_external_result(self) -> None:
         """Waits for the thread responsible for loading the external request to finish."""
         if not self.future:
             logger.warning("No future to wait for.")
             # Nothing to wait for in this case, just return immediately
             return
```

### Comparing `ssb_datadoc-0.8.1/src/datadoc/backend/model_backwards_compatibility.py` & `ssb_datadoc-0.8.2/src/datadoc/backend/model_backwards_compatibility.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.1/src/datadoc/backend/statistic_subject_mapping.py` & `ssb_datadoc-0.8.2/src/datadoc/backend/statistic_subject_mapping.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from __future__ import annotations
 
 import logging
 from dataclasses import dataclass
+from typing import TYPE_CHECKING
 
 import bs4
 import requests
 from bs4 import BeautifulSoup
 from bs4 import ResultSet
 
 from datadoc.backend.external_sources.external_sources import GetExternalSource
 from datadoc.enums import SupportedLanguages
 
+if TYPE_CHECKING:
+    import concurrent
+
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class Subject:
     """Base class for Primary and Secondary subjects."""
 
@@ -58,26 +62,30 @@
 
     secondary_subjects: list[SecondarySubject]
 
 
 class StatisticSubjectMapping(GetExternalSource):
     """Allow mapping between statistic short name and primary and secondary subject."""
 
-    def __init__(self, source_url: str | None) -> None:
+    def __init__(
+        self,
+        executor: concurrent.futures.ThreadPoolExecutor,
+        source_url: str | None,
+    ) -> None:
         """Retrieves the statistical structure document from the given URL.
 
         Initializes the mapping dicts. Based on the values in the statistical structure document.
         """
         self.source_url = source_url
 
         self._statistic_subject_structure_xml: ResultSet | None = None
 
         self._primary_subjects: list[PrimarySubject] = []
 
-        super().__init__()
+        super().__init__(executor)
 
     def get_secondary_subject(self, statistic_short_name: str | None) -> str | None:
         """Looks up the secondary subject for the given statistic short name in the mapping dict.
 
         Returns the secondary subject string if found, else None.
         """
         for p in self.primary_subjects:
```

### Comparing `ssb_datadoc-0.8.1/src/datadoc/backend/user_info.py` & `ssb_datadoc-0.8.2/src/datadoc/backend/user_info.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.1/src/datadoc/config.py` & `ssb_datadoc-0.8.2/src/datadoc/config.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.1/src/datadoc/enums.py` & `ssb_datadoc-0.8.2/src/datadoc/enums.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.1/src/datadoc/frontend/callbacks/dataset.py` & `ssb_datadoc-0.8.2/src/datadoc/frontend/callbacks/dataset.py`

 * *Files 20% similar despite different names*

```diff
@@ -51,14 +51,17 @@
 
 
 def open_dataset_handling(
     n_clicks: int,
     file_path: str,
 ) -> tuple[bool, bool, str, str]:
     """Handle errors and other logic around opening a dataset file."""
+    if file_path:
+        file_path = file_path.strip()
+
     try:
         state.metadata = open_file(file_path)
     except FileNotFoundError:
         logger.exception("File %s not found", str(file_path))
         return (
             False,
             True,
@@ -98,34 +101,14 @@
     """
     updated_value: MetadataInputTypes | LanguageStringType
     if metadata_identifier == DatasetIdentifiers.KEYWORD.value and isinstance(
         value,
         str,
     ):
         updated_value = process_keyword(value)
-    elif metadata_identifier == DatasetIdentifiers.CONTAINS_DATA_FROM.value:
-        updated_value, _ = parse_and_validate_dates(
-            str(value),
-            getattr(
-                state.metadata.dataset,
-                DatasetIdentifiers.CONTAINS_DATA_UNTIL.value,
-            ),
-        )
-        if updated_value:
-            updated_value = updated_value.isoformat()
-    elif metadata_identifier == DatasetIdentifiers.CONTAINS_DATA_UNTIL.value:
-        _, updated_value = parse_and_validate_dates(
-            getattr(
-                state.metadata.dataset,
-                DatasetIdentifiers.CONTAINS_DATA_FROM.value,
-            ),
-            str(value),
-        )
-        if updated_value:
-            updated_value = updated_value.isoformat()
     elif metadata_identifier == DatasetIdentifiers.VERSION.value:
         updated_value = str(value)
     elif metadata_identifier in MULTIPLE_LANGUAGE_DATASET_METADATA and isinstance(
         value,
         str,
     ):
         updated_value = find_existing_language_string(
@@ -196,7 +179,66 @@
     - Update the language of all the metadata values.
     """
     update_global_language_state(language)
     return (
         *(e.options_getter(language) for e in DISPLAYED_DROPDOWN_DATASET_METADATA),
         update_dataset_metadata_language(),
     )
+
+
+def accept_dataset_metadata_date_input(
+    dataset_identifier: DatasetIdentifiers,
+    contains_data_from: str | None,
+    contains_data_until: str | None,
+) -> tuple[bool, str, bool, str]:
+    """Validate and save date range inputs."""
+    try:
+        (
+            parsed_contains_data_from,
+            parsed_contains_data_until,
+        ) = parse_and_validate_dates(
+            str(contains_data_from),
+            str(contains_data_until),
+        )
+
+        if parsed_contains_data_from:
+            state.metadata.dataset.contains_data_from = (
+                parsed_contains_data_from.isoformat()
+            )
+
+        if parsed_contains_data_until:
+            state.metadata.dataset.contains_data_until = (
+                parsed_contains_data_until.isoformat()
+            )
+
+    except (ValidationError, ValueError) as e:
+        logger.exception(
+            "Validation failed for %s, %s, %s: %s, %s",
+            dataset_identifier,
+            "contains_data_from",
+            contains_data_from,
+            "contains_data_until",
+            contains_data_until,
+        )
+        message: str | None = str(e)
+    else:
+        logger.debug(
+            "Successfully updated %s, %s, %s: %s, %s",
+            dataset_identifier,
+            "contains_data_from",
+            contains_data_from,
+            "contains_data_until",
+            contains_data_until,
+        )
+        message = None
+
+    no_error = (False, "")
+    if not message:
+        # No error to display.
+        return no_error + no_error
+
+    error = (True, message)
+    return (
+        error + no_error
+        if dataset_identifier == DatasetIdentifiers.CONTAINS_DATA_FROM
+        else no_error + error
+    )
```

### Comparing `ssb_datadoc-0.8.1/src/datadoc/frontend/callbacks/register_callbacks.py` & `ssb_datadoc-0.8.2/src/datadoc/frontend/callbacks/register_callbacks.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,29 +15,34 @@
 from dash import Output
 from dash import State
 from dash import ctx
 from dash import no_update
 
 from datadoc import state
 from datadoc.enums import SupportedLanguages
+from datadoc.frontend.callbacks.dataset import accept_dataset_metadata_date_input
 from datadoc.frontend.callbacks.dataset import accept_dataset_metadata_input
-from datadoc.frontend.callbacks.dataset import change_language_dataset_metadata
 from datadoc.frontend.callbacks.dataset import open_dataset_handling
 from datadoc.frontend.callbacks.utils import update_global_language_state
 from datadoc.frontend.callbacks.variables import accept_variable_metadata_date_input
 from datadoc.frontend.callbacks.variables import accept_variable_metadata_input
+from datadoc.frontend.components.builders import build_dataset_edit_section
 from datadoc.frontend.components.builders import build_edit_section
 from datadoc.frontend.components.builders import build_ssb_accordion
-from datadoc.frontend.components.dataset_tab import DATASET_METADATA_INPUT
-from datadoc.frontend.components.dataset_tab import build_dataset_metadata_accordion
+from datadoc.frontend.components.dataset_tab import SECTION_WRAPPER_ID
 from datadoc.frontend.components.variables_tab import ACCORDION_WRAPPER_ID
 from datadoc.frontend.components.variables_tab import VARIABLES_INFORMATION_ID
+from datadoc.frontend.fields.display_base import DATASET_METADATA_DATE_INPUT
+from datadoc.frontend.fields.display_base import DATASET_METADATA_INPUT
 from datadoc.frontend.fields.display_base import VARIABLES_METADATA_DATE_INPUT
 from datadoc.frontend.fields.display_base import VARIABLES_METADATA_INPUT
-from datadoc.frontend.fields.display_dataset import DISPLAYED_DROPDOWN_DATASET_METADATA
+from datadoc.frontend.fields.display_dataset import NON_EDITABLE_DATASET_METADATA
+from datadoc.frontend.fields.display_dataset import OBLIGATORY_EDITABLE_DATASET_METADATA
+from datadoc.frontend.fields.display_dataset import OPTIONAL_DATASET_METADATA
+from datadoc.frontend.fields.display_dataset import DatasetIdentifiers
 from datadoc.frontend.fields.display_variables import OBLIGATORY_VARIABLES_METADATA
 from datadoc.frontend.fields.display_variables import OPTIONAL_VARIABLES_METADATA
 from datadoc.frontend.fields.display_variables import VariableIdentifiers
 
 if TYPE_CHECKING:
     import dash_bootstrap_components as dbc
 
@@ -80,37 +85,14 @@
         if n_clicks and n_clicks > 0:
             state.metadata.write_metadata_document()
             return True
 
         return False
 
     @app.callback(
-        *[
-            Output(
-                {
-                    "type": DATASET_METADATA_INPUT,
-                    "id": m.identifier,
-                },
-                "options",
-            )
-            for m in DISPLAYED_DROPDOWN_DATASET_METADATA
-        ],
-        Output(
-            {"type": DATASET_METADATA_INPUT, "id": ALL},
-            "value",
-        ),
-        Input("language-dropdown", "value"),
-    )
-    def callback_change_language_dataset_metadata(
-        language: str,
-    ) -> tuple[object, ...]:
-        """Update dataset metadata values upon change of language."""
-        return change_language_dataset_metadata(SupportedLanguages(language))
-
-    @app.callback(
         Output("dataset-validation-error", "is_open"),
         Output("dataset-validation-explanation", "children"),
         Input({"type": DATASET_METADATA_INPUT, "id": ALL}, "value"),
         prevent_initial_call=True,
     )
     def callback_accept_dataset_metadata_input(
         value: MetadataInputTypes,  # noqa: ARG001 argument required by Dash
@@ -144,29 +126,14 @@
         To trigger reload of data in the UI, we update the
         language dropdown. This is a hack and could be replaced
         by a more formal mechanism.
         """
         return open_dataset_handling(n_clicks, dataset_path)
 
     @app.callback(
-        Output("dataset-accordion", "children"),
-        Input("open-button", "n_clicks"),
-        prevent_initial_call=True,
-    )
-    def callback_clear_accordion_values(n_clicks: int) -> list[dbc.AccordionItem]:
-        """Recreate accordion items with unique IDs.
-
-        The purpose is to avoid browser caching and clear the values of all
-        components inside the dataset accordion when new file is opened
-        """
-        if n_clicks and n_clicks > 0:
-            return build_dataset_metadata_accordion(n_clicks)
-        return no_update
-
-    @app.callback(
         Output(VARIABLES_INFORMATION_ID, "children"),
         Input("language-dropdown", "value"),
         prevent_initial_call=True,
     )
     def callback_populate_variables_info_section(
         language: str,  # noqa: ARG001 Dash requires arguments for all Inputs
     ) -> str:
@@ -206,14 +173,53 @@
                     ),
                 ],
             )
             for variable in list(state.metadata.variables)
         ]
 
     @app.callback(
+        Output(SECTION_WRAPPER_ID, "children"),
+        Input("language-dropdown", "value"),
+        Input("open-button", "n_clicks"),
+        prevent_initial_call=True,
+    )
+    def callback_populate_dataset_workspace(
+        language: str,
+        n_clicks: int,
+    ) -> list:
+        """Create dataset workspace with sections."""
+        update_global_language_state(SupportedLanguages(language))
+        logger.info("Populating new dataset workspace")
+        if n_clicks:
+            return [
+                build_dataset_edit_section(
+                    "Obligatorisk",
+                    OBLIGATORY_EDITABLE_DATASET_METADATA,
+                    state.current_metadata_language,
+                    state.metadata.dataset,
+                    {"type": "dataset-edit-section", "id": f"obligatory-{language}"},
+                ),
+                build_dataset_edit_section(
+                    "Anbefalt",
+                    OPTIONAL_DATASET_METADATA,
+                    state.current_metadata_language,
+                    state.metadata.dataset,
+                    {"type": "dataset-edit-section", "id": f"recommended-{language}"},
+                ),
+                build_dataset_edit_section(
+                    "Maskingenerert",
+                    NON_EDITABLE_DATASET_METADATA,
+                    state.current_metadata_language,
+                    state.metadata.dataset,
+                    {"type": "dataset-edit-section", "id": f"machine-{language}"},
+                ),
+            ]
+        return no_update
+
+    @app.callback(
         Output(
             {
                 "type": VARIABLES_METADATA_INPUT,
                 "variable_short_name": MATCH,
                 "id": MATCH,
             },
             "error",
@@ -309,7 +315,63 @@
         """Special case handling for date fields which have a relationship to one another."""
         return accept_variable_metadata_date_input(
             VariableIdentifiers(ctx.triggered_id["id"]),
             ctx.triggered_id["variable_short_name"],
             contains_data_from,
             contains_data_until,
         )
+
+    @app.callback(
+        Output(
+            {
+                "type": DATASET_METADATA_DATE_INPUT,
+                "id": DatasetIdentifiers.CONTAINS_DATA_FROM.value,
+            },
+            "error",
+        ),
+        Output(
+            {
+                "type": DATASET_METADATA_DATE_INPUT,
+                "id": DatasetIdentifiers.CONTAINS_DATA_FROM.value,
+            },
+            "errorMessage",
+        ),
+        Output(
+            {
+                "type": DATASET_METADATA_DATE_INPUT,
+                "id": DatasetIdentifiers.CONTAINS_DATA_UNTIL.value,
+            },
+            "error",
+        ),
+        Output(
+            {
+                "type": DATASET_METADATA_DATE_INPUT,
+                "id": DatasetIdentifiers.CONTAINS_DATA_UNTIL.value,
+            },
+            "errorMessage",
+        ),
+        Input(
+            {
+                "type": DATASET_METADATA_DATE_INPUT,
+                "id": DatasetIdentifiers.CONTAINS_DATA_FROM.value,
+            },
+            "value",
+        ),
+        Input(
+            {
+                "type": DATASET_METADATA_DATE_INPUT,
+                "id": DatasetIdentifiers.CONTAINS_DATA_UNTIL.value,
+            },
+            "value",
+        ),
+        prevent_initial_call=True,
+    )
+    def callback_accept_dataset_metadata_date_input(
+        contains_data_from: str,
+        contains_data_until: str,
+    ) -> dbc.Alert:
+        """Special case handling for date fields which have a relationship to one another."""
+        return accept_dataset_metadata_date_input(
+            DatasetIdentifiers(ctx.triggered_id["id"]),
+            contains_data_from,
+            contains_data_until,
+        )
```

### Comparing `ssb_datadoc-0.8.1/src/datadoc/frontend/callbacks/utils.py` & `ssb_datadoc-0.8.2/src/datadoc/frontend/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.1/src/datadoc/frontend/callbacks/variables.py` & `ssb_datadoc-0.8.2/src/datadoc/frontend/callbacks/variables.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,16 @@
             "Validation failed for %s, %s, %s:",
             metadata_field,
             variable_short_name,
             value,
         )
         return str(e)
     else:
+        if value == "":
+            value = None
         logger.debug(
             "Successfully updated %s, %s with %s",
             metadata_field,
             variable_short_name,
             value,
         )
         return None
```

### Comparing `ssb_datadoc-0.8.1/src/datadoc/frontend/components/alerts.py` & `ssb_datadoc-0.8.2/src/datadoc/frontend/components/alerts.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.1/src/datadoc/frontend/components/builders.py` & `ssb_datadoc-0.8.2/src/datadoc/frontend/components/builders.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 from enum import auto
 from typing import TYPE_CHECKING
 
 import dash_bootstrap_components as dbc
 import ssb_dash_components as ssb
 from dash import html
 
+from datadoc.frontend.fields.display_base import DATASET_METADATA_INPUT
 from datadoc.frontend.fields.display_base import VARIABLES_METADATA_INPUT
+from datadoc.frontend.fields.display_base import DatasetFieldTypes
 from datadoc.frontend.fields.display_base import VariablesFieldTypes
 
 if TYPE_CHECKING:
     from datadoc_model import model
 
 
 class AlertTypes(Enum):
@@ -47,24 +49,23 @@
     AlertTypes.SUCCESS: AlertType(
         alert_class_name="ssb-dialog",
         color="success",
     ),
 }
 
 
-def build_ssb_styled_tab(label: str, content: dbc.Container) -> dbc.Tab:
+def build_ssb_styled_tab(label: str, content: html.Article) -> dbc.Tab:
     """Make a Dash Tab according to SSBs Design System."""
     return dbc.Tab(
         label=label,
         # Replace all whitespace with dashes
         tab_id=re.sub(r"\s+", "-", label.lower()),
-        label_class_name="ssb-tabs navigation-item",
-        label_style={"marginLeft": "10px", "marginRight": "10px"},
-        style={"padding": "4px"},
+        label_class_name="ssb-tabs navigation-item workspace-tab-label",
         children=content,
+        className="workspace-tab",
     )
 
 
 def build_ssb_alert(  # noqa: PLR0913 not immediately obvious how to improve this
     alert_type: AlertTypes,
     alert_identifier: str,
     title: str,
@@ -91,77 +92,62 @@
                 children=message,
             ),
         ],
         style={"width": "70%"},
     )
 
 
-def build_ssb_button(text: str, icon_class: str, button_id: str) -> dbc.Button:
-    """Make a Dash Button according to SSBs Design System."""
-    return dbc.Button(
-        [
-            html.I(
-                className=icon_class,
-                style={"paddingRight": "10px"},
-            ),
-            f"   {text}",
-        ],
-        class_name="ssb-btn primary-btn",
-        id=button_id,
-    )
-
-
 def build_input_field_section(
     metadata_fields: list[VariablesFieldTypes],
     variable: model.Variable,
     language: str,
 ) -> dbc.Form:
-    """Create input fields."""
+    """Create form with input fields for variable workspace."""
     return dbc.Form(
         [
             i.render(
                 {
                     "type": VARIABLES_METADATA_INPUT,
                     "variable_short_name": variable.short_name,
                     "id": i.identifier,
                 },
                 language,
                 variable,
             )
             for i in metadata_fields
         ],
         id=VARIABLES_METADATA_INPUT,
-        className="variables-input-group",
+        className="edit-section-form",
     )
 
 
 def build_edit_section(
     metadata_inputs: list,
     title: str,
     variable: model.Variable,
     language: str,
 ) -> html.Section:
-    """Create input section."""
+    """Create input section for variable workspace."""
     return html.Section(
         id={"type": "edit-section", "title": title},
         children=[
-            ssb.Title(title, size=3, className="input-section-title"),
+            ssb.Title(title, size=3, className="edit-section-title"),
             build_input_field_section(metadata_inputs, variable, language),
         ],
-        className="input-section",
+        className="edit-section",
     )
 
 
 def build_ssb_accordion(
     header: str,
     key: dict,
     variable_short_name: str,
     children: list,
 ) -> ssb.Accordion:
-    """Build Accordion for one variable."""
+    """Build Accordion for one variable in variable workspace."""
     return ssb.Accordion(
         header=header,
         id=key,
         children=[
             html.Section(
                 id={
                     "type": "variable-input-alerts",
@@ -173,9 +159,41 @@
                 id={
                     "type": "variable-inputs",
                     "variable_short_name": variable_short_name,
                 },
                 children=children,
             ),
         ],
-        className="variable",
+        className="variable-accordion",
+    )
+
+
+def build_dataset_edit_section(
+    title: str,
+    metadata_inputs: list[DatasetFieldTypes],
+    language: str,
+    dataset: model.Dataset,
+    key: dict,
+) -> html.Section:
+    """Create edit section for dataset workspace."""
+    return html.Section(
+        id=key,
+        children=[
+            ssb.Title(title, size=3, className="edit-section-title"),
+            dbc.Form(
+                [
+                    i.render(
+                        {
+                            "type": DATASET_METADATA_INPUT,
+                            "id": i.identifier,
+                        },
+                        language,
+                        dataset,
+                    )
+                    for i in metadata_inputs
+                ],
+                id=f"{DATASET_METADATA_INPUT}-{title}",
+                className="edit-section-form",
+            ),
+        ],
+        className="edit-section dataset-edit-section",
     )
```

### Comparing `ssb_datadoc-0.8.1/src/datadoc/frontend/fields/display_base.py` & `ssb_datadoc-0.8.2/src/datadoc/frontend/fields/display_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Functionality common to displaying dataset and variables metadata."""
 
 from __future__ import annotations
 
 import logging
+import re
 import typing as t
 from dataclasses import dataclass
 from dataclasses import field
 from typing import TYPE_CHECKING
 from typing import Any
 
 import dash_bootstrap_components as dbc
@@ -26,47 +27,35 @@
     from datadoc_model.model import LanguageStringType
     from pydantic import BaseModel
 
     from datadoc.frontend.callbacks.utils import MetadataInputTypes
 
 logger = logging.getLogger(__name__)
 
+DATASET_METADATA_INPUT = "dataset-metadata-input"
 
 VARIABLES_METADATA_INPUT = "variables-metadata-input"
 VARIABLES_METADATA_DATE_INPUT = "variables-metadata-date-input"
-
-# Must be changed if new design
-INPUT_KWARGS = {
-    "debounce": True,
-    "style": {"width": "100%"},
-    "className": "ssb-input",
-}
+DATASET_METADATA_DATE_INPUT = "dataset-metadata-date-input"
 
 
 def get_enum_options_for_language(
     enum: Enum,
     language: SupportedLanguages,
 ) -> list[dict[str, str]]:
     """Generate the list of options based on the currently chosen language."""
-    return [
+    dropdown_options = [
         {
             "title": i.get_value_for_language(language),
             "id": i.name,
         }
         for i in get_language_strings_enum(enum)  # type: ignore [attr-defined]
     ]
-
-
-def input_kwargs_factory() -> dict[str, t.Any]:
-    """Initialize the field extra_kwargs.
-
-    We aren't allowed to directly assign a mutable type like a dict to
-    a dataclass field.
-    """
-    return INPUT_KWARGS
+    dropdown_options.insert(0, {"title": "", "id": ""})
+    return dropdown_options
 
 
 def empty_kwargs_factory() -> dict[str, t.Any]:
     """Initialize the field extra_kwargs.
 
     We aren't allowed to directly assign a mutable type like a dict to
     a dataclass field.
@@ -83,14 +72,37 @@
     """Get a metadata value from the model and cast to string."""
     value = get_standard_metadata(metadata, identifier)
     if value is None:
         return None
     return str(value)
 
 
+def get_date_metadata_and_stringify(metadata: BaseModel, identifier: str) -> str | None:
+    """Get a metadata date value from the model.
+
+    Handle converting datetime format to date format string.
+    """
+    value = get_standard_metadata(metadata, identifier)
+    if value is None:
+        return ""
+    logger.info("Date registered: %s", value)
+    date = str(value)
+    # Pattern for datetime without T, with space - used for variables
+    pattern = r"\d{4}-\d{2}-\d{2}\s\d{2}:\d{2}:\d{2}\+\d{2}:\d{2}"
+    if re.match(pattern, date):
+        convert_date_to_iso = date.replace(" ", "T")
+        logger.info("Date converted to iso format: %s", convert_date_to_iso)
+        convert_date_format = convert_date_to_iso[:10]
+        logger.info("Display date: %s", convert_date_format)
+        return convert_date_format
+    convert_value = date[:10]
+    logger.info("Display date: %s", convert_value)
+    return convert_value
+
+
 def get_multi_language_metadata(metadata: BaseModel, identifier: str) -> str | None:
     """Get a metadata value supporting multiple languages from the model."""
     value: LanguageStringType | None = getattr(metadata, identifier)
     if value is None:
         return value
     return str(getattr(value, state.current_metadata_language))
 
@@ -115,135 +127,110 @@
     obligatory: bool = False
     editable: bool = True
     url: bool = False
     multiple_language_support: bool = False
 
 
 @dataclass
-class DisplayDatasetMetadata(DisplayMetadata):
-    """Controls for how a given metadata field should be displayed.
-
-    Specific to dataset fields.
-    """
-
-    extra_kwargs: dict[str, Any] = field(default_factory=input_kwargs_factory)
-    component: type[Component] = dcc.Input
-    value_getter: Callable[[BaseModel, str], Any] = get_metadata_and_stringify
-
+class MetadataInputField(DisplayMetadata):
+    """Controls how a input field should be displayed."""
 
-@dataclass
-class DisplayDatasetMetadataDropdown(DisplayDatasetMetadata):
-    """Include the possible options which a user may choose from."""
-
-    # fmt: off
-    options_getter: Callable[[SupportedLanguages], list[dict[str, str]]] = lambda _: []  # noqa: E731
-    # fmt: on
-    extra_kwargs: dict[str, Any] = field(default_factory=empty_kwargs_factory)
-    component: type[Component] = dcc.Dropdown
-
-
-@dataclass
-class VariablesInputField(DisplayMetadata):
-    """Controls for how a given metadata field should be displayed.
-
-    Specific to variable fields.
-    """
-
-    extra_kwargs: dict[str, Any] = field(default_factory=empty_kwargs_factory)
-    value_getter: Callable[[BaseModel, str], Any] = get_metadata_and_stringify
     type: str = "text"
-
-    def render(
-        self,
-        variable_id: dict,
-        language: str,  # noqa: ARG002
-        variable: model.Variable,
-    ) -> ssb.Input:
-        """Build Input component."""
-        value = self.value_getter(variable, self.identifier)
-        return ssb.Input(
-            label=self.display_name,
-            id=variable_id,
-            debounce=True,
-            type=self.type,
-            disabled=not self.editable,
-            value=value,
-            className="variable-input",
-        )
-
-
-@dataclass
-class VariablesPeriodField(DisplayMetadata):
-    """Control how fields which define a time period are displayed.
-
-    These are a special case since two fields have a relationship to one another.>
-    """
-
     extra_kwargs: dict[str, Any] = field(default_factory=empty_kwargs_factory)
     value_getter: Callable[[BaseModel, str], Any] = get_metadata_and_stringify
-    type: str = "date"
 
     def render(
         self,
-        variable_id: dict,
-        language: str,  # noqa: ARG002
-        variable: model.Variable,
+        component_id: dict,
+        language: str,  # noqa: ARG002 Required by Dash
+        metadata: BaseModel,
     ) -> ssb.Input:
-        """Build Input date component."""
-        value = self.value_getter(variable, self.identifier)
-        variable_id["type"] = VARIABLES_METADATA_DATE_INPUT
+        """Build component."""
+        value = self.value_getter(metadata, self.identifier)
         return ssb.Input(
             label=self.display_name,
-            id=variable_id,
-            debounce=False,
+            id=component_id,
+            debounce=True,
             type=self.type,
             disabled=not self.editable,
             value=value,
-            className="variable-input",
+            className="input-component",
         )
 
 
 @dataclass
-class VariablesDropdownField(DisplayMetadata):
+class MetadataDropdownField(DisplayMetadata):
     """Control how a Dropdown should be displayed."""
 
     extra_kwargs: dict[str, Any] = field(default_factory=empty_kwargs_factory)
     value_getter: Callable[[BaseModel, str], Any] = get_metadata_and_stringify
     # fmt: off
     options_getter: Callable[[SupportedLanguages], list[dict[str, str]]] = lambda _: []  # noqa: E731
     # fmt: on
 
     def render(
         self,
-        variable_id: dict,
+        component_id: dict,
         language: str,
-        variable: model.Variable,
+        dataset: BaseModel,
     ) -> ssb.Dropdown:
         """Build Dropdown component."""
-        value = self.value_getter(variable, self.identifier)
+        value = self.value_getter(dataset, self.identifier)
         return ssb.Dropdown(
             header=self.display_name,
-            id=variable_id,
+            id=component_id,
             items=self.options_getter(SupportedLanguages(language)),
             value=value,
-            className="variable-dropdown",
+            className="dropdown-component",
         )
 
 
 @dataclass
-class VariablesCheckboxField(DisplayMetadata):
+class MetadataPeriodField(DisplayMetadata):
+    """Control how fields which define a time period are displayed for Dataset.
+
+    These are a special case since two fields have a relationship to one another.>
+    """
+
+    id_type: str = ""
+    extra_kwargs: dict[str, Any] = field(default_factory=empty_kwargs_factory)
+    value_getter: Callable[[BaseModel, str], Any] = get_date_metadata_and_stringify
+    type: str = "date"
+
+    def render(
+        self,
+        component_id: dict,
+        language: str,  # noqa: ARG002 Required by Dash
+        dataset: BaseModel,
+    ) -> ssb.Input:
+        """Build Input date component."""
+        value = self.value_getter(dataset, self.identifier)
+        component_id["type"] = self.id_type
+        return ssb.Input(
+            label=self.display_name,
+            id=component_id,
+            debounce=False,
+            type=self.type,
+            disabled=not self.editable,
+            value=value,
+            className="input-component",
+        )
+
+
+@dataclass
+class MetadataCheckboxField(DisplayMetadata):
     """Controls for how a checkbox metadata field should be displayed."""
 
-    extra_kwargs: dict[str, Any] = field(default_factory=input_kwargs_factory)
+    extra_kwargs: dict[str, Any] = field(default_factory=empty_kwargs_factory)
     value_getter: Callable[[BaseModel, str], Any] = get_standard_metadata
 
     def render(
         self,
         variable_id: dict,
-        language: str,  # noqa: ARG002
+        language: str,  # noqa: ARG002 Required by Dash
         variable: model.Variable,
     ) -> dbc.Checkbox:
         """Build Checkbox component."""
         value = self.value_getter(variable, self.identifier)
         return dbc.Checkbox(
             label=self.display_name,
             id=variable_id,
@@ -251,12 +238,37 @@
             label_class_name="ssb-checkbox checkbox-label",
             class_name="ssb-checkbox",
             value=value,
         )
 
 
 VariablesFieldTypes = (
-    VariablesInputField
-    | VariablesDropdownField
-    | VariablesCheckboxField
-    | VariablesPeriodField
+    MetadataInputField
+    | MetadataDropdownField
+    | MetadataCheckboxField
+    | MetadataPeriodField
 )
+
+DatasetFieldTypes = MetadataInputField | MetadataDropdownField | MetadataPeriodField
+
+
+@dataclass
+class DisplayDatasetMetadata(DisplayMetadata):
+    """Controls for how a given metadata field should be displayed.
+
+    Specific to dataset fields.
+    """
+
+    extra_kwargs: dict[str, Any] = field(default_factory=empty_kwargs_factory)
+    component: type[Component] = dcc.Input
+    value_getter: Callable[[BaseModel, str], Any] = get_metadata_and_stringify
+
+
+@dataclass
+class DisplayDatasetMetadataDropdown(DisplayDatasetMetadata):
+    """Include the possible options which a user may choose from."""
+
+    # fmt: off
+    options_getter: Callable[[SupportedLanguages], list[dict[str, str]]] = lambda _: []  # noqa: E731
+    # fmt: on
+    extra_kwargs: dict[str, Any] = field(default_factory=empty_kwargs_factory)
+    component: type[Component] = dcc.Dropdown
```

### Comparing `ssb_datadoc-0.8.1/src/datadoc/frontend/fields/display_dataset.py` & `ssb_datadoc-0.8.2/src/datadoc/frontend/fields/display_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,84 +3,77 @@
 from __future__ import annotations
 
 import functools
 import logging
 from enum import Enum
 from typing import TYPE_CHECKING
 
-from dash import dcc
-
 from datadoc import enums
 from datadoc import state
-from datadoc.frontend.callbacks.utils import get_language_strings_enum
-from datadoc.frontend.fields.display_base import INPUT_KWARGS
-from datadoc.frontend.fields.display_base import DisplayDatasetMetadata
+from datadoc.frontend.fields.display_base import DATASET_METADATA_DATE_INPUT
+from datadoc.frontend.fields.display_base import DatasetFieldTypes
 from datadoc.frontend.fields.display_base import DisplayDatasetMetadataDropdown
+from datadoc.frontend.fields.display_base import MetadataDropdownField
+from datadoc.frontend.fields.display_base import MetadataInputField
+from datadoc.frontend.fields.display_base import MetadataPeriodField
 from datadoc.frontend.fields.display_base import get_comma_separated_string
+from datadoc.frontend.fields.display_base import get_enum_options_for_language
 from datadoc.frontend.fields.display_base import get_metadata_and_stringify
 from datadoc.frontend.fields.display_base import get_multi_language_metadata
 
 if TYPE_CHECKING:
     from datadoc.enums import SupportedLanguages
 
 logger = logging.getLogger(__name__)
 
 
-def get_enum_options_for_language(
-    enum: Enum,
-    language: SupportedLanguages,
-) -> list[dict[str, str]]:
-    """Generate the list of options based on the currently chosen language."""
-    return [
-        {
-            "label": i.get_value_for_language(language),
-            "value": i.name,
-        }
-        for i in get_language_strings_enum(enum)  # type: ignore [attr-defined]
-    ]
-
-
 def get_statistical_subject_options(
     language: SupportedLanguages,
 ) -> list[dict[str, str]]:
-    """Collect the statistical subject options for the given language."""
-    return [
+    """Generate the list of options for statistical subject."""
+    dropdown_options = [
         {
-            "label": f"{primary.get_title(language)} - {secondary.get_title(language)}",
-            "value": secondary.subject_code,
+            "title": f"{primary.get_title(language)} - {secondary.get_title(language)}",
+            "id": secondary.subject_code,
         }
         for primary in state.statistic_subject_mapping.primary_subjects
         for secondary in primary.secondary_subjects
     ]
+    dropdown_options.insert(0, {"title": "", "id": ""})
+    return dropdown_options
 
 
 def get_unit_type_options(
     language: SupportedLanguages,
 ) -> list[dict[str, str]]:
     """Collect the unit type options for the given language."""
-    return [
+    dropdown_options = [
         {
-            "label": unit_type.get_title(language),
-            "value": unit_type.code,
+            "title": unit_type.get_title(language),
+            "id": unit_type.code,
         }
         for unit_type in state.unit_types.classifications
     ]
+    dropdown_options.insert(0, {"title": "", "id": ""})
+    return dropdown_options
 
 
 def get_owner_options(
     language: SupportedLanguages,
 ) -> list[dict[str, str]]:
     """Collect the owner options for the given language."""
-    return [
+    dropdown_options = [
         {
-            "label": f"{option.code} - {option.get_title(language)}",
-            "value": option.code,
+            "title": f"{option.code} - {option.get_title(language)}",
+            "id": option.code,
         }
         for option in state.organisational_units.classifications
     ]
+    dropdown_options.insert(0, {"title": "", "id": ""})
+    return dropdown_options
 
 
 class DatasetIdentifiers(str, Enum):
     """As defined here: https://statistics-norway.atlassian.net/l/c/aoSfEWJU."""
 
     SHORT_NAME = "short_name"
     ASSESSMENT = "assessment"
@@ -105,205 +98,212 @@
     METADATA_CREATED_BY = "metadata_created_by"
     METADATA_LAST_UPDATED_DATE = "metadata_last_updated_date"
     METADATA_LAST_UPDATED_BY = "metadata_last_updated_by"
     CONTAINS_DATA_FROM = "contains_data_from"
     CONTAINS_DATA_UNTIL = "contains_data_until"
 
 
-DISPLAY_DATASET: dict[DatasetIdentifiers, DisplayDatasetMetadata] = {
-    DatasetIdentifiers.SHORT_NAME: DisplayDatasetMetadata(
+DISPLAY_DATASET: dict[
+    DatasetIdentifiers,
+    DatasetFieldTypes,
+] = {
+    DatasetIdentifiers.SHORT_NAME: MetadataInputField(
         identifier=DatasetIdentifiers.SHORT_NAME.value,
         display_name="Kortnavn",
         description="Navn på (fysisk) datafil, datatabell eller datasett",
-        component=dcc.Input,
         obligatory=True,
         editable=False,
     ),
-    DatasetIdentifiers.ASSESSMENT: DisplayDatasetMetadataDropdown(
+    DatasetIdentifiers.ASSESSMENT: MetadataDropdownField(
         identifier=DatasetIdentifiers.ASSESSMENT.value,
         display_name="Verdivurdering",
         description="Verdivurdering (sensitivitetsklassifisering) for datasettet.",
         options_getter=functools.partial(
             get_enum_options_for_language,
             enums.Assessment,
         ),
     ),
-    DatasetIdentifiers.DATASET_STATUS: DisplayDatasetMetadataDropdown(
+    DatasetIdentifiers.DATASET_STATUS: MetadataDropdownField(
         identifier=DatasetIdentifiers.DATASET_STATUS.value,
         display_name="Status",
         description="Livssyklus for datasettet",
         options_getter=functools.partial(
             get_enum_options_for_language,
             enums.DataSetStatus,
         ),
         obligatory=True,
     ),
-    DatasetIdentifiers.DATASET_STATE: DisplayDatasetMetadataDropdown(
+    DatasetIdentifiers.DATASET_STATE: MetadataDropdownField(
         identifier=DatasetIdentifiers.DATASET_STATE.value,
         display_name="Datatilstand",
         description="Datatilstand. Se Intern dokument 2021- 17  Datatilstander i SSB",
         obligatory=True,
         options_getter=functools.partial(
             get_enum_options_for_language,
             enums.DataSetState,
         ),
     ),
-    DatasetIdentifiers.NAME: DisplayDatasetMetadata(
+    DatasetIdentifiers.NAME: MetadataInputField(
         identifier=DatasetIdentifiers.NAME.value,
         display_name="Navn",
         description="Datasettnavn",
         obligatory=True,
         multiple_language_support=True,
+        value_getter=get_metadata_and_stringify,
     ),
-    DatasetIdentifiers.DATA_SOURCE: DisplayDatasetMetadata(
+    DatasetIdentifiers.DATA_SOURCE: MetadataInputField(
         identifier=DatasetIdentifiers.DATA_SOURCE.value,
         display_name="Datakilde",
         description="Datakilde. Settes enten for datasettet eller variabelforekomst.",
         obligatory=True,
         multiple_language_support=True,
     ),
-    DatasetIdentifiers.REGISTER_URI: DisplayDatasetMetadata(
+    DatasetIdentifiers.REGISTER_URI: MetadataInputField(
         identifier=DatasetIdentifiers.REGISTER_URI.value,
         display_name="Register URI",
         description="Lenke (URI) til register i registeroversikt (oversikt over alle registre meldt Datatilsynet (oppdatering foretas av sikkerhetsrådgiver))",
         multiple_language_support=True,
+        url=True,
+        type="url",
     ),
-    DatasetIdentifiers.POPULATION_DESCRIPTION: DisplayDatasetMetadata(
+    DatasetIdentifiers.POPULATION_DESCRIPTION: MetadataInputField(
         identifier=DatasetIdentifiers.POPULATION_DESCRIPTION.value,
         display_name="Populasjon",
         description="Populasjonen datasettet dekker. Populasjonsbeskrivelsen inkluderer enhetstype, geografisk dekningsområde og tidsperiode.",
         obligatory=True,
         multiple_language_support=True,
     ),
-    DatasetIdentifiers.VERSION: DisplayDatasetMetadata(
+    DatasetIdentifiers.VERSION: MetadataInputField(
         identifier=DatasetIdentifiers.VERSION.value,
         display_name="Versjon",
         description="Versjon",
-        extra_kwargs=dict(type="number", min=1, **INPUT_KWARGS),
+        extra_kwargs={"type": "number", "min": 1},
         obligatory=True,
     ),
-    DatasetIdentifiers.VERSION_DESCRIPTION: DisplayDatasetMetadata(
+    DatasetIdentifiers.VERSION_DESCRIPTION: MetadataInputField(
         identifier=DatasetIdentifiers.VERSION_DESCRIPTION.value,
         display_name="Versjonsbeskrivelse",
         description="Årsak/grunnlag for denne versjonen av datasettet i form av beskrivende tekst.",
         multiple_language_support=True,
         obligatory=True,
     ),
-    DatasetIdentifiers.UNIT_TYPE: DisplayDatasetMetadataDropdown(
+    DatasetIdentifiers.UNIT_TYPE: MetadataDropdownField(
         identifier=DatasetIdentifiers.UNIT_TYPE.value,
         display_name="Enhetstype",
         description="Primær enhetstype for datafil, datatabell eller datasett. Se  Vi jobber med en avklaring av behov for flere enhetstyper her.",
         multiple_language_support=False,
         options_getter=get_unit_type_options,
         obligatory=True,
     ),
-    DatasetIdentifiers.TEMPORALITY_TYPE: DisplayDatasetMetadataDropdown(
+    DatasetIdentifiers.TEMPORALITY_TYPE: MetadataDropdownField(
         identifier=DatasetIdentifiers.TEMPORALITY_TYPE.value,
         display_name="Temporalitetstype",
         description="Temporalitetstype. Settes enten for variabelforekomst eller datasett. Se Temporalitet, hendelser og forløp.",
         options_getter=functools.partial(
             get_enum_options_for_language,
             enums.TemporalityTypeType,
         ),
         obligatory=True,
     ),
-    DatasetIdentifiers.DESCRIPTION: DisplayDatasetMetadata(
+    DatasetIdentifiers.DESCRIPTION: MetadataInputField(
         identifier=DatasetIdentifiers.DESCRIPTION.value,
         display_name="Beskrivelse",
         description="Beskrivelse av datasettet",
         multiple_language_support=True,
         obligatory=True,
     ),
-    DatasetIdentifiers.SUBJECT_FIELD: DisplayDatasetMetadataDropdown(
+    DatasetIdentifiers.SUBJECT_FIELD: MetadataDropdownField(
         identifier=DatasetIdentifiers.SUBJECT_FIELD.value,
         display_name="Statistikkområde",
         description="Primær statistikkområdet som datasettet inngår i",
         obligatory=True,
         # TODO @mmwinther: Remove multiple_language_support once the model is updated.
         # https://github.com/statisticsnorway/ssb-datadoc-model/issues/41
         multiple_language_support=True,
         options_getter=get_statistical_subject_options,
     ),
-    DatasetIdentifiers.KEYWORD: DisplayDatasetMetadata(
+    DatasetIdentifiers.KEYWORD: MetadataInputField(
         identifier=DatasetIdentifiers.KEYWORD.value,
         display_name="Nøkkelord",
         description="En kommaseparert liste med søkbare nøkkelord som kan bidra til utvikling av effektive filtrerings- og søketjeneste.",
         value_getter=get_comma_separated_string,
     ),
-    DatasetIdentifiers.SPATIAL_COVERAGE_DESCRIPTION: DisplayDatasetMetadata(
+    DatasetIdentifiers.SPATIAL_COVERAGE_DESCRIPTION: MetadataInputField(
         identifier=DatasetIdentifiers.SPATIAL_COVERAGE_DESCRIPTION.value,
         display_name="Geografisk dekningsområde",
         description="Beskrivelse av datasettets geografiske dekningsområde. Målet er på sikt at dette skal hentes fra Klass, men fritekst vil også kunne brukes.",
         multiple_language_support=True,
     ),
-    DatasetIdentifiers.ID: DisplayDatasetMetadata(
+    DatasetIdentifiers.ID: MetadataInputField(
         identifier=DatasetIdentifiers.ID.value,
         display_name="ID",
         description="Unik SSB-identifikator for datasettet (løpenummer)",
         obligatory=True,
         editable=False,
         value_getter=get_metadata_and_stringify,
     ),
-    DatasetIdentifiers.OWNER: DisplayDatasetMetadataDropdown(
+    DatasetIdentifiers.OWNER: MetadataDropdownField(
         identifier=DatasetIdentifiers.OWNER.value,
         display_name="Eier",
         description="Maskingenerert seksjonstilhørighet til den som oppretter metadata om datasettet, men kan korrigeres manuelt",
         obligatory=True,
         editable=True,
         multiple_language_support=False,
         options_getter=get_owner_options,
     ),
-    DatasetIdentifiers.FILE_PATH: DisplayDatasetMetadata(
+    DatasetIdentifiers.FILE_PATH: MetadataInputField(
         identifier=DatasetIdentifiers.FILE_PATH.value,
         display_name="Filsti",
         description="Filstien inneholder datasettets navn og stien til hvor det er lagret.",
         obligatory=True,
         editable=False,
     ),
-    DatasetIdentifiers.METADATA_CREATED_DATE: DisplayDatasetMetadata(
+    DatasetIdentifiers.METADATA_CREATED_DATE: MetadataInputField(
         identifier=DatasetIdentifiers.METADATA_CREATED_DATE.value,
         display_name="Dato opprettet",
         description="Opprettet dato for metadata om datasettet",
         obligatory=True,
         editable=False,
     ),
-    DatasetIdentifiers.METADATA_CREATED_BY: DisplayDatasetMetadata(
+    DatasetIdentifiers.METADATA_CREATED_BY: MetadataInputField(
         identifier=DatasetIdentifiers.METADATA_CREATED_BY.value,
         display_name="Opprettet av",
         description="Opprettet av person. Kun til bruk i SSB.",
         obligatory=True,
         editable=False,
     ),
-    DatasetIdentifiers.METADATA_LAST_UPDATED_DATE: DisplayDatasetMetadata(
+    DatasetIdentifiers.METADATA_LAST_UPDATED_DATE: MetadataInputField(
         identifier=DatasetIdentifiers.METADATA_LAST_UPDATED_DATE.value,
         display_name="Dato oppdatert",
         description="Sist oppdatert dato for metadata om datasettet",
         obligatory=True,
         editable=False,
     ),
-    DatasetIdentifiers.METADATA_LAST_UPDATED_BY: DisplayDatasetMetadata(
+    DatasetIdentifiers.METADATA_LAST_UPDATED_BY: MetadataInputField(
         identifier=DatasetIdentifiers.METADATA_LAST_UPDATED_BY.value,
         display_name="Oppdatert av",
         description="Siste endring utført av person. Kun til bruk i SSB.",
         obligatory=True,
         editable=False,
     ),
-    DatasetIdentifiers.CONTAINS_DATA_FROM: DisplayDatasetMetadata(
+    DatasetIdentifiers.CONTAINS_DATA_FROM: MetadataPeriodField(
         identifier=DatasetIdentifiers.CONTAINS_DATA_FROM.value,
         display_name="Inneholder data f.o.m.",
         description="ÅÅÅÅ-MM-DD",
         obligatory=True,
         editable=True,
+        id_type=DATASET_METADATA_DATE_INPUT,
     ),
-    DatasetIdentifiers.CONTAINS_DATA_UNTIL: DisplayDatasetMetadata(
+    DatasetIdentifiers.CONTAINS_DATA_UNTIL: MetadataPeriodField(
         identifier=DatasetIdentifiers.CONTAINS_DATA_UNTIL.value,
         display_name="Inneholder data t.o.m.",
         description="ÅÅÅÅ-MM-DD",
         obligatory=True,
         editable=True,
+        id_type=DATASET_METADATA_DATE_INPUT,
     ),
 }
 
 for v in DISPLAY_DATASET.values():
     if v.multiple_language_support:
         v.value_getter = get_multi_language_metadata
 
@@ -319,15 +319,15 @@
     m for m in DISPLAY_DATASET.values() if not m.obligatory and m.editable
 ]
 
 NON_EDITABLE_DATASET_METADATA = [m for m in DISPLAY_DATASET.values() if not m.editable]
 
 
 # The order of this list MUST match the order of display components, as defined in DatasetTab.py
-DISPLAYED_DATASET_METADATA: list[DisplayDatasetMetadata] = (
+DISPLAYED_DATASET_METADATA: list[DatasetFieldTypes] = (
     OBLIGATORY_EDITABLE_DATASET_METADATA
     + OPTIONAL_DATASET_METADATA
     + NON_EDITABLE_DATASET_METADATA
 )
 
 DISPLAYED_DROPDOWN_DATASET_METADATA: list[DisplayDatasetMetadataDropdown] = [
     m
```

### Comparing `ssb_datadoc-0.8.1/src/datadoc/frontend/fields/display_variables.py` & `ssb_datadoc-0.8.2/src/datadoc/frontend/fields/display_variables.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 
 from __future__ import annotations
 
 import functools
 from enum import Enum
 
 from datadoc import enums
-from datadoc.frontend.fields.display_base import VariablesCheckboxField
-from datadoc.frontend.fields.display_base import VariablesDropdownField
+from datadoc.frontend.fields.display_base import VARIABLES_METADATA_DATE_INPUT
+from datadoc.frontend.fields.display_base import MetadataCheckboxField
+from datadoc.frontend.fields.display_base import MetadataDropdownField
+from datadoc.frontend.fields.display_base import MetadataInputField
+from datadoc.frontend.fields.display_base import MetadataPeriodField
 from datadoc.frontend.fields.display_base import VariablesFieldTypes
-from datadoc.frontend.fields.display_base import VariablesInputField
-from datadoc.frontend.fields.display_base import VariablesPeriodField
 from datadoc.frontend.fields.display_base import get_enum_options_for_language
 from datadoc.frontend.fields.display_base import get_multi_language_metadata
 
 
 class VariableIdentifiers(str, Enum):
     """As defined here: https://statistics-norway.atlassian.net/wiki/spaces/MPD/pages/3042869256/Variabelforekomst."""
 
@@ -38,139 +39,141 @@
     CONTAINS_DATA_UNTIL = "contains_data_until"
 
 
 DISPLAY_VARIABLES: dict[
     VariableIdentifiers,
     VariablesFieldTypes,
 ] = {
-    VariableIdentifiers.SHORT_NAME: VariablesInputField(
+    VariableIdentifiers.SHORT_NAME: MetadataInputField(
         identifier=VariableIdentifiers.SHORT_NAME.value,
         display_name="Kortnavn",
         description="Fysisk navn på variabelen i datasettet. Bør tilsvare anbefalt kortnavn.",
         obligatory=True,
         editable=False,
     ),
-    VariableIdentifiers.NAME: VariablesInputField(
+    VariableIdentifiers.NAME: MetadataInputField(
         identifier=VariableIdentifiers.NAME.value,
         display_name="Navn",
         description="Variabelnavn kan arves fra VarDef, men kan også dokumenteres/endres her.",
         obligatory=True,
         multiple_language_support=True,
         type="text",
     ),
-    VariableIdentifiers.DATA_TYPE: VariablesDropdownField(
+    VariableIdentifiers.DATA_TYPE: MetadataDropdownField(
         identifier=VariableIdentifiers.DATA_TYPE.value,
         display_name="Datatype",
         description="Datatype",
         obligatory=True,
         options_getter=functools.partial(
             get_enum_options_for_language,
             enums.DataType,
         ),
     ),
-    VariableIdentifiers.VARIABLE_ROLE: VariablesDropdownField(
+    VariableIdentifiers.VARIABLE_ROLE: MetadataDropdownField(
         identifier=VariableIdentifiers.VARIABLE_ROLE.value,
         display_name="Variabelens rolle",
         description="Variabelens rolle i datasett",
         obligatory=True,
         options_getter=functools.partial(
             get_enum_options_for_language,
             enums.VariableRole,
         ),
     ),
-    VariableIdentifiers.DEFINITION_URI: VariablesInputField(
+    VariableIdentifiers.DEFINITION_URI: MetadataInputField(
         identifier=VariableIdentifiers.DEFINITION_URI.value,
         display_name="Definition URI",
         description="En lenke (URI) til variabelens definisjon i SSB (Vardok/VarDef)",
         url=True,
         obligatory=True,
         type="url",
     ),
-    VariableIdentifiers.DIRECT_PERSON_IDENTIFYING: VariablesCheckboxField(
+    VariableIdentifiers.DIRECT_PERSON_IDENTIFYING: MetadataCheckboxField(
         identifier=VariableIdentifiers.DIRECT_PERSON_IDENTIFYING.value,
         display_name="Direkte personidentifiserende informasjon",
         description="Direkte personidentifiserende informasjon (DPI)",
         obligatory=True,
     ),
-    VariableIdentifiers.DATA_SOURCE: VariablesInputField(
+    VariableIdentifiers.DATA_SOURCE: MetadataInputField(
         identifier=VariableIdentifiers.DATA_SOURCE.value,
         display_name="Datakilde",
         description="Datakilde. Settes på datasettnivå, men kan overstyres på variabelforekomstnivå.",
         multiple_language_support=True,
         type="text",
     ),
-    VariableIdentifiers.POPULATION_DESCRIPTION: VariablesInputField(
+    VariableIdentifiers.POPULATION_DESCRIPTION: MetadataInputField(
         identifier=VariableIdentifiers.POPULATION_DESCRIPTION.value,
         display_name="Populasjonen",
         description="Populasjonen variabelen beskriver kan spesifiseres nærmere her. Settes på datasettnivå, men kan overstyres på variabelforekomstnivå.",
         multiple_language_support=True,
         type="text",
     ),
-    VariableIdentifiers.COMMENT: VariablesInputField(
+    VariableIdentifiers.COMMENT: MetadataInputField(
         identifier=VariableIdentifiers.COMMENT.value,
         display_name="Kommentar",
         description="Ytterligere presiseringer av variabeldefinisjon",
         multiple_language_support=True,
         type="text",
     ),
-    VariableIdentifiers.TEMPORALITY_TYPE: VariablesDropdownField(
+    VariableIdentifiers.TEMPORALITY_TYPE: MetadataDropdownField(
         identifier=VariableIdentifiers.TEMPORALITY_TYPE.value,
         display_name="Temporalitetstype",
         description="Temporalitetstype. Settes enten for variabelforekomst eller datasett. Se Temporalitet, hendelser og forløp.",
         options_getter=functools.partial(
             get_enum_options_for_language,
             enums.TemporalityTypeType,
         ),
     ),
-    VariableIdentifiers.MEASUREMENT_UNIT: VariablesInputField(
+    VariableIdentifiers.MEASUREMENT_UNIT: MetadataInputField(
         identifier=VariableIdentifiers.MEASUREMENT_UNIT.value,
         display_name="Måleenhet",
         description="Måleenhet. Eksempel: NOK eller USD for valuta, KG eller TONN for vekt. Se også forslag til SSBs måletyper/måleenheter.",
         type="text",
     ),
-    VariableIdentifiers.FORMAT: VariablesInputField(
+    VariableIdentifiers.FORMAT: MetadataInputField(
         identifier=VariableIdentifiers.FORMAT.value,
         display_name="Format",
         description="Verdienes format (fysisk format eller regulært uttrykk) i maskinlesbar form ifm validering. Dette kan benyttes som en ytterligere presisering av datatypen (dataType) i de tilfellene hvor dette er relevant. ",
     ),
-    VariableIdentifiers.CLASSIFICATION_URI: VariablesInputField(
+    VariableIdentifiers.CLASSIFICATION_URI: MetadataInputField(
         identifier=VariableIdentifiers.CLASSIFICATION_URI.value,
         display_name="Kodeverkets URI",
         description="Lenke (URI) til gyldige kodeverk (klassifikasjon eller kodeliste) i KLASS",
         url=True,
         type="url",
     ),
-    VariableIdentifiers.SENTINEL_VALUE_URI: VariablesInputField(
+    VariableIdentifiers.SENTINEL_VALUE_URI: MetadataInputField(
         identifier=VariableIdentifiers.SENTINEL_VALUE_URI.value,
         display_name="Spesialverdienes URI",
         description="En lenke (URI) til en oversikt over 'spesialverdier' som inngår i variabelen.",
         url=True,
         type="url",
     ),
-    VariableIdentifiers.INVALID_VALUE_DESCRIPTION: VariablesInputField(
+    VariableIdentifiers.INVALID_VALUE_DESCRIPTION: MetadataInputField(
         identifier=VariableIdentifiers.INVALID_VALUE_DESCRIPTION.value,
         display_name="Ugyldige verdier",
         description="En beskrivelse av ugyldige verdier som inngår i variabelen dersom spesialverdiene ikke er tilstrekkelige eller ikke kan benyttes.",
         multiple_language_support=True,
     ),
-    VariableIdentifiers.IDENTIFIER: VariablesInputField(
+    VariableIdentifiers.IDENTIFIER: MetadataInputField(
         identifier=VariableIdentifiers.IDENTIFIER.value,
         display_name="ID",
         description="Unik SSB identifikator for variabelforekomsten i datasettet",
         editable=False,
     ),
-    VariableIdentifiers.CONTAINS_DATA_FROM: VariablesPeriodField(
+    VariableIdentifiers.CONTAINS_DATA_FROM: MetadataPeriodField(
         identifier=VariableIdentifiers.CONTAINS_DATA_FROM.value,
         display_name="Inneholder data f.o.m.",
         description="Variabelforekomsten i datasettet inneholder data fra og med denne dato.",
+        id_type=VARIABLES_METADATA_DATE_INPUT,
     ),
-    VariableIdentifiers.CONTAINS_DATA_UNTIL: VariablesPeriodField(
+    VariableIdentifiers.CONTAINS_DATA_UNTIL: MetadataPeriodField(
         identifier=VariableIdentifiers.CONTAINS_DATA_UNTIL.value,
         display_name="Inneholder data t.o.m.",
         description="Variabelforekomsten i datasettet inneholder data til og med denne dato.",
+        id_type=VARIABLES_METADATA_DATE_INPUT,
     ),
 }
 
 MULTIPLE_LANGUAGE_VARIABLES_METADATA = [
     m.identifier for m in DISPLAY_VARIABLES.values() if m.multiple_language_support
 ]
```

### Comparing `ssb_datadoc-0.8.1/src/datadoc/logging/json_formatter.py` & `ssb_datadoc-0.8.2/src/datadoc/logging_configuration/json_formatter.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.1/src/datadoc/logging/logging_config.py` & `ssb_datadoc-0.8.2/src/datadoc/logging_configuration/logging_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             "formatters": {
                 "simple": {
                     "format": "%(asctime)s.%(msecs)03d %(levelname)s %(name)s: %(message)s",
                     "logger": "name",
                     "datefmt": "%Y-%m-%d %H:%M:%S",
                 },
                 "json": {
-                    "()": "datadoc.logging.json_formatter.DatadocJSONFormatter",
+                    "()": "datadoc.logging_configuration.json_formatter.DatadocJSONFormatter",
                     "fmt_keys": {
                         "level": "levelname",
                         "message": "message",
                         "timestamp": "timestamp",
                         "logger": "name",
                         "module": "module",
                         "function": "funcName",
```

### Comparing `ssb_datadoc-0.8.1/src/datadoc/state.py` & `ssb_datadoc-0.8.2/src/datadoc/state.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.1/src/datadoc/utils.py` & `ssb_datadoc-0.8.2/src/datadoc/utils.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.1/PKG-INFO` & `ssb_datadoc-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-datadoc
-Version: 0.8.1
+Version: 0.8.2
 Summary: Document dataset metadata. For use in Statistics Norway's metadata system.
 Home-page: https://github.com/statisticsnorway/datadoc
 License: MIT
 Author: Statistics Norway
 Author-email: stat-dev@ssb.no
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

