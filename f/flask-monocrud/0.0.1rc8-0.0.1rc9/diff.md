# Comparing `tmp/flask-monocrud-0.0.1rc8.tar.gz` & `tmp/flask-monocrud-0.0.1rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-monocrud-0.0.1rc8.tar", last modified: Mon Mar 18 21:34:53 2024, max compression
+gzip compressed data, was "flask-monocrud-0.0.1rc9.tar", last modified: Mon Mar 18 21:38:32 2024, max compression
```

## Comparing `flask-monocrud-0.0.1rc8.tar` & `flask-monocrud-0.0.1rc9.tar`

### file list

```diff
@@ -1,140 +1,151 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.923745 flask-monocrud-0.0.1rc8/
--rw-rw-rw-   0        0        0      253 2024-03-18 21:34:40.000000 flask-monocrud-0.0.1rc8/MANIFEST.in
--rw-rw-rw-   0        0        0     6805 2024-03-18 21:34:53.916746 flask-monocrud-0.0.1rc8/PKG-INFO
--rw-rw-rw-   0        0        0     6014 2024-03-18 19:50:13.000000 flask-monocrud-0.0.1rc8/README.md
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.799747 flask-monocrud-0.0.1rc8/flask_monocrud/
--rw-rw-rw-   0        0        0     4377 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/AdminModel.py
--rw-rw-rw-   0        0        0     2182 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/QueryHandler.py
--rw-rw-rw-   0        0        0    16068 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.804746 flask-monocrud-0.0.1rc8/flask_monocrud/action_components/
--rw-rw-rw-   0        0        0     1733 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/action_components/__init__.py
--rw-rw-rw-   0        0        0    14960 2024-03-18 21:16:25.000000 flask-monocrud-0.0.1rc8/flask_monocrud/ext.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.809747 flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/
--rw-rw-rw-   0        0        0    10046 2024-03-18 20:07:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/__init__.py
--rw-rw-rw-   0        0        0      141 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/compat.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.819746 flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/panels/
--rw-rw-rw-   0        0        0     1524 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/panels/__init__.py
--rw-rw-rw-   0        0        0      622 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/panels/config_vars.py
--rw-rw-rw-   0        0        0      565 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/panels/g.py
--rw-rw-rw-   0        0        0     1332 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/panels/headers.py
--rw-rw-rw-   0        0        0     3294 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/panels/logger.py
--rw-rw-rw-   0        0        0     3650 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/panels/profiler.py
--rw-rw-rw-   0        0        0     1755 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/panels/request_vars.py
--rw-rw-rw-   0        0        0      890 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/panels/route_list.py
--rw-rw-rw-   0        0        0     4244 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/panels/sqlalchemy.py
--rw-rw-rw-   0        0        0     5181 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/panels/template.py
--rw-rw-rw-   0        0        0     3290 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/panels/timer.py
--rw-rw-rw-   0        0        0     1274 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/panels/versions.py
--rw-rw-rw-   0        0        0     2161 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/toolbar.py
--rw-rw-rw-   0        0        0     2736 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/utils.py
--rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/flask_monocrud.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.831746 flask-monocrud-0.0.1rc8/flask_monocrud/form_components/
--rw-rw-rw-   0        0        0      281 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/form_components/__init__.py
--rw-rw-rw-   0        0        0      800 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/form_components/checkbox.py
--rw-rw-rw-   0        0        0     1654 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/form_components/field.py
--rw-rw-rw-   0        0        0      432 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/form_components/file_upload.py
--rw-rw-rw-   0        0        0      855 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/form_components/grid.py
--rw-rw-rw-   0        0        0       68 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/form_components/guard.py
--rw-rw-rw-   0        0        0      784 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/form_components/horizontal_separator.py
--rw-rw-rw-   0        0        0      353 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/form_components/radio.py
--rw-rw-rw-   0        0        0     2992 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/form_components/repeater.py
--rw-rw-rw-   0        0        0      944 2024-03-16 20:01:15.000000 flask-monocrud-0.0.1rc8/flask_monocrud/form_components/select.py
--rw-rw-rw-   0        0        0     1879 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/form_components/text_area.py
--rw-rw-rw-   0        0        0     3165 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/form_components/text_input.py
--rw-rw-rw-   0        0        0      398 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/form_components/toggle.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.836746 flask-monocrud-0.0.1rc8/flask_monocrud/helpers/
--rw-rw-rw-   0        0        0     1330 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/helpers/Dater.py
--rw-rw-rw-   0        0        0     1641 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/helpers/__init__.py
--rw-rw-rw-   0        0        0     1079 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/helpers/get_by_dot.py
--rw-rw-rw-   0        0        0       53 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/helpers/get_type.py
--rw-rw-rw-   0        0        0      143 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/helpers/optional.py
--rw-rw-rw-   0        0        0      336 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/helpers/to_class.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.836746 flask-monocrud-0.0.1rc8/flask_monocrud/live_component/
--rw-rw-rw-   0        0        0      410 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/live_component/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.838746 flask-monocrud-0.0.1rc8/flask_monocrud/metrics/
--rw-rw-rw-   0        0        0       26 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/metrics/__init__.py
--rw-rw-rw-   0        0        0     1170 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/metrics/metric.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.840745 flask-monocrud-0.0.1rc8/flask_monocrud/notification_component/
--rw-rw-rw-   0        0        0       38 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/notification_component/__init__.py
--rw-rw-rw-   0        0        0     2315 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/notification_component/notification.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.841747 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/
--rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.842746 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/application/
--rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/application/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.842746 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/application/admin/
--rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/application/admin/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.843747 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/application/casts/
--rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/application/casts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.844746 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/application/events/
--rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/application/events/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.845747 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/application/hooks/
--rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/application/hooks/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.845747 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/application/models/
--rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/application/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.846747 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/application/observers/
--rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/application/observers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.847747 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/application/policies/
--rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/application/policies/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.848746 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/application/providers/
--rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/application/providers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.848746 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/application/scopes/
--rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/application/scopes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.849748 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/application/services/
--rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/application/services/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.851746 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/application/traits/
--rw-rw-rw-   0        0        0     3498 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/application/traits/EnhancedModelTrait.py
--rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/application/traits/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.852748 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/config/
--rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/config/__init__.py
--rw-rw-rw-   0        0        0      461 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/config/database.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.853747 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/databases/
--rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/databases/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.854746 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/databases/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/databases/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.855746 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/pages/
--rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/pages/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.855746 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/pages/admin/
--rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/pages/admin/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.856747 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/static/
--rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/static/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.857747 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/templates/
--rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.858745 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/uploads/
--rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/uploads/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.860746 flask-monocrud-0.0.1rc8/flask_monocrud/relations/
--rw-rw-rw-   0        0        0       30 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/relations/__init__.py
--rw-rw-rw-   0        0        0     1071 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/relations/relation.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.872747 flask-monocrud-0.0.1rc8/flask_monocrud/stubs/
--rw-rw-rw-   0        0        0      191 2024-03-18 21:23:59.000000 flask-monocrud-0.0.1rc8/flask_monocrud/stubs/create-view.stub
--rw-rw-rw-   0        0        0      193 2024-03-18 21:23:59.000000 flask-monocrud-0.0.1rc8/flask_monocrud/stubs/edit-view.stub
--rw-rw-rw-   0        0        0      184 2024-03-18 21:23:59.000000 flask-monocrud-0.0.1rc8/flask_monocrud/stubs/list-view.stub
--rw-rw-rw-   0        0        0      461 2024-03-18 21:23:59.000000 flask-monocrud-0.0.1rc8/flask_monocrud/stubs/migration.stub
--rw-rw-rw-   0        0        0      199 2024-03-18 21:23:59.000000 flask-monocrud-0.0.1rc8/flask_monocrud/stubs/preview-view.stub
--rw-rw-rw-   0        0        0     1156 2024-03-18 21:23:59.000000 flask-monocrud-0.0.1rc8/flask_monocrud/stubs/resource-admin.stub
--rw-rw-rw-   0        0        0      374 2024-03-18 21:27:39.000000 flask-monocrud-0.0.1rc8/flask_monocrud/stubs/resource-hooks.stub
--rw-rw-rw-   0        0        0      346 2024-03-18 21:23:59.000000 flask-monocrud-0.0.1rc8/flask_monocrud/stubs/resource-model.stub
--rw-rw-rw-   0        0        0      352 2024-03-18 21:27:11.000000 flask-monocrud-0.0.1rc8/flask_monocrud/stubs/resource-policies.stub
--rw-rw-rw-   0        0        0      276 2024-03-18 21:23:59.000000 flask-monocrud-0.0.1rc8/flask_monocrud/stubs/submit-create.stub
--rw-rw-rw-   0        0        0      237 2024-03-18 21:23:59.000000 flask-monocrud-0.0.1rc8/flask_monocrud/stubs/submit-delete.stub
--rw-rw-rw-   0        0        0      271 2024-03-18 21:23:59.000000 flask-monocrud-0.0.1rc8/flask_monocrud/stubs/submit-edit.stub
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.874746 flask-monocrud-0.0.1rc8/flask_monocrud/table_components/
--rw-rw-rw-   0        0        0      260 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/table_components/__init__.py
--rw-rw-rw-   0        0        0     1319 2024-03-15 04:58:50.000000 flask-monocrud-0.0.1rc8/flask_monocrud/table_components/table.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.875746 flask-monocrud-0.0.1rc8/flask_monocrud/templates/
--rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.881746 flask-monocrud-0.0.1rc8/flask_monocrud/templates/admin/
--rw-rw-rw-   0        0        0      113 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/templates/admin/Page.html
--rw-rw-rw-   0        0        0     2176 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc8/flask_monocrud/templates/admin/index.html
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.908747 flask-monocrud-0.0.1rc8/flask_monocrud/templates/admin/views/
--rw-rw-rw-   0        0        0      980 2024-03-17 01:41:49.000000 flask-monocrud-0.0.1rc8/flask_monocrud/templates/admin/views/CreateView.html
--rw-rw-rw-   0        0        0    17166 2024-03-17 17:12:18.000000 flask-monocrud-0.0.1rc8/flask_monocrud/templates/admin/views/EditView.html
--rw-rw-rw-   0        0        0    19310 2024-03-17 01:34:28.000000 flask-monocrud-0.0.1rc8/flask_monocrud/templates/admin/views/ListView.html
--rw-rw-rw-   0        0        0     1241 2024-03-17 17:25:03.000000 flask-monocrud-0.0.1rc8/flask_monocrud/templates/admin/views/PreviewView.html
-drwxrwxrwx   0        0        0        0 2024-03-18 21:34:53.803746 flask-monocrud-0.0.1rc8/flask_monocrud.egg-info/
--rw-rw-rw-   0        0        0     6805 2024-03-18 21:34:53.000000 flask-monocrud-0.0.1rc8/flask_monocrud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4539 2024-03-18 21:34:53.000000 flask-monocrud-0.0.1rc8/flask_monocrud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 21:34:53.000000 flask-monocrud-0.0.1rc8/flask_monocrud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2024-03-18 21:34:53.000000 flask-monocrud-0.0.1rc8/flask_monocrud.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-03-18 21:34:53.000000 flask-monocrud-0.0.1rc8/flask_monocrud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-18 21:34:53.923745 flask-monocrud-0.0.1rc8/setup.cfg
--rw-rw-rw-   0        0        0     1069 2024-03-18 21:34:49.000000 flask-monocrud-0.0.1rc8/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.565490 flask-monocrud-0.0.1rc9/
+-rw-rw-rw-   0        0        0      253 2024-03-18 21:34:40.000000 flask-monocrud-0.0.1rc9/MANIFEST.in
+-rw-rw-rw-   0        0        0     6805 2024-03-18 21:38:32.558490 flask-monocrud-0.0.1rc9/PKG-INFO
+-rw-rw-rw-   0        0        0     6014 2024-03-18 19:50:13.000000 flask-monocrud-0.0.1rc9/README.md
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.427491 flask-monocrud-0.0.1rc9/flask_monocrud/
+-rw-rw-rw-   0        0        0     4377 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/AdminModel.py
+-rw-rw-rw-   0        0        0     2182 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/QueryHandler.py
+-rw-rw-rw-   0        0        0    16068 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.434491 flask-monocrud-0.0.1rc9/flask_monocrud/action_components/
+-rw-rw-rw-   0        0        0     1733 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/action_components/__init__.py
+-rw-rw-rw-   0        0        0    14960 2024-03-18 21:16:25.000000 flask-monocrud-0.0.1rc9/flask_monocrud/ext.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.448490 flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/
+-rw-rw-rw-   0        0        0    10046 2024-03-18 20:07:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/__init__.py
+-rw-rw-rw-   0        0        0      141 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/compat.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.459491 flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/panels/
+-rw-rw-rw-   0        0        0     1524 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/panels/__init__.py
+-rw-rw-rw-   0        0        0      622 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/panels/config_vars.py
+-rw-rw-rw-   0        0        0      565 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/panels/g.py
+-rw-rw-rw-   0        0        0     1332 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/panels/headers.py
+-rw-rw-rw-   0        0        0     3294 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/panels/logger.py
+-rw-rw-rw-   0        0        0     3650 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/panels/profiler.py
+-rw-rw-rw-   0        0        0     1755 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/panels/request_vars.py
+-rw-rw-rw-   0        0        0      890 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/panels/route_list.py
+-rw-rw-rw-   0        0        0     4244 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/panels/sqlalchemy.py
+-rw-rw-rw-   0        0        0     5181 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/panels/template.py
+-rw-rw-rw-   0        0        0     3290 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/panels/timer.py
+-rw-rw-rw-   0        0        0     1274 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/panels/versions.py
+-rw-rw-rw-   0        0        0     2161 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/toolbar.py
+-rw-rw-rw-   0        0        0     2736 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/utils.py
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/flask_monocrud.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.471491 flask-monocrud-0.0.1rc9/flask_monocrud/form_components/
+-rw-rw-rw-   0        0        0      281 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/form_components/__init__.py
+-rw-rw-rw-   0        0        0      800 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/form_components/checkbox.py
+-rw-rw-rw-   0        0        0     1654 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/form_components/field.py
+-rw-rw-rw-   0        0        0      432 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/form_components/file_upload.py
+-rw-rw-rw-   0        0        0      855 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/form_components/grid.py
+-rw-rw-rw-   0        0        0       68 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/form_components/guard.py
+-rw-rw-rw-   0        0        0      784 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/form_components/horizontal_separator.py
+-rw-rw-rw-   0        0        0      353 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/form_components/radio.py
+-rw-rw-rw-   0        0        0     2992 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/form_components/repeater.py
+-rw-rw-rw-   0        0        0      944 2024-03-16 20:01:15.000000 flask-monocrud-0.0.1rc9/flask_monocrud/form_components/select.py
+-rw-rw-rw-   0        0        0     1879 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/form_components/text_area.py
+-rw-rw-rw-   0        0        0     3165 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/form_components/text_input.py
+-rw-rw-rw-   0        0        0      398 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/form_components/toggle.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.478492 flask-monocrud-0.0.1rc9/flask_monocrud/helpers/
+-rw-rw-rw-   0        0        0     1330 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/helpers/Dater.py
+-rw-rw-rw-   0        0        0     1641 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1079 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/helpers/get_by_dot.py
+-rw-rw-rw-   0        0        0       53 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/helpers/get_type.py
+-rw-rw-rw-   0        0        0      143 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/helpers/optional.py
+-rw-rw-rw-   0        0        0      336 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/helpers/to_class.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.479491 flask-monocrud-0.0.1rc9/flask_monocrud/live_component/
+-rw-rw-rw-   0        0        0      410 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/live_component/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.481490 flask-monocrud-0.0.1rc9/flask_monocrud/metrics/
+-rw-rw-rw-   0        0        0       26 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/metrics/__init__.py
+-rw-rw-rw-   0        0        0     1170 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/metrics/metric.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.483492 flask-monocrud-0.0.1rc9/flask_monocrud/notification_component/
+-rw-rw-rw-   0        0        0       38 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/notification_component/__init__.py
+-rw-rw-rw-   0        0        0     2315 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/notification_component/notification.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.484512 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.485491 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/application/
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/application/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.485491 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/application/admin/
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/application/admin/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.486489 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/application/casts/
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/application/casts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.487490 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/application/events/
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/application/events/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.488490 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/application/hooks/
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/application/hooks/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.489490 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/application/models/
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/application/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.489490 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/application/observers/
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/application/observers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.490490 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/application/policies/
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/application/policies/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.491490 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/application/providers/
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/application/providers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.491490 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/application/scopes/
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/application/scopes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.492490 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/application/services/
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/application/services/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.494490 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/application/traits/
+-rw-rw-rw-   0        0        0     3498 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/application/traits/EnhancedModelTrait.py
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/application/traits/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.495490 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/config/
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/config/__init__.py
+-rw-rw-rw-   0        0        0      461 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/config/database.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.496492 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/databases/
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/databases/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.497491 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/databases/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/databases/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.497491 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/pages/
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/pages/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.498490 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/pages/admin/
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/pages/admin/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.499492 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/static/
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/static/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.499492 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/templates/
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.500493 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/uploads/
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/uploads/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.502492 flask-monocrud-0.0.1rc9/flask_monocrud/relations/
+-rw-rw-rw-   0        0        0       30 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/relations/__init__.py
+-rw-rw-rw-   0        0        0     1071 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/relations/relation.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.512490 flask-monocrud-0.0.1rc9/flask_monocrud/stubs/
+-rw-rw-rw-   0        0        0      191 2024-03-18 21:23:59.000000 flask-monocrud-0.0.1rc9/flask_monocrud/stubs/create-view.stub
+-rw-rw-rw-   0        0        0      193 2024-03-18 21:23:59.000000 flask-monocrud-0.0.1rc9/flask_monocrud/stubs/edit-view.stub
+-rw-rw-rw-   0        0        0      184 2024-03-18 21:23:59.000000 flask-monocrud-0.0.1rc9/flask_monocrud/stubs/list-view.stub
+-rw-rw-rw-   0        0        0      461 2024-03-18 21:23:59.000000 flask-monocrud-0.0.1rc9/flask_monocrud/stubs/migration.stub
+-rw-rw-rw-   0        0        0      199 2024-03-18 21:23:59.000000 flask-monocrud-0.0.1rc9/flask_monocrud/stubs/preview-view.stub
+-rw-rw-rw-   0        0        0     1156 2024-03-18 21:23:59.000000 flask-monocrud-0.0.1rc9/flask_monocrud/stubs/resource-admin.stub
+-rw-rw-rw-   0        0        0      374 2024-03-18 21:27:39.000000 flask-monocrud-0.0.1rc9/flask_monocrud/stubs/resource-hooks.stub
+-rw-rw-rw-   0        0        0      346 2024-03-18 21:23:59.000000 flask-monocrud-0.0.1rc9/flask_monocrud/stubs/resource-model.stub
+-rw-rw-rw-   0        0        0      352 2024-03-18 21:27:11.000000 flask-monocrud-0.0.1rc9/flask_monocrud/stubs/resource-policies.stub
+-rw-rw-rw-   0        0        0      276 2024-03-18 21:23:59.000000 flask-monocrud-0.0.1rc9/flask_monocrud/stubs/submit-create.stub
+-rw-rw-rw-   0        0        0      237 2024-03-18 21:23:59.000000 flask-monocrud-0.0.1rc9/flask_monocrud/stubs/submit-delete.stub
+-rw-rw-rw-   0        0        0      271 2024-03-18 21:23:59.000000 flask-monocrud-0.0.1rc9/flask_monocrud/stubs/submit-edit.stub
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.514490 flask-monocrud-0.0.1rc9/flask_monocrud/table_components/
+-rw-rw-rw-   0        0        0      260 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/table_components/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.519512 flask-monocrud-0.0.1rc9/flask_monocrud/table_components/columns/
+-rw-rw-rw-   0        0        0        0 2024-03-18 21:38:13.000000 flask-monocrud-0.0.1rc9/flask_monocrud/table_components/columns/__init__.py
+-rw-rw-rw-   0        0        0      329 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/table_components/columns/badge_column.py
+-rw-rw-rw-   0        0        0      371 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/table_components/columns/boolean_column.py
+-rw-rw-rw-   0        0        0     1183 2024-03-18 21:26:34.000000 flask-monocrud-0.0.1rc9/flask_monocrud/table_components/columns/column.py
+-rw-rw-rw-   0        0        0      760 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/table_components/columns/image_column.py
+-rw-rw-rw-   0        0        0     1255 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/table_components/columns/text_column.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.521489 flask-monocrud-0.0.1rc9/flask_monocrud/table_components/filters/
+-rw-rw-rw-   0        0        0        0 2024-03-18 21:38:13.000000 flask-monocrud-0.0.1rc9/flask_monocrud/table_components/filters/__init__.py
+-rw-rw-rw-   0        0        0     1403 2024-03-12 11:22:17.000000 flask-monocrud-0.0.1rc9/flask_monocrud/table_components/filters/filter.py
+-rw-rw-rw-   0        0        0     1344 2024-03-14 23:45:22.000000 flask-monocrud-0.0.1rc9/flask_monocrud/table_components/filters/tab.py
+-rw-rw-rw-   0        0        0     1319 2024-03-15 04:58:50.000000 flask-monocrud-0.0.1rc9/flask_monocrud/table_components/table.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.522490 flask-monocrud-0.0.1rc9/flask_monocrud/templates/
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:04:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.528508 flask-monocrud-0.0.1rc9/flask_monocrud/templates/admin/
+-rw-rw-rw-   0        0        0      113 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/templates/admin/Page.html
+-rw-rw-rw-   0        0        0     2176 2024-03-10 13:54:38.000000 flask-monocrud-0.0.1rc9/flask_monocrud/templates/admin/index.html
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.552491 flask-monocrud-0.0.1rc9/flask_monocrud/templates/admin/views/
+-rw-rw-rw-   0        0        0      980 2024-03-17 01:41:49.000000 flask-monocrud-0.0.1rc9/flask_monocrud/templates/admin/views/CreateView.html
+-rw-rw-rw-   0        0        0    17166 2024-03-17 17:12:18.000000 flask-monocrud-0.0.1rc9/flask_monocrud/templates/admin/views/EditView.html
+-rw-rw-rw-   0        0        0    19310 2024-03-17 01:34:28.000000 flask-monocrud-0.0.1rc9/flask_monocrud/templates/admin/views/ListView.html
+-rw-rw-rw-   0        0        0     1241 2024-03-17 17:25:03.000000 flask-monocrud-0.0.1rc9/flask_monocrud/templates/admin/views/PreviewView.html
+drwxrwxrwx   0        0        0        0 2024-03-18 21:38:32.433492 flask-monocrud-0.0.1rc9/flask_monocrud.egg-info/
+-rw-rw-rw-   0        0        0     6805 2024-03-18 21:38:32.000000 flask-monocrud-0.0.1rc9/flask_monocrud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5015 2024-03-18 21:38:32.000000 flask-monocrud-0.0.1rc9/flask_monocrud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-18 21:38:32.000000 flask-monocrud-0.0.1rc9/flask_monocrud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2024-03-18 21:38:32.000000 flask-monocrud-0.0.1rc9/flask_monocrud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-03-18 21:38:32.000000 flask-monocrud-0.0.1rc9/flask_monocrud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-03-18 21:38:32.565490 flask-monocrud-0.0.1rc9/setup.cfg
+-rw-rw-rw-   0        0        0     1069 2024-03-18 21:38:30.000000 flask-monocrud-0.0.1rc9/setup.py
```

### Comparing `flask-monocrud-0.0.1rc8/PKG-INFO` & `flask-monocrud-0.0.1rc9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-monocrud
-Version: 0.0.1rc8
+Version: 0.0.1rc9
 Summary: Package provides utilities for managing fixture data python applications. It offers a convenient way to populate database tables with predefined data.
 Home-page: https://github.com/JarriqTheTechie/masonite-fixtures
 Author: Jarriq Rolle
 Author-email: jrolle@bnbbahamas.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `flask-monocrud-0.0.1rc8/README.md` & `flask-monocrud-0.0.1rc9/README.md`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/AdminModel.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/AdminModel.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/QueryHandler.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/QueryHandler.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/__init__.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/action_components/__init__.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/action_components/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/ext.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/ext.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/__init__.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/panels/__init__.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/panels/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/panels/config_vars.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/panels/config_vars.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/panels/g.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/panels/g.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/panels/headers.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/panels/headers.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/panels/logger.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/panels/logger.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/panels/profiler.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/panels/profiler.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/panels/request_vars.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/panels/request_vars.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/panels/route_list.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/panels/route_list.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/panels/sqlalchemy.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/panels/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/panels/template.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/panels/template.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/panels/timer.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/panels/timer.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/panels/versions.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/panels/versions.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/toolbar.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/toolbar.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/flask_debugtoolbar/utils.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/flask_debugtoolbar/utils.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/form_components/checkbox.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/form_components/checkbox.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/form_components/field.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/form_components/field.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/form_components/grid.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/form_components/grid.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/form_components/horizontal_separator.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/form_components/horizontal_separator.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/form_components/repeater.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/form_components/repeater.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/form_components/select.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/form_components/select.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/form_components/text_area.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/form_components/text_area.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/form_components/text_input.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/form_components/text_input.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/helpers/Dater.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/helpers/Dater.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/helpers/__init__.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/helpers/get_by_dot.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/helpers/get_by_dot.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/metrics/metric.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/notification_component/notification.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/notification_component/notification.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/project_structure/application/traits/EnhancedModelTrait.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/project_structure/application/traits/EnhancedModelTrait.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/relations/relation.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/relations/relation.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/stubs/resource-admin.stub` & `flask-monocrud-0.0.1rc9/flask_monocrud/stubs/resource-admin.stub`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/table_components/table.py` & `flask-monocrud-0.0.1rc9/flask_monocrud/table_components/table.py`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/templates/admin/index.html` & `flask-monocrud-0.0.1rc9/flask_monocrud/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/templates/admin/views/CreateView.html` & `flask-monocrud-0.0.1rc9/flask_monocrud/templates/admin/views/CreateView.html`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/templates/admin/views/EditView.html` & `flask-monocrud-0.0.1rc9/flask_monocrud/templates/admin/views/EditView.html`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/templates/admin/views/ListView.html` & `flask-monocrud-0.0.1rc9/flask_monocrud/templates/admin/views/ListView.html`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud/templates/admin/views/PreviewView.html` & `flask-monocrud-0.0.1rc9/flask_monocrud/templates/admin/views/PreviewView.html`

 * *Files identical despite different names*

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud.egg-info/PKG-INFO` & `flask-monocrud-0.0.1rc9/flask_monocrud.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-monocrud
-Version: 0.0.1rc8
+Version: 0.0.1rc9
 Summary: Package provides utilities for managing fixture data python applications. It offers a convenient way to populate database tables with predefined data.
 Home-page: https://github.com/JarriqTheTechie/masonite-fixtures
 Author: Jarriq Rolle
 Author-email: jrolle@bnbbahamas.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `flask-monocrud-0.0.1rc8/flask_monocrud.egg-info/SOURCES.txt` & `flask-monocrud-0.0.1rc9/flask_monocrud.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -87,14 +87,23 @@
 flask_monocrud/stubs/resource-model.stub
 flask_monocrud/stubs/resource-policies.stub
 flask_monocrud/stubs/submit-create.stub
 flask_monocrud/stubs/submit-delete.stub
 flask_monocrud/stubs/submit-edit.stub
 flask_monocrud/table_components/__init__.py
 flask_monocrud/table_components/table.py
+flask_monocrud/table_components/columns/__init__.py
+flask_monocrud/table_components/columns/badge_column.py
+flask_monocrud/table_components/columns/boolean_column.py
+flask_monocrud/table_components/columns/column.py
+flask_monocrud/table_components/columns/image_column.py
+flask_monocrud/table_components/columns/text_column.py
+flask_monocrud/table_components/filters/__init__.py
+flask_monocrud/table_components/filters/filter.py
+flask_monocrud/table_components/filters/tab.py
 flask_monocrud/templates/__init__.py
 flask_monocrud/templates/admin/Page.html
 flask_monocrud/templates/admin/index.html
 flask_monocrud/templates/admin/views/CreateView.html
 flask_monocrud/templates/admin/views/EditView.html
 flask_monocrud/templates/admin/views/ListView.html
 flask_monocrud/templates/admin/views/PreviewView.html
```

### Comparing `flask-monocrud-0.0.1rc8/setup.py` & `flask-monocrud-0.0.1rc9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="flask-monocrud",
-    version="0.0.1rc8",
+    version="0.0.1rc9",
     author="Jarriq Rolle",
     author_email="jrolle@bnbbahamas.com",
     description="Package provides utilities for managing fixture data python applications. It offers a convenient way to populate database tables with predefined data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JarriqTheTechie/masonite-fixtures",
     packages=find_packages(),
```

