# Comparing `tmp/nr-metadata-2.0.8.tar.gz` & `tmp/nr-metadata-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nr-metadata-2.0.8.tar", last modified: Wed Jan 10 09:43:15 2024, max compression
+gzip compressed data, was "nr-metadata-2.0.9.tar", last modified: Thu Feb 29 06:42:24 2024, max compression
```

## Comparing `nr-metadata-2.0.8.tar` & `nr-metadata-2.0.9.tar`

### file list

```diff
@@ -1,138 +1,248 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.070607 nr-metadata-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-01-10 09:40:26.000000 nr-metadata-2.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-01-10 09:43:15.070607 nr-metadata-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-01-10 09:41:54.000000 nr-metadata-2.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.050607 nr-metadata-2.0.8/nr_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:40:26.000000 nr-metadata-2.0.8/nr_metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.054607 nr-metadata-2.0.8/nr_metadata/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:41:32.000000 nr-metadata-2.0.8/nr_metadata/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-01-10 09:41:32.000000 nr-metadata-2.0.8/nr_metadata/common/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-01-10 09:41:32.000000 nr-metadata-2.0.8/nr_metadata/common/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.054607 nr-metadata-2.0.8/nr_metadata/common/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:41:33.000000 nr-metadata-2.0.8/nr_metadata/common/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   236495 2024-01-10 09:41:33.000000 nr-metadata-2.0.8/nr_metadata/common/models/records.json
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-01-10 09:41:33.000000 nr-metadata-2.0.8/nr_metadata/common/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.054607 nr-metadata-2.0.8/nr_metadata/common/records/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:41:33.000000 nr-metadata-2.0.8/nr_metadata/common/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-01-10 09:41:33.000000 nr-metadata-2.0.8/nr_metadata/common/records/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.054607 nr-metadata-2.0.8/nr_metadata/common/records/dumpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:41:33.000000 nr-metadata-2.0.8/nr_metadata/common/records/dumpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-01-10 09:41:34.000000 nr-metadata-2.0.8/nr_metadata/common/records/dumpers/dumper.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-01-10 09:41:34.000000 nr-metadata-2.0.8/nr_metadata/common/records/dumpers/edtf.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-01-10 09:41:34.000000 nr-metadata-2.0.8/nr_metadata/common/records/dumpers/multilingual.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.054607 nr-metadata-2.0.8/nr_metadata/common/records/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:41:34.000000 nr-metadata-2.0.8/nr_metadata/common/records/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35321 2024-01-10 09:41:34.000000 nr-metadata-2.0.8/nr_metadata/common/records/jsonschemas/common-1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.054607 nr-metadata-2.0.8/nr_metadata/common/records/mappings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:41:34.000000 nr-metadata-2.0.8/nr_metadata/common/records/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.054607 nr-metadata-2.0.8/nr_metadata/common/records/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:41:34.000000 nr-metadata-2.0.8/nr_metadata/common/records/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.058607 nr-metadata-2.0.8/nr_metadata/common/records/mappings/os-v2/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:41:35.000000 nr-metadata-2.0.8/nr_metadata/common/records/mappings/os-v2/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51772 2024-01-10 09:41:35.000000 nr-metadata-2.0.8/nr_metadata/common/records/mappings/os-v2/common/common-1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-01-10 09:41:35.000000 nr-metadata-2.0.8/nr_metadata/common/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.058607 nr-metadata-2.0.8/nr_metadata/common/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:41:35.000000 nr-metadata-2.0.8/nr_metadata/common/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.058607 nr-metadata-2.0.8/nr_metadata/common/resources/records/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:41:35.000000 nr-metadata-2.0.8/nr_metadata/common/resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-01-10 09:41:36.000000 nr-metadata-2.0.8/nr_metadata/common/resources/records/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-01-10 09:41:36.000000 nr-metadata-2.0.8/nr_metadata/common/resources/records/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-01-10 09:41:36.000000 nr-metadata-2.0.8/nr_metadata/common/resources/records/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.058607 nr-metadata-2.0.8/nr_metadata/common/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:41:36.000000 nr-metadata-2.0.8/nr_metadata/common/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.058607 nr-metadata-2.0.8/nr_metadata/common/services/records/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:41:36.000000 nr-metadata-2.0.8/nr_metadata/common/services/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-01-10 09:41:37.000000 nr-metadata-2.0.8/nr_metadata/common/services/records/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    13855 2024-01-10 09:41:37.000000 nr-metadata-2.0.8/nr_metadata/common/services/records/facets.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-01-10 09:41:37.000000 nr-metadata-2.0.8/nr_metadata/common/services/records/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-01-10 09:41:37.000000 nr-metadata-2.0.8/nr_metadata/common/services/records/schema_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-01-10 09:41:38.000000 nr-metadata-2.0.8/nr_metadata/common/services/records/schema_datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-01-10 09:41:38.000000 nr-metadata-2.0.8/nr_metadata/common/services/records/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-01-10 09:41:38.000000 nr-metadata-2.0.8/nr_metadata/common/services/records/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-01-10 09:41:38.000000 nr-metadata-2.0.8/nr_metadata/common/services/records/ui_schema_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-01-10 09:41:39.000000 nr-metadata-2.0.8/nr_metadata/common/services/records/ui_schema_datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-10 09:41:39.000000 nr-metadata-2.0.8/nr_metadata/common/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.058607 nr-metadata-2.0.8/nr_metadata/common/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:41:39.000000 nr-metadata-2.0.8/nr_metadata/common/views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.058607 nr-metadata-2.0.8/nr_metadata/common/views/records/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:41:39.000000 nr-metadata-2.0.8/nr_metadata/common/views/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-01-10 09:41:40.000000 nr-metadata-2.0.8/nr_metadata/common/views/records/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-01-10 09:41:40.000000 nr-metadata-2.0.8/nr_metadata/common/views/records/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.062607 nr-metadata-2.0.8/nr_metadata/documents/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:41:46.000000 nr-metadata-2.0.8/nr_metadata/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-01-10 09:41:46.000000 nr-metadata-2.0.8/nr_metadata/documents/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-01-10 09:41:47.000000 nr-metadata-2.0.8/nr_metadata/documents/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.062607 nr-metadata-2.0.8/nr_metadata/documents/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:41:47.000000 nr-metadata-2.0.8/nr_metadata/documents/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   352942 2024-01-10 09:41:47.000000 nr-metadata-2.0.8/nr_metadata/documents/models/records.json
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-01-10 09:41:47.000000 nr-metadata-2.0.8/nr_metadata/documents/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.062607 nr-metadata-2.0.8/nr_metadata/documents/records/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:41:47.000000 nr-metadata-2.0.8/nr_metadata/documents/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-01-10 09:41:48.000000 nr-metadata-2.0.8/nr_metadata/documents/records/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.062607 nr-metadata-2.0.8/nr_metadata/documents/records/dumpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:41:48.000000 nr-metadata-2.0.8/nr_metadata/documents/records/dumpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-10 09:41:48.000000 nr-metadata-2.0.8/nr_metadata/documents/records/dumpers/dumper.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-01-10 09:41:48.000000 nr-metadata-2.0.8/nr_metadata/documents/records/dumpers/edtf.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-01-10 09:41:48.000000 nr-metadata-2.0.8/nr_metadata/documents/records/dumpers/multilingual.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.062607 nr-metadata-2.0.8/nr_metadata/documents/records/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:41:48.000000 nr-metadata-2.0.8/nr_metadata/documents/records/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40544 2024-01-10 09:41:49.000000 nr-metadata-2.0.8/nr_metadata/documents/records/jsonschemas/documents-1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.062607 nr-metadata-2.0.8/nr_metadata/documents/records/mappings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:41:49.000000 nr-metadata-2.0.8/nr_metadata/documents/records/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.062607 nr-metadata-2.0.8/nr_metadata/documents/records/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:41:49.000000 nr-metadata-2.0.8/nr_metadata/documents/records/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.062607 nr-metadata-2.0.8/nr_metadata/documents/records/mappings/os-v2/documents/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:41:49.000000 nr-metadata-2.0.8/nr_metadata/documents/records/mappings/os-v2/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    58351 2024-01-10 09:41:49.000000 nr-metadata-2.0.8/nr_metadata/documents/records/mappings/os-v2/documents/documents-1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-01-10 09:41:49.000000 nr-metadata-2.0.8/nr_metadata/documents/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.062607 nr-metadata-2.0.8/nr_metadata/documents/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:41:49.000000 nr-metadata-2.0.8/nr_metadata/documents/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.066607 nr-metadata-2.0.8/nr_metadata/documents/resources/records/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:41:49.000000 nr-metadata-2.0.8/nr_metadata/documents/resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-01-10 09:41:50.000000 nr-metadata-2.0.8/nr_metadata/documents/resources/records/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-01-10 09:41:50.000000 nr-metadata-2.0.8/nr_metadata/documents/resources/records/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-01-10 09:41:50.000000 nr-metadata-2.0.8/nr_metadata/documents/resources/records/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.066607 nr-metadata-2.0.8/nr_metadata/documents/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:41:50.000000 nr-metadata-2.0.8/nr_metadata/documents/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.066607 nr-metadata-2.0.8/nr_metadata/documents/services/records/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:41:50.000000 nr-metadata-2.0.8/nr_metadata/documents/services/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-01-10 09:41:51.000000 nr-metadata-2.0.8/nr_metadata/documents/services/records/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    15104 2024-01-10 09:41:51.000000 nr-metadata-2.0.8/nr_metadata/documents/services/records/facets.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-01-10 09:41:51.000000 nr-metadata-2.0.8/nr_metadata/documents/services/records/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-01-10 09:41:52.000000 nr-metadata-2.0.8/nr_metadata/documents/services/records/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     9858 2024-01-10 09:41:52.000000 nr-metadata-2.0.8/nr_metadata/documents/services/records/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-01-10 09:41:52.000000 nr-metadata-2.0.8/nr_metadata/documents/services/records/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-01-10 09:41:53.000000 nr-metadata-2.0.8/nr_metadata/documents/services/records/ui_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-10 09:41:53.000000 nr-metadata-2.0.8/nr_metadata/documents/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.066607 nr-metadata-2.0.8/nr_metadata/documents/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:41:53.000000 nr-metadata-2.0.8/nr_metadata/documents/views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.066607 nr-metadata-2.0.8/nr_metadata/documents/views/records/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:41:53.000000 nr-metadata-2.0.8/nr_metadata/documents/views/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-01-10 09:41:53.000000 nr-metadata-2.0.8/nr_metadata/documents/views/records/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-01-10 09:41:54.000000 nr-metadata-2.0.8/nr_metadata/documents/views/records/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.066607 nr-metadata-2.0.8/nr_metadata/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:40:26.000000 nr-metadata-2.0.8/nr_metadata/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-01-10 09:40:26.000000 nr-metadata-2.0.8/nr_metadata/schema/identifiers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.066607 nr-metadata-2.0.8/nr_metadata/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:40:26.000000 nr-metadata-2.0.8/nr_metadata/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.066607 nr-metadata-2.0.8/nr_metadata/services/records/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:40:26.000000 nr-metadata-2.0.8/nr_metadata/services/records/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.070607 nr-metadata-2.0.8/nr_metadata/services/records/facets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:40:26.000000 nr-metadata-2.0.8/nr_metadata/services/records/facets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-01-10 09:40:26.000000 nr-metadata-2.0.8/nr_metadata/services/records/facets/dumper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.070607 nr-metadata-2.0.8/nr_metadata/ui_schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:40:26.000000 nr-metadata-2.0.8/nr_metadata/ui_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-01-10 09:40:26.000000 nr-metadata-2.0.8/nr_metadata/ui_schema/identifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-01-10 09:40:26.000000 nr-metadata-2.0.8/nr_metadata/ui_schema/subjects.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-10 09:41:54.000000 nr-metadata-2.0.8/nr_metadata/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.070607 nr-metadata-2.0.8/nr_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-01-10 09:43:14.000000 nr-metadata-2.0.8/nr_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-01-10 09:43:15.000000 nr-metadata-2.0.8/nr_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 09:43:14.000000 nr-metadata-2.0.8/nr_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-01-10 09:43:14.000000 nr-metadata-2.0.8/nr_metadata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 09:43:00.000000 nr-metadata-2.0.8/nr_metadata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-01-10 09:43:14.000000 nr-metadata-2.0.8/nr_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-10 09:43:14.000000 nr-metadata-2.0.8/nr_metadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-01-10 09:40:26.000000 nr-metadata-2.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-01-10 09:43:15.070607 nr-metadata-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-10 09:40:26.000000 nr-metadata-2.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.485904 nr-metadata-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-02-29 06:42:24.485904 nr-metadata-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-02-29 06:40:52.000000 nr-metadata-2.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.453904 nr-metadata-2.0.9/nr_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.453904 nr-metadata-2.0.9/nr_metadata/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:10.000000 nr-metadata-2.0.9/nr_metadata/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-02-29 06:40:11.000000 nr-metadata-2.0.9/nr_metadata/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-02-29 06:40:11.000000 nr-metadata-2.0.9/nr_metadata/common/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.453904 nr-metadata-2.0.9/nr_metadata/common/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:11.000000 nr-metadata-2.0.9/nr_metadata/common/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   339677 2024-02-29 06:40:11.000000 nr-metadata-2.0.9/nr_metadata/common/models/records.json
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-02-29 06:40:11.000000 nr-metadata-2.0.9/nr_metadata/common/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.457904 nr-metadata-2.0.9/nr_metadata/common/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:11.000000 nr-metadata-2.0.9/nr_metadata/common/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-02-29 06:40:12.000000 nr-metadata-2.0.9/nr_metadata/common/records/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.457904 nr-metadata-2.0.9/nr_metadata/common/records/dumpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:12.000000 nr-metadata-2.0.9/nr_metadata/common/records/dumpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-02-29 06:40:12.000000 nr-metadata-2.0.9/nr_metadata/common/records/dumpers/dumper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-29 06:40:12.000000 nr-metadata-2.0.9/nr_metadata/common/records/dumpers/edtf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-02-29 06:40:12.000000 nr-metadata-2.0.9/nr_metadata/common/records/dumpers/multilingual.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.457904 nr-metadata-2.0.9/nr_metadata/common/records/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:12.000000 nr-metadata-2.0.9/nr_metadata/common/records/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36444 2024-02-29 06:40:13.000000 nr-metadata-2.0.9/nr_metadata/common/records/jsonschemas/common-1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.457904 nr-metadata-2.0.9/nr_metadata/common/records/mappings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:13.000000 nr-metadata-2.0.9/nr_metadata/common/records/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.457904 nr-metadata-2.0.9/nr_metadata/common/records/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:13.000000 nr-metadata-2.0.9/nr_metadata/common/records/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.457904 nr-metadata-2.0.9/nr_metadata/common/records/mappings/os-v2/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:13.000000 nr-metadata-2.0.9/nr_metadata/common/records/mappings/os-v2/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53381 2024-02-29 06:40:13.000000 nr-metadata-2.0.9/nr_metadata/common/records/mappings/os-v2/common/common-1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-02-29 06:40:13.000000 nr-metadata-2.0.9/nr_metadata/common/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.457904 nr-metadata-2.0.9/nr_metadata/common/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:13.000000 nr-metadata-2.0.9/nr_metadata/common/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.457904 nr-metadata-2.0.9/nr_metadata/common/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:14.000000 nr-metadata-2.0.9/nr_metadata/common/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-02-29 06:40:14.000000 nr-metadata-2.0.9/nr_metadata/common/resources/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-29 06:40:14.000000 nr-metadata-2.0.9/nr_metadata/common/resources/records/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-02-29 06:40:14.000000 nr-metadata-2.0.9/nr_metadata/common/resources/records/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.457904 nr-metadata-2.0.9/nr_metadata/common/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:14.000000 nr-metadata-2.0.9/nr_metadata/common/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.461904 nr-metadata-2.0.9/nr_metadata/common/services/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:15.000000 nr-metadata-2.0.9/nr_metadata/common/services/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-02-29 06:40:15.000000 nr-metadata-2.0.9/nr_metadata/common/services/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14955 2024-02-29 06:40:15.000000 nr-metadata-2.0.9/nr_metadata/common/services/records/facets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-02-29 06:40:16.000000 nr-metadata-2.0.9/nr_metadata/common/services/records/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-02-29 06:40:16.000000 nr-metadata-2.0.9/nr_metadata/common/services/records/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-02-29 06:40:43.000000 nr-metadata-2.0.9/nr_metadata/common/services/records/schema_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-02-29 06:40:43.000000 nr-metadata-2.0.9/nr_metadata/common/services/records/schema_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7964 2024-02-29 06:40:17.000000 nr-metadata-2.0.9/nr_metadata/common/services/records/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-29 06:40:17.000000 nr-metadata-2.0.9/nr_metadata/common/services/records/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-02-29 06:40:44.000000 nr-metadata-2.0.9/nr_metadata/common/services/records/ui_schema_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8886 2024-02-29 06:40:44.000000 nr-metadata-2.0.9/nr_metadata/common/services/records/ui_schema_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-29 06:40:18.000000 nr-metadata-2.0.9/nr_metadata/common/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.461904 nr-metadata-2.0.9/nr_metadata/common/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:18.000000 nr-metadata-2.0.9/nr_metadata/common/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.461904 nr-metadata-2.0.9/nr_metadata/common/views/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:18.000000 nr-metadata-2.0.9/nr_metadata/common/views/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-02-29 06:40:18.000000 nr-metadata-2.0.9/nr_metadata/common/views/records/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-02-29 06:40:18.000000 nr-metadata-2.0.9/nr_metadata/common/views/records/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.461904 nr-metadata-2.0.9/nr_metadata/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:44.000000 nr-metadata-2.0.9/nr_metadata/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-02-29 06:40:44.000000 nr-metadata-2.0.9/nr_metadata/data/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-02-29 06:40:45.000000 nr-metadata-2.0.9/nr_metadata/data/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.461904 nr-metadata-2.0.9/nr_metadata/data/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:45.000000 nr-metadata-2.0.9/nr_metadata/data/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   424493 2024-02-29 06:40:45.000000 nr-metadata-2.0.9/nr_metadata/data/models/records.json
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-02-29 06:40:45.000000 nr-metadata-2.0.9/nr_metadata/data/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.461904 nr-metadata-2.0.9/nr_metadata/data/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:45.000000 nr-metadata-2.0.9/nr_metadata/data/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-02-29 06:40:45.000000 nr-metadata-2.0.9/nr_metadata/data/records/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.465904 nr-metadata-2.0.9/nr_metadata/data/records/dumpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:45.000000 nr-metadata-2.0.9/nr_metadata/data/records/dumpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-02-29 06:40:46.000000 nr-metadata-2.0.9/nr_metadata/data/records/dumpers/dumper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-02-29 06:40:46.000000 nr-metadata-2.0.9/nr_metadata/data/records/dumpers/edtf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-02-29 06:40:46.000000 nr-metadata-2.0.9/nr_metadata/data/records/dumpers/multilingual.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.465904 nr-metadata-2.0.9/nr_metadata/data/records/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:46.000000 nr-metadata-2.0.9/nr_metadata/data/records/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39371 2024-02-29 06:40:46.000000 nr-metadata-2.0.9/nr_metadata/data/records/jsonschemas/data-1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.465904 nr-metadata-2.0.9/nr_metadata/data/records/mappings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:46.000000 nr-metadata-2.0.9/nr_metadata/data/records/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.465904 nr-metadata-2.0.9/nr_metadata/data/records/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:47.000000 nr-metadata-2.0.9/nr_metadata/data/records/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.465904 nr-metadata-2.0.9/nr_metadata/data/records/mappings/os-v2/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:47.000000 nr-metadata-2.0.9/nr_metadata/data/records/mappings/os-v2/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57154 2024-02-29 06:40:47.000000 nr-metadata-2.0.9/nr_metadata/data/records/mappings/os-v2/data/data-1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-02-29 06:40:47.000000 nr-metadata-2.0.9/nr_metadata/data/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.465904 nr-metadata-2.0.9/nr_metadata/data/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:47.000000 nr-metadata-2.0.9/nr_metadata/data/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.465904 nr-metadata-2.0.9/nr_metadata/data/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:47.000000 nr-metadata-2.0.9/nr_metadata/data/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-02-29 06:40:48.000000 nr-metadata-2.0.9/nr_metadata/data/resources/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-02-29 06:40:48.000000 nr-metadata-2.0.9/nr_metadata/data/resources/records/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-29 06:40:48.000000 nr-metadata-2.0.9/nr_metadata/data/resources/records/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.465904 nr-metadata-2.0.9/nr_metadata/data/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:48.000000 nr-metadata-2.0.9/nr_metadata/data/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.465904 nr-metadata-2.0.9/nr_metadata/data/services/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:48.000000 nr-metadata-2.0.9/nr_metadata/data/services/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-02-29 06:40:49.000000 nr-metadata-2.0.9/nr_metadata/data/services/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15528 2024-02-29 06:40:49.000000 nr-metadata-2.0.9/nr_metadata/data/services/records/facets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-02-29 06:40:49.000000 nr-metadata-2.0.9/nr_metadata/data/services/records/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-02-29 06:40:50.000000 nr-metadata-2.0.9/nr_metadata/data/services/records/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-02-29 06:40:50.000000 nr-metadata-2.0.9/nr_metadata/data/services/records/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-02-29 06:40:50.000000 nr-metadata-2.0.9/nr_metadata/data/services/records/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-29 06:40:50.000000 nr-metadata-2.0.9/nr_metadata/data/services/records/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-02-29 06:40:50.000000 nr-metadata-2.0.9/nr_metadata/data/services/records/ui_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-29 06:40:51.000000 nr-metadata-2.0.9/nr_metadata/data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.465904 nr-metadata-2.0.9/nr_metadata/data/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:51.000000 nr-metadata-2.0.9/nr_metadata/data/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.469904 nr-metadata-2.0.9/nr_metadata/data/views/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:51.000000 nr-metadata-2.0.9/nr_metadata/data/views/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-02-29 06:40:51.000000 nr-metadata-2.0.9/nr_metadata/data/views/records/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-02-29 06:40:51.000000 nr-metadata-2.0.9/nr_metadata/data/views/records/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.469904 nr-metadata-2.0.9/nr_metadata/datacite/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/datacite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/datacite/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/datacite/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.469904 nr-metadata-2.0.9/nr_metadata/datacite/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/datacite/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90098 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/datacite/models/records.json
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/datacite/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.469904 nr-metadata-2.0.9/nr_metadata/datacite/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/datacite/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-02-29 06:41:00.000000 nr-metadata-2.0.9/nr_metadata/datacite/records/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.469904 nr-metadata-2.0.9/nr_metadata/datacite/records/dumpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/datacite/records/dumpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-02-29 06:41:00.000000 nr-metadata-2.0.9/nr_metadata/datacite/records/dumpers/dumper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/datacite/records/dumpers/edtf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-02-29 06:41:00.000000 nr-metadata-2.0.9/nr_metadata/datacite/records/dumpers/multilingual.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.469904 nr-metadata-2.0.9/nr_metadata/datacite/records/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/datacite/records/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28542 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/datacite/records/jsonschemas/datacite-1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.469904 nr-metadata-2.0.9/nr_metadata/datacite/records/mappings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/datacite/records/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.469904 nr-metadata-2.0.9/nr_metadata/datacite/records/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/datacite/records/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.469904 nr-metadata-2.0.9/nr_metadata/datacite/records/mappings/os-v2/datacite/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/datacite/records/mappings/os-v2/datacite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32013 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/datacite/records/mappings/os-v2/datacite/datacite-1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/datacite/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.469904 nr-metadata-2.0.9/nr_metadata/datacite/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/datacite/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.473904 nr-metadata-2.0.9/nr_metadata/datacite/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/datacite/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/datacite/resources/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/datacite/resources/records/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/datacite/resources/records/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.473904 nr-metadata-2.0.9/nr_metadata/datacite/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/datacite/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.473904 nr-metadata-2.0.9/nr_metadata/datacite/services/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/datacite/services/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-02-29 06:41:01.000000 nr-metadata-2.0.9/nr_metadata/datacite/services/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22318 2024-02-29 06:41:01.000000 nr-metadata-2.0.9/nr_metadata/datacite/services/records/facets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/datacite/services/records/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-02-29 06:41:01.000000 nr-metadata-2.0.9/nr_metadata/datacite/services/records/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-02-29 06:41:02.000000 nr-metadata-2.0.9/nr_metadata/datacite/services/records/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61191 2024-02-29 06:41:02.000000 nr-metadata-2.0.9/nr_metadata/datacite/services/records/schema_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-02-29 06:41:03.000000 nr-metadata-2.0.9/nr_metadata/datacite/services/records/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/datacite/services/records/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-02-29 06:41:03.000000 nr-metadata-2.0.9/nr_metadata/datacite/services/records/ui_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60699 2024-02-29 06:41:04.000000 nr-metadata-2.0.9/nr_metadata/datacite/services/records/ui_schema_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/datacite/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.473904 nr-metadata-2.0.9/nr_metadata/datacite/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/datacite/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.473904 nr-metadata-2.0.9/nr_metadata/datacite/views/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/datacite/views/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8771 2024-02-29 06:41:04.000000 nr-metadata-2.0.9/nr_metadata/datacite/views/records/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/datacite/views/records/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.477904 nr-metadata-2.0.9/nr_metadata/documents/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:28.000000 nr-metadata-2.0.9/nr_metadata/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-02-29 06:40:28.000000 nr-metadata-2.0.9/nr_metadata/documents/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-02-29 06:40:28.000000 nr-metadata-2.0.9/nr_metadata/documents/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.477904 nr-metadata-2.0.9/nr_metadata/documents/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:28.000000 nr-metadata-2.0.9/nr_metadata/documents/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   446420 2024-02-29 06:40:28.000000 nr-metadata-2.0.9/nr_metadata/documents/models/records.json
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-02-29 06:40:29.000000 nr-metadata-2.0.9/nr_metadata/documents/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.477904 nr-metadata-2.0.9/nr_metadata/documents/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:29.000000 nr-metadata-2.0.9/nr_metadata/documents/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-02-29 06:40:29.000000 nr-metadata-2.0.9/nr_metadata/documents/records/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.477904 nr-metadata-2.0.9/nr_metadata/documents/records/dumpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:29.000000 nr-metadata-2.0.9/nr_metadata/documents/records/dumpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-29 06:40:29.000000 nr-metadata-2.0.9/nr_metadata/documents/records/dumpers/dumper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-02-29 06:40:30.000000 nr-metadata-2.0.9/nr_metadata/documents/records/dumpers/edtf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-02-29 06:40:30.000000 nr-metadata-2.0.9/nr_metadata/documents/records/dumpers/multilingual.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.477904 nr-metadata-2.0.9/nr_metadata/documents/records/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:30.000000 nr-metadata-2.0.9/nr_metadata/documents/records/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42317 2024-02-29 06:40:30.000000 nr-metadata-2.0.9/nr_metadata/documents/records/jsonschemas/documents-1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.477904 nr-metadata-2.0.9/nr_metadata/documents/records/mappings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:30.000000 nr-metadata-2.0.9/nr_metadata/documents/records/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.477904 nr-metadata-2.0.9/nr_metadata/documents/records/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:30.000000 nr-metadata-2.0.9/nr_metadata/documents/records/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.477904 nr-metadata-2.0.9/nr_metadata/documents/records/mappings/os-v2/documents/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:30.000000 nr-metadata-2.0.9/nr_metadata/documents/records/mappings/os-v2/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60615 2024-02-29 06:40:31.000000 nr-metadata-2.0.9/nr_metadata/documents/records/mappings/os-v2/documents/documents-1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-02-29 06:40:31.000000 nr-metadata-2.0.9/nr_metadata/documents/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.477904 nr-metadata-2.0.9/nr_metadata/documents/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:31.000000 nr-metadata-2.0.9/nr_metadata/documents/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.481904 nr-metadata-2.0.9/nr_metadata/documents/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:31.000000 nr-metadata-2.0.9/nr_metadata/documents/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-02-29 06:40:31.000000 nr-metadata-2.0.9/nr_metadata/documents/resources/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-29 06:40:32.000000 nr-metadata-2.0.9/nr_metadata/documents/resources/records/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-02-29 06:40:32.000000 nr-metadata-2.0.9/nr_metadata/documents/resources/records/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.481904 nr-metadata-2.0.9/nr_metadata/documents/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:32.000000 nr-metadata-2.0.9/nr_metadata/documents/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.481904 nr-metadata-2.0.9/nr_metadata/documents/services/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:32.000000 nr-metadata-2.0.9/nr_metadata/documents/services/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-02-29 06:40:32.000000 nr-metadata-2.0.9/nr_metadata/documents/services/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-02-29 06:40:33.000000 nr-metadata-2.0.9/nr_metadata/documents/services/records/facets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-02-29 06:40:33.000000 nr-metadata-2.0.9/nr_metadata/documents/services/records/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-29 06:40:33.000000 nr-metadata-2.0.9/nr_metadata/documents/services/records/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-02-29 06:40:33.000000 nr-metadata-2.0.9/nr_metadata/documents/services/records/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8718 2024-02-29 06:40:34.000000 nr-metadata-2.0.9/nr_metadata/documents/services/records/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-02-29 06:40:34.000000 nr-metadata-2.0.9/nr_metadata/documents/services/records/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-02-29 06:40:34.000000 nr-metadata-2.0.9/nr_metadata/documents/services/records/ui_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-29 06:40:34.000000 nr-metadata-2.0.9/nr_metadata/documents/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.481904 nr-metadata-2.0.9/nr_metadata/documents/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:34.000000 nr-metadata-2.0.9/nr_metadata/documents/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.481904 nr-metadata-2.0.9/nr_metadata/documents/views/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:40:35.000000 nr-metadata-2.0.9/nr_metadata/documents/views/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-02-29 06:40:35.000000 nr-metadata-2.0.9/nr_metadata/documents/views/records/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-02-29 06:40:35.000000 nr-metadata-2.0.9/nr_metadata/documents/views/records/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.481904 nr-metadata-2.0.9/nr_metadata/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/schema/identifiers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.481904 nr-metadata-2.0.9/nr_metadata/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.481904 nr-metadata-2.0.9/nr_metadata/services/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/services/records/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.481904 nr-metadata-2.0.9/nr_metadata/services/records/facets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/services/records/facets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/services/records/facets/dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.481904 nr-metadata-2.0.9/nr_metadata/ui_schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/ui_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/ui_schema/identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/nr_metadata/ui_schema/subjects.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-29 06:40:52.000000 nr-metadata-2.0.9/nr_metadata/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:24.481904 nr-metadata-2.0.9/nr_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-02-29 06:42:24.000000 nr-metadata-2.0.9/nr_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7919 2024-02-29 06:42:24.000000 nr-metadata-2.0.9/nr_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 06:42:24.000000 nr-metadata-2.0.9/nr_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-29 06:42:24.000000 nr-metadata-2.0.9/nr_metadata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 06:42:11.000000 nr-metadata-2.0.9/nr_metadata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-29 06:42:24.000000 nr-metadata-2.0.9/nr_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-29 06:42:24.000000 nr-metadata-2.0.9/nr_metadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-02-29 06:42:24.485904 nr-metadata-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 06:39:09.000000 nr-metadata-2.0.9/setup.py
```

### Comparing `nr-metadata-2.0.8/PKG-INFO` & `nr-metadata-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nr-metadata
-Version: 2.0.8
+Version: 2.0.9
 Summary: "Generated metadata files for the Czech National Repository"
 Home-page: https://github.com/Narodni-repozitar/ne-metadata
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio Czech NR
 Platform: any
```

### Comparing `nr-metadata-2.0.8/README.md` & `nr-metadata-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nr-metadata-2.0.8/nr_metadata/common/ext.py` & `nr-metadata-2.0.9/nr_metadata/common/ext.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 from functools import cached_property
 
 from nr_metadata.common import config
 
 
 class CommonExt:
+
     def __init__(self, app=None):
 
         if app:
             self.init_app(app)
 
     def init_app(self, app):
         """Flask application initialization."""
```

### Comparing `nr-metadata-2.0.8/nr_metadata/common/models/records.json` & `nr-metadata-2.0.9/nr_metadata/common/models/records.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642173872619838%*

 * *Differences: {"'model'": "{'search-options': {'fields': OrderedDict()}, 'facets': {'groups': True}, 'record': "*

 * *            "{'fields': OrderedDict()}, 'resource': {'additional-args': []}, 'resource-config': "*

 * *            "{'additional-args': []}, 'service-config': {'additional-args': [], delete: "*

 * *            "['result-list-class']}, 'service': {'additional-args': []}, 'json-serializer': "*

 * *            '{\'schema-context-args\': OrderedDict([(\'"object_key"\', \'"ui"\'), (\'"identity"\', '*

 * *            "'{{ flask.g{g.ide […]*

```diff
@@ -45,14 +45,15 @@
         "ext-resource": {
             "generate": true,
             "skip": false
         },
         "facets": {
             "extra-code": "",
             "generate": true,
+            "groups": true,
             "module": "nr_metadata.common.services.records.facets"
         },
         "json-schema-settings": {
             "alias": "common",
             "file": "nr_metadata/common/records/jsonschemas/common-1.0.0.json",
             "generate": true,
             "module": "nr_metadata.common.records.jsonschemas",
@@ -65,15 +66,19 @@
             ],
             "class": "nr_metadata.common.resources.records.ui.CommonUIJSONSerializer",
             "extra-code": "",
             "format_serializer_cls": "flask_resources.serializers.JSONSerializer",
             "generate": true,
             "imports": [],
             "list_schema_cls": "flask_resources.BaseListSchema",
-            "module": "nr_metadata.common.resources.records.ui"
+            "module": "nr_metadata.common.resources.records.ui",
+            "schema-context-args": {
+                "\"identity\"": "{{ flask.g{g.identity} }}",
+                "\"object_key\"": "\"ui\""
+            }
         },
         "mapping": {
             "alias": "common",
             "file": "nr_metadata/common/records/mappings/os-v2/common/common-1.0.0.json",
             "generate": true,
             "index": "common-common-1.0.0",
             "module": "nr_metadata.common.records.mappings"
@@ -479,14 +484,17 @@
                         },
                         "label.cs": "Dal\u0161\u00ed n\u00e1zvy",
                         "label.en": "Additional titles",
                         "type": "array"
                     },
                     "contributors": {
                         "items": {
+                            "discriminator": "nameType",
+                            "hint.cs": "Jako tv\u016frce je mo\u017en\u00e9 ozna\u010dit osobu nebo instituci.",
+                            "hint.en": "It is possible to designate a person or an institution as the creator/contributor.",
                             "marshmallow": {
                                 "class": "nr_metadata.common.services.records.schema_common.NRContributorSchema",
                                 "generate": true
                             },
                             "properties": {
                                 "affiliations": {
                                     "items": {
@@ -501,14 +509,21 @@
                                                 "import": "invenio_vocabularies.records.api.Vocabulary"
                                             }
                                         ],
                                         "keys": [
                                             "id",
                                             "title",
                                             {
+                                                "key": "props.ror",
+                                                "model": {
+                                                    "type": "keyword"
+                                                },
+                                                "target": "ror"
+                                            },
+                                            {
                                                 "key": "hierarchy",
                                                 "model": {
                                                     "marshmallow": {
                                                         "class": "oarepo_vocabularies.services.schema.HierarchySchema",
                                                         "generate": false,
                                                         "imports": [
                                                             {
@@ -696,14 +711,17 @@
                                                     "marshmallow": {
                                                         "field-class": "marshmallow.fields.String",
                                                         "imports": [],
                                                         "validators": []
                                                     }
                                                 }
                                             },
+                                            "ror": {
+                                                "type": "keyword"
+                                            },
                                             "title": {
                                                 "additionalProperties": {
                                                     "type": "string"
                                                 },
                                                 "mapping": {
                                                     "dynamic": true,
                                                     "properties": {
@@ -748,15 +766,15 @@
                                         "vocabulary-type": "institutions"
                                     },
                                     "type": "array"
                                 },
                                 "authorityIdentifiers": {
                                     "items": {
                                         "marshmallow": {
-                                            "class": "nr_metadata.schema.identifiers.NRAuthorityIdentifierSchema",
+                                            "class": "nr_metadata.schema.identifiers.NROrganizationIdentifierSchema",
                                             "generate": false
                                         },
                                         "properties": {
                                             "identifier": {
                                                 "i18n.key": "identifier",
                                                 "label.cs": "Identifik\u00e1tor",
                                                 "label.en": "Identifier",
@@ -764,20 +782,14 @@
                                                 "sample": {
                                                     "faker": "isbn13"
                                                 },
                                                 "type": "keyword"
                                             },
                                             "scheme": {
                                                 "enum": [
-                                                    "orcid",
-                                                    "scopusID",
-                                                    "researcherID",
-                                                    "czenasAutID",
-                                                    "vedidk",
-                                                    "institutionalID",
                                                     "ISNI",
                                                     "ROR",
                                                     "ICO",
                                                     "DOI"
                                                 ],
                                                 "hint.cs": "Doporu\u010dujeme zadat alespo\u0148 jeden z typ\u016f identifik\u00e1tor\u016f.\nPokud pot\u0159ebujete roz\u0161\u00ed\u0159it nab\u00eddku typ\u016f identifik\u00e1tor\u016f, kontaktujte n\u00e1s na support@narodni-repozitar.cz.\n",
                                                 "hint.en": "We recommend providing at least one of the identifier types.\nIf you need to expand the range of identifier types, contact us at support@narodni-repozitar.cz.\n",
@@ -786,71 +798,47 @@
                                                 "label.en": "Identifier type",
                                                 "required": true,
                                                 "type": "keyword"
                                             }
                                         },
                                         "type": "object",
                                         "ui": {
-                                            "detail": "nr_authority_identifier",
+                                            "detail": "nr_organization_identifier",
                                             "marshmallow": {
-                                                "class": "nr_metadata.ui_schema.identifiers.NRAuthorityIdentifierUISchema",
+                                                "class": "nr_metadata.ui_schema.identifiers.NROrganizationIdentifierUISchema",
                                                 "generate": false
                                             }
                                         }
                                     },
                                     "type": "array"
                                 },
-                                "fullName": {
-                                    "label.cs": "Jm\u00e9no p\u0159isp\u011bvatele",
-                                    "label.en": "Contributor name",
-                                    "required": true,
-                                    "sample": {
-                                        "faker": "name"
-                                    },
-                                    "type": "keyword"
-                                },
-                                "nameType": {
-                                    "enum": [
-                                        "Organizational",
-                                        "Personal"
-                                    ],
-                                    "hint.cs": "Jako tv\u016frce je mo\u017en\u00e9 ozna\u010dit osobu nebo instituci.",
-                                    "hint.en": "It is possible to designate a person or an institution as the creator/contributor.",
-                                    "label.cs": "Typ",
-                                    "label.en": "Type",
-                                    "sample": [
-                                        "Organizational",
-                                        "Personal"
-                                    ],
-                                    "type": "keyword"
-                                },
-                                "role": {
+                                "contributorType": {
                                     "facets": {
                                         "args": [
-                                            "vocabulary='contributor-roles'"
+                                            "vocabulary='contributor-types'"
                                         ]
                                     },
                                     "imports": [
                                         {
                                             "import": "invenio_vocabularies.records.api.Vocabulary"
                                         }
                                     ],
                                     "keys": [
                                         "id",
                                         "title"
                                     ],
-                                    "label.cs": "Role p\u0159isp\u011bvatele",
-                                    "label.en": "Contributor's role",
+                                    "label.cs": "Typ p\u0159isp\u011bvatele",
+                                    "label.en": "Contributor's type",
                                     "marshmallow": {
-                                        "class": "nr_metadata.common.services.records.schema_datatypes.NRAuthorityRoleVocabularySchema",
-                                        "generate": true,
+                                        "class": "nr_metadata.common.services.records.schema_datatypes.NRContributorTypeVocabularySchema",
+                                        "generate": false,
                                         "unknown": "INCLUDE"
                                     },
                                     "model": "vocabularies",
-                                    "pid-field": "Vocabulary.pid.with_type_ctx(\"contributor-roles\")",
+                                    "pid-field": "Vocabulary.pid.with_type_ctx(\"contributor-types\")",
                                     "properties": {
                                         "@v": {
                                             "facets": {
                                                 "facet": false
                                             },
                                             "marshmallow": {
                                                 "field-class": "marshmallow.fields.String",
@@ -922,37 +910,433 @@
                                         }
                                     },
                                     "type": "vocabulary",
                                     "ui": {
                                         "detail": "vocabulary_item",
                                         "edit": "vocabulary_item",
                                         "marshmallow": {
-                                            "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRAuthorityRoleVocabularyUISchema",
-                                            "generate": true,
+                                            "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRContributorTypeVocabularyUISchema",
+                                            "generate": false,
                                             "unknown": "INCLUDE"
                                         }
                                     },
-                                    "vocabulary-type": "contributor-roles"
+                                    "vocabulary-type": "contributor-types"
+                                },
+                                "familyName": {
+                                    "type": "keyword"
+                                },
+                                "fullName": {
+                                    "label.cs": "Jm\u00e9no p\u0159isp\u011bvatele",
+                                    "label.en": "Contributor name",
+                                    "required": true,
+                                    "sample": {
+                                        "faker": "name"
+                                    },
+                                    "type": "keyword"
+                                },
+                                "givenName": {
+                                    "type": "keyword"
+                                },
+                                "nameType": {
+                                    "enum": [
+                                        "Organizational"
+                                    ],
+                                    "label.cs": "Typ",
+                                    "label.en": "Type",
+                                    "sample": [
+                                        "Organizational"
+                                    ],
+                                    "type": "keyword"
                                 }
                             },
-                            "type": "object",
+                            "schemas": {
+                                "Organizational": {
+                                    "marshmallow": {
+                                        "class": "nr_metadata.common.services.records.schema_common.NRContributorOrganizationSchema",
+                                        "generate": true
+                                    },
+                                    "properties": {
+                                        "authorityIdentifiers": {
+                                            "items": {
+                                                "marshmallow": {
+                                                    "class": "nr_metadata.schema.identifiers.NROrganizationIdentifierSchema",
+                                                    "generate": false
+                                                },
+                                                "properties": {
+                                                    "identifier": {
+                                                        "i18n.key": "identifier",
+                                                        "label.cs": "Identifik\u00e1tor",
+                                                        "label.en": "Identifier",
+                                                        "required": true,
+                                                        "sample": {
+                                                            "faker": "isbn13"
+                                                        },
+                                                        "type": "keyword"
+                                                    },
+                                                    "scheme": {
+                                                        "enum": [
+                                                            "ISNI",
+                                                            "ROR",
+                                                            "ICO",
+                                                            "DOI"
+                                                        ],
+                                                        "hint.cs": "Doporu\u010dujeme zadat alespo\u0148 jeden z typ\u016f identifik\u00e1tor\u016f.\nPokud pot\u0159ebujete roz\u0161\u00ed\u0159it nab\u00eddku typ\u016f identifik\u00e1tor\u016f, kontaktujte n\u00e1s na support@narodni-repozitar.cz.\n",
+                                                        "hint.en": "We recommend providing at least one of the identifier types.\nIf you need to expand the range of identifier types, contact us at support@narodni-repozitar.cz.\n",
+                                                        "i18n.key": "identifier_type",
+                                                        "label.cs": "Typ identifik\u00e1toru",
+                                                        "label.en": "Identifier type",
+                                                        "required": true,
+                                                        "type": "keyword"
+                                                    }
+                                                },
+                                                "type": "object",
+                                                "ui": {
+                                                    "detail": "nr_organization_identifier",
+                                                    "marshmallow": {
+                                                        "class": "nr_metadata.ui_schema.identifiers.NROrganizationIdentifierUISchema",
+                                                        "generate": false
+                                                    }
+                                                }
+                                            },
+                                            "type": "array"
+                                        },
+                                        "contributorType": {
+                                            "facets": {
+                                                "args": [
+                                                    "vocabulary='contributor-types'"
+                                                ]
+                                            },
+                                            "imports": [
+                                                {
+                                                    "import": "invenio_vocabularies.records.api.Vocabulary"
+                                                }
+                                            ],
+                                            "keys": [
+                                                "id",
+                                                "title"
+                                            ],
+                                            "label.cs": "Typ p\u0159isp\u011bvatele",
+                                            "label.en": "Contributor's type",
+                                            "marshmallow": {
+                                                "class": "nr_metadata.common.services.records.schema_datatypes.NRContributorTypeVocabularySchema",
+                                                "generate": false,
+                                                "unknown": "INCLUDE"
+                                            },
+                                            "model": "vocabularies",
+                                            "pid-field": "Vocabulary.pid.with_type_ctx(\"contributor-types\")",
+                                            "properties": {},
+                                            "type": "vocabulary",
+                                            "ui": {
+                                                "detail": "vocabulary_item",
+                                                "edit": "vocabulary_item",
+                                                "marshmallow": {
+                                                    "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRContributorTypeVocabularyUISchema",
+                                                    "generate": false,
+                                                    "unknown": "INCLUDE"
+                                                }
+                                            },
+                                            "vocabulary-type": "contributor-types"
+                                        },
+                                        "fullName": {
+                                            "label.cs": "Jm\u00e9no p\u0159isp\u011bvatele",
+                                            "label.en": "Contributor name",
+                                            "required": true,
+                                            "sample": {
+                                                "faker": "name"
+                                            },
+                                            "type": "keyword"
+                                        },
+                                        "nameType": {
+                                            "enum": [
+                                                "Organizational"
+                                            ],
+                                            "label.cs": "Typ",
+                                            "label.en": "Type",
+                                            "sample": [
+                                                "Organizational"
+                                            ],
+                                            "type": "keyword"
+                                        }
+                                    },
+                                    "type": "object",
+                                    "ui": {
+                                        "detail": "nr_contributor_organization",
+                                        "marshmallow": {
+                                            "class": "nr_metadata.common.services.records.ui_schema_common.NRContributorOrganizationUISchema",
+                                            "generate": true
+                                        }
+                                    }
+                                },
+                                "Personal": {
+                                    "marshmallow": {
+                                        "class": "nr_metadata.common.services.records.schema_common.NRContributorPersonSchema",
+                                        "generate": true
+                                    },
+                                    "properties": {
+                                        "affiliations": {
+                                            "items": {
+                                                "facets": {
+                                                    "args": [
+                                                        "vocabulary='institutions'"
+                                                    ]
+                                                },
+                                                "hint.cs": "Uve\u010fte instituci/instituce, pod jej\u00ed\u017e z\u00e1\u0161titou jste se na tvorb\u011b objektu pod\u00edleli.",
+                                                "imports": [
+                                                    {
+                                                        "import": "invenio_vocabularies.records.api.Vocabulary"
+                                                    }
+                                                ],
+                                                "keys": [
+                                                    "id",
+                                                    "title",
+                                                    {
+                                                        "key": "props.ror",
+                                                        "model": {
+                                                            "type": "keyword"
+                                                        },
+                                                        "target": "ror"
+                                                    },
+                                                    {
+                                                        "key": "hierarchy",
+                                                        "model": {
+                                                            "marshmallow": {
+                                                                "class": "oarepo_vocabularies.services.schema.HierarchySchema",
+                                                                "generate": false,
+                                                                "imports": [
+                                                                    {
+                                                                        "import": "oarepo_vocabularies.services.schema.HierarchySchema"
+                                                                    }
+                                                                ]
+                                                            },
+                                                            "properties": {
+                                                                "ancestors": {
+                                                                    "items": {
+                                                                        "type": "keyword"
+                                                                    },
+                                                                    "type": "array"
+                                                                },
+                                                                "ancestors_or_self": {
+                                                                    "items": {
+                                                                        "type": "keyword"
+                                                                    },
+                                                                    "type": "array"
+                                                                },
+                                                                "level": {
+                                                                    "type": "integer"
+                                                                },
+                                                                "parent": {
+                                                                    "type": "keyword"
+                                                                },
+                                                                "title": {
+                                                                    "items": {
+                                                                        "additionalProperties": {
+                                                                            "type": "string"
+                                                                        },
+                                                                        "mapping": {
+                                                                            "dynamic": true
+                                                                        },
+                                                                        "marshmallow": {
+                                                                            "class": "nr_metadata.common.services.records.schema.TitleItemSchema",
+                                                                            "field": "i18n_strings",
+                                                                            "generate": true
+                                                                        },
+                                                                        "propertyNames": {
+                                                                            "pattern": "^[a-z]{2}$"
+                                                                        },
+                                                                        "type": "object",
+                                                                        "ui": {
+                                                                            "marshmallow": {
+                                                                                "class": "nr_metadata.common.services.records.ui_schema.TitleItemUISchema",
+                                                                                "field": "i18n_strings",
+                                                                                "generate": true
+                                                                            }
+                                                                        }
+                                                                    },
+                                                                    "type": "array"
+                                                                }
+                                                            },
+                                                            "type": "object",
+                                                            "ui": {
+                                                                "marshmallow": {
+                                                                    "class": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema",
+                                                                    "generate": false,
+                                                                    "imports": [
+                                                                        {
+                                                                            "import": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema"
+                                                                        }
+                                                                    ]
+                                                                }
+                                                            }
+                                                        },
+                                                        "target": "hierarchy"
+                                                    }
+                                                ],
+                                                "label.cs": "Afiliace",
+                                                "label.en": "Affiliation",
+                                                "marshmallow": {
+                                                    "class": "nr_metadata.common.services.records.schema_datatypes.NRAffiliationVocabularySchema",
+                                                    "generate": true,
+                                                    "unknown": "INCLUDE"
+                                                },
+                                                "model": "vocabularies",
+                                                "pid-field": "Vocabulary.pid.with_type_ctx(\"institutions\")",
+                                                "properties": {},
+                                                "sample": {
+                                                    "faker": "company"
+                                                },
+                                                "type": "taxonomy",
+                                                "ui": {
+                                                    "detail": "taxonomy_item",
+                                                    "edit": "taxonomy_item",
+                                                    "marshmallow": {
+                                                        "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRAffiliationVocabularyUISchema",
+                                                        "generate": true,
+                                                        "unknown": "INCLUDE"
+                                                    }
+                                                },
+                                                "vocabulary-type": "institutions"
+                                            },
+                                            "type": "array"
+                                        },
+                                        "authorityIdentifiers": {
+                                            "items": {
+                                                "marshmallow": {
+                                                    "class": "nr_metadata.schema.identifiers.NRPersonIdentifierSchema",
+                                                    "generate": false
+                                                },
+                                                "properties": {
+                                                    "identifier": {
+                                                        "i18n.key": "identifier",
+                                                        "label.cs": "Identifik\u00e1tor",
+                                                        "label.en": "Identifier",
+                                                        "required": true,
+                                                        "sample": {
+                                                            "faker": "isbn13"
+                                                        },
+                                                        "type": "keyword"
+                                                    },
+                                                    "scheme": {
+                                                        "enum": [
+                                                            "orcid",
+                                                            "scopusID",
+                                                            "researcherID",
+                                                            "czenasAutID",
+                                                            "vedidk",
+                                                            "institutionalID",
+                                                            "ISNI"
+                                                        ],
+                                                        "hint.cs": "Doporu\u010dujeme zadat alespo\u0148 jeden z typ\u016f identifik\u00e1tor\u016f.\nPokud pot\u0159ebujete roz\u0161\u00ed\u0159it nab\u00eddku typ\u016f identifik\u00e1tor\u016f, kontaktujte n\u00e1s na support@narodni-repozitar.cz.\n",
+                                                        "hint.en": "We recommend providing at least one of the identifier types.\nIf you need to expand the range of identifier types, contact us at support@narodni-repozitar.cz.\n",
+                                                        "i18n.key": "identifier_type",
+                                                        "label.cs": "Typ identifik\u00e1toru",
+                                                        "label.en": "Identifier type",
+                                                        "required": true,
+                                                        "type": "keyword"
+                                                    }
+                                                },
+                                                "type": "object",
+                                                "ui": {
+                                                    "detail": "nr_person_identifier",
+                                                    "marshmallow": {
+                                                        "class": "nr_metadata.ui_schema.identifiers.NRPersonIdentifierUISchema",
+                                                        "generate": false
+                                                    }
+                                                }
+                                            },
+                                            "type": "array"
+                                        },
+                                        "contributorType": {
+                                            "facets": {
+                                                "args": [
+                                                    "vocabulary='contributor-types'"
+                                                ]
+                                            },
+                                            "imports": [
+                                                {
+                                                    "import": "invenio_vocabularies.records.api.Vocabulary"
+                                                }
+                                            ],
+                                            "keys": [
+                                                "id",
+                                                "title"
+                                            ],
+                                            "label.cs": "Typ p\u0159isp\u011bvatele",
+                                            "label.en": "Contributor's type",
+                                            "marshmallow": {
+                                                "class": "nr_metadata.common.services.records.schema_datatypes.NRContributorTypeVocabularySchema",
+                                                "generate": true,
+                                                "unknown": "INCLUDE"
+                                            },
+                                            "model": "vocabularies",
+                                            "pid-field": "Vocabulary.pid.with_type_ctx(\"contributor-types\")",
+                                            "properties": {},
+                                            "type": "vocabulary",
+                                            "ui": {
+                                                "detail": "vocabulary_item",
+                                                "edit": "vocabulary_item",
+                                                "marshmallow": {
+                                                    "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRContributorTypeVocabularyUISchema",
+                                                    "generate": true,
+                                                    "unknown": "INCLUDE"
+                                                }
+                                            },
+                                            "vocabulary-type": "contributor-types"
+                                        },
+                                        "familyName": {
+                                            "type": "keyword"
+                                        },
+                                        "fullName": {
+                                            "label.cs": "Jm\u00e9no p\u0159isp\u011bvatele",
+                                            "label.en": "Contributor name",
+                                            "required": true,
+                                            "sample": {
+                                                "faker": "name"
+                                            },
+                                            "type": "keyword"
+                                        },
+                                        "givenName": {
+                                            "type": "keyword"
+                                        },
+                                        "nameType": {
+                                            "enum": [
+                                                "Personal"
+                                            ],
+                                            "label.cs": "Typ",
+                                            "label.en": "Type",
+                                            "type": "keyword"
+                                        }
+                                    },
+                                    "type": "object",
+                                    "ui": {
+                                        "detail": "nr_contributor_person",
+                                        "marshmallow": {
+                                            "class": "nr_metadata.common.services.records.ui_schema_common.NRContributorPersonUISchema",
+                                            "generate": true
+                                        }
+                                    }
+                                }
+                            },
+                            "type": "polymorphic",
                             "ui": {
                                 "detail": "contributor",
                                 "marshmallow": {
                                     "class": "nr_metadata.common.services.records.ui_schema_common.NRContributorUISchema",
                                     "generate": true
                                 }
                             }
                         },
                         "label.cs": "P\u0159isp\u011bvatel\u00e9",
                         "label.en": "Contributors",
                         "type": "array"
                     },
                     "creators": {
                         "items": {
+                            "discriminator": "nameType",
+                            "hint.cs": "Jako tv\u016frce je mo\u017en\u00e9 ozna\u010dit osobu nebo instituci.",
+                            "hint.en": "It is possible to designate a person or an institution as the creator/contributor.",
                             "marshmallow": {
                                 "class": "nr_metadata.common.services.records.schema_common.NRCreatorSchema",
                                 "generate": true
                             },
                             "properties": {
                                 "affiliations": {
                                     "items": {
@@ -967,14 +1351,21 @@
                                                 "import": "invenio_vocabularies.records.api.Vocabulary"
                                             }
                                         ],
                                         "keys": [
                                             "id",
                                             "title",
                                             {
+                                                "key": "props.ror",
+                                                "model": {
+                                                    "type": "keyword"
+                                                },
+                                                "target": "ror"
+                                            },
+                                            {
                                                 "key": "hierarchy",
                                                 "model": {
                                                     "marshmallow": {
                                                         "class": "oarepo_vocabularies.services.schema.HierarchySchema",
                                                         "generate": false,
                                                         "imports": [
                                                             {
@@ -1162,14 +1553,17 @@
                                                     "marshmallow": {
                                                         "field-class": "marshmallow.fields.String",
                                                         "imports": [],
                                                         "validators": []
                                                     }
                                                 }
                                             },
+                                            "ror": {
+                                                "type": "keyword"
+                                            },
                                             "title": {
                                                 "additionalProperties": {
                                                     "type": "string"
                                                 },
                                                 "mapping": {
                                                     "dynamic": true,
                                                     "properties": {
@@ -1214,15 +1608,15 @@
                                         "vocabulary-type": "institutions"
                                     },
                                     "type": "array"
                                 },
                                 "authorityIdentifiers": {
                                     "items": {
                                         "marshmallow": {
-                                            "class": "nr_metadata.schema.identifiers.NRAuthorityIdentifierSchema",
+                                            "class": "nr_metadata.schema.identifiers.NROrganizationIdentifierSchema",
                                             "generate": false
                                         },
                                         "properties": {
                                             "identifier": {
                                                 "i18n.key": "identifier",
                                                 "label.cs": "Identifik\u00e1tor",
                                                 "label.en": "Identifier",
@@ -1230,20 +1624,14 @@
                                                 "sample": {
                                                     "faker": "isbn13"
                                                 },
                                                 "type": "keyword"
                                             },
                                             "scheme": {
                                                 "enum": [
-                                                    "orcid",
-                                                    "scopusID",
-                                                    "researcherID",
-                                                    "czenasAutID",
-                                                    "vedidk",
-                                                    "institutionalID",
                                                     "ISNI",
                                                     "ROR",
                                                     "ICO",
                                                     "DOI"
                                                 ],
                                                 "hint.cs": "Doporu\u010dujeme zadat alespo\u0148 jeden z typ\u016f identifik\u00e1tor\u016f.\nPokud pot\u0159ebujete roz\u0161\u00ed\u0159it nab\u00eddku typ\u016f identifik\u00e1tor\u016f, kontaktujte n\u00e1s na support@narodni-repozitar.cz.\n",
                                                 "hint.en": "We recommend providing at least one of the identifier types.\nIf you need to expand the range of identifier types, contact us at support@narodni-repozitar.cz.\n",
@@ -1252,49 +1640,344 @@
                                                 "label.en": "Identifier type",
                                                 "required": true,
                                                 "type": "keyword"
                                             }
                                         },
                                         "type": "object",
                                         "ui": {
-                                            "detail": "nr_authority_identifier",
+                                            "detail": "nr_organization_identifier",
                                             "marshmallow": {
-                                                "class": "nr_metadata.ui_schema.identifiers.NRAuthorityIdentifierUISchema",
+                                                "class": "nr_metadata.ui_schema.identifiers.NROrganizationIdentifierUISchema",
                                                 "generate": false
                                             }
                                         }
                                     },
                                     "type": "array"
                                 },
+                                "familyName": {
+                                    "type": "keyword"
+                                },
                                 "fullName": {
                                     "label.cs": "Jm\u00e9no autora",
                                     "label.en": "Author name",
                                     "required": true,
                                     "sample": {
                                         "faker": "name"
                                     },
                                     "type": "keyword"
                                 },
+                                "givenName": {
+                                    "type": "keyword"
+                                },
                                 "nameType": {
                                     "enum": [
-                                        "Organizational",
-                                        "Personal"
+                                        "Organizational"
                                     ],
-                                    "hint.cs": "Jako tv\u016frce je mo\u017en\u00e9 ozna\u010dit osobu nebo instituci.",
-                                    "hint.en": "It is possible to designate a person or an institution as the creator/contributor.",
                                     "label.cs": "Typ",
                                     "label.en": "Type",
                                     "sample": [
-                                        "Organizational",
-                                        "Personal"
+                                        "Organizational"
                                     ],
                                     "type": "keyword"
                                 }
                             },
-                            "type": "object",
+                            "schemas": {
+                                "Organizational": {
+                                    "marshmallow": {
+                                        "class": "nr_metadata.common.services.records.schema_datatypes.NROrganizationSchema",
+                                        "generate": true
+                                    },
+                                    "properties": {
+                                        "authorityIdentifiers": {
+                                            "items": {
+                                                "marshmallow": {
+                                                    "class": "nr_metadata.schema.identifiers.NROrganizationIdentifierSchema",
+                                                    "generate": false
+                                                },
+                                                "properties": {
+                                                    "identifier": {
+                                                        "i18n.key": "identifier",
+                                                        "label.cs": "Identifik\u00e1tor",
+                                                        "label.en": "Identifier",
+                                                        "required": true,
+                                                        "sample": {
+                                                            "faker": "isbn13"
+                                                        },
+                                                        "type": "keyword"
+                                                    },
+                                                    "scheme": {
+                                                        "enum": [
+                                                            "ISNI",
+                                                            "ROR",
+                                                            "ICO",
+                                                            "DOI"
+                                                        ],
+                                                        "hint.cs": "Doporu\u010dujeme zadat alespo\u0148 jeden z typ\u016f identifik\u00e1tor\u016f.\nPokud pot\u0159ebujete roz\u0161\u00ed\u0159it nab\u00eddku typ\u016f identifik\u00e1tor\u016f, kontaktujte n\u00e1s na support@narodni-repozitar.cz.\n",
+                                                        "hint.en": "We recommend providing at least one of the identifier types.\nIf you need to expand the range of identifier types, contact us at support@narodni-repozitar.cz.\n",
+                                                        "i18n.key": "identifier_type",
+                                                        "label.cs": "Typ identifik\u00e1toru",
+                                                        "label.en": "Identifier type",
+                                                        "required": true,
+                                                        "type": "keyword"
+                                                    }
+                                                },
+                                                "type": "object",
+                                                "ui": {
+                                                    "detail": "nr_organization_identifier",
+                                                    "marshmallow": {
+                                                        "class": "nr_metadata.ui_schema.identifiers.NROrganizationIdentifierUISchema",
+                                                        "generate": false
+                                                    }
+                                                }
+                                            },
+                                            "type": "array"
+                                        },
+                                        "fullName": {
+                                            "label.cs": "Jm\u00e9no autora",
+                                            "label.en": "Author name",
+                                            "required": true,
+                                            "sample": {
+                                                "faker": "name"
+                                            },
+                                            "type": "keyword"
+                                        },
+                                        "nameType": {
+                                            "enum": [
+                                                "Organizational"
+                                            ],
+                                            "label.cs": "Typ",
+                                            "label.en": "Type",
+                                            "sample": [
+                                                "Organizational"
+                                            ],
+                                            "type": "keyword"
+                                        }
+                                    },
+                                    "type": "object",
+                                    "ui": {
+                                        "detail": "nr_organization",
+                                        "marshmallow": {
+                                            "class": "nr_metadata.common.services.records.ui_schema_datatypes.NROrganizationUISchema",
+                                            "generate": true
+                                        }
+                                    }
+                                },
+                                "Personal": {
+                                    "marshmallow": {
+                                        "class": "nr_metadata.common.services.records.schema_datatypes.NRPersonSchema",
+                                        "generate": true
+                                    },
+                                    "properties": {
+                                        "affiliations": {
+                                            "items": {
+                                                "facets": {
+                                                    "args": [
+                                                        "vocabulary='institutions'"
+                                                    ]
+                                                },
+                                                "hint.cs": "Uve\u010fte instituci/instituce, pod jej\u00ed\u017e z\u00e1\u0161titou jste se na tvorb\u011b objektu pod\u00edleli.",
+                                                "imports": [
+                                                    {
+                                                        "import": "invenio_vocabularies.records.api.Vocabulary"
+                                                    }
+                                                ],
+                                                "keys": [
+                                                    "id",
+                                                    "title",
+                                                    {
+                                                        "key": "props.ror",
+                                                        "model": {
+                                                            "type": "keyword"
+                                                        },
+                                                        "target": "ror"
+                                                    },
+                                                    {
+                                                        "key": "hierarchy",
+                                                        "model": {
+                                                            "marshmallow": {
+                                                                "class": "oarepo_vocabularies.services.schema.HierarchySchema",
+                                                                "generate": false,
+                                                                "imports": [
+                                                                    {
+                                                                        "import": "oarepo_vocabularies.services.schema.HierarchySchema"
+                                                                    }
+                                                                ]
+                                                            },
+                                                            "properties": {
+                                                                "ancestors": {
+                                                                    "items": {
+                                                                        "type": "keyword"
+                                                                    },
+                                                                    "type": "array"
+                                                                },
+                                                                "ancestors_or_self": {
+                                                                    "items": {
+                                                                        "type": "keyword"
+                                                                    },
+                                                                    "type": "array"
+                                                                },
+                                                                "level": {
+                                                                    "type": "integer"
+                                                                },
+                                                                "parent": {
+                                                                    "type": "keyword"
+                                                                },
+                                                                "title": {
+                                                                    "items": {
+                                                                        "additionalProperties": {
+                                                                            "type": "string"
+                                                                        },
+                                                                        "mapping": {
+                                                                            "dynamic": true
+                                                                        },
+                                                                        "marshmallow": {
+                                                                            "class": "nr_metadata.common.services.records.schema.TitleItemSchema",
+                                                                            "field": "i18n_strings",
+                                                                            "generate": false
+                                                                        },
+                                                                        "propertyNames": {
+                                                                            "pattern": "^[a-z]{2}$"
+                                                                        },
+                                                                        "type": "object",
+                                                                        "ui": {
+                                                                            "marshmallow": {
+                                                                                "class": "nr_metadata.common.services.records.ui_schema.TitleItemUISchema",
+                                                                                "field": "i18n_strings",
+                                                                                "generate": false
+                                                                            }
+                                                                        }
+                                                                    },
+                                                                    "type": "array"
+                                                                }
+                                                            },
+                                                            "type": "object",
+                                                            "ui": {
+                                                                "marshmallow": {
+                                                                    "class": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema",
+                                                                    "generate": false,
+                                                                    "imports": [
+                                                                        {
+                                                                            "import": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema"
+                                                                        }
+                                                                    ]
+                                                                }
+                                                            }
+                                                        },
+                                                        "target": "hierarchy"
+                                                    }
+                                                ],
+                                                "label.cs": "Afiliace",
+                                                "label.en": "Affiliation",
+                                                "marshmallow": {
+                                                    "class": "nr_metadata.common.services.records.schema_datatypes.NRAffiliationVocabularySchema",
+                                                    "generate": false,
+                                                    "unknown": "INCLUDE"
+                                                },
+                                                "model": "vocabularies",
+                                                "pid-field": "Vocabulary.pid.with_type_ctx(\"institutions\")",
+                                                "properties": {},
+                                                "sample": {
+                                                    "faker": "company"
+                                                },
+                                                "type": "taxonomy",
+                                                "ui": {
+                                                    "detail": "taxonomy_item",
+                                                    "edit": "taxonomy_item",
+                                                    "marshmallow": {
+                                                        "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRAffiliationVocabularyUISchema",
+                                                        "generate": false,
+                                                        "unknown": "INCLUDE"
+                                                    }
+                                                },
+                                                "vocabulary-type": "institutions"
+                                            },
+                                            "type": "array"
+                                        },
+                                        "authorityIdentifiers": {
+                                            "items": {
+                                                "marshmallow": {
+                                                    "class": "nr_metadata.schema.identifiers.NRPersonIdentifierSchema",
+                                                    "generate": false
+                                                },
+                                                "properties": {
+                                                    "identifier": {
+                                                        "i18n.key": "identifier",
+                                                        "label.cs": "Identifik\u00e1tor",
+                                                        "label.en": "Identifier",
+                                                        "required": true,
+                                                        "sample": {
+                                                            "faker": "isbn13"
+                                                        },
+                                                        "type": "keyword"
+                                                    },
+                                                    "scheme": {
+                                                        "enum": [
+                                                            "orcid",
+                                                            "scopusID",
+                                                            "researcherID",
+                                                            "czenasAutID",
+                                                            "vedidk",
+                                                            "institutionalID",
+                                                            "ISNI"
+                                                        ],
+                                                        "hint.cs": "Doporu\u010dujeme zadat alespo\u0148 jeden z typ\u016f identifik\u00e1tor\u016f.\nPokud pot\u0159ebujete roz\u0161\u00ed\u0159it nab\u00eddku typ\u016f identifik\u00e1tor\u016f, kontaktujte n\u00e1s na support@narodni-repozitar.cz.\n",
+                                                        "hint.en": "We recommend providing at least one of the identifier types.\nIf you need to expand the range of identifier types, contact us at support@narodni-repozitar.cz.\n",
+                                                        "i18n.key": "identifier_type",
+                                                        "label.cs": "Typ identifik\u00e1toru",
+                                                        "label.en": "Identifier type",
+                                                        "required": true,
+                                                        "type": "keyword"
+                                                    }
+                                                },
+                                                "type": "object",
+                                                "ui": {
+                                                    "detail": "nr_person_identifier",
+                                                    "marshmallow": {
+                                                        "class": "nr_metadata.ui_schema.identifiers.NRPersonIdentifierUISchema",
+                                                        "generate": false
+                                                    }
+                                                }
+                                            },
+                                            "type": "array"
+                                        },
+                                        "familyName": {
+                                            "type": "keyword"
+                                        },
+                                        "fullName": {
+                                            "label.cs": "Jm\u00e9no autora",
+                                            "label.en": "Author name",
+                                            "required": true,
+                                            "sample": {
+                                                "faker": "name"
+                                            },
+                                            "type": "keyword"
+                                        },
+                                        "givenName": {
+                                            "type": "keyword"
+                                        },
+                                        "nameType": {
+                                            "enum": [
+                                                "Personal"
+                                            ],
+                                            "label.cs": "Typ",
+                                            "label.en": "Type",
+                                            "type": "keyword"
+                                        }
+                                    },
+                                    "type": "object",
+                                    "ui": {
+                                        "detail": "nr_person",
+                                        "marshmallow": {
+                                            "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRPersonUISchema",
+                                            "generate": true
+                                        }
+                                    }
+                                }
+                            },
+                            "type": "polymorphic",
                             "ui": {
                                 "detail": "creator",
                                 "marshmallow": {
                                     "class": "nr_metadata.common.services.records.ui_schema_common.NRCreatorUISchema",
                                     "generate": true
                                 }
                             }
@@ -1312,32 +1995,24 @@
                     },
                     "dateAvailable": {
                         "label.cs": "Datum zve\u0159ejn\u011bn\u00ed",
                         "label.en": "Date available",
                         "sample": {
                             "faker": "date"
                         },
-                        "type": "edtf"
+                        "type": "date"
                     },
                     "dateIssued": {
                         "label.cs": "Datum vyd\u00e1n\u00ed",
                         "label.en": "Date issued",
                         "sample": {
                             "faker": "date"
                         },
                         "type": "edtf"
                     },
-                    "dateModified": {
-                        "label.cs": "Datum zm\u011bny zdroje",
-                        "label.en": "Date modified",
-                        "sample": {
-                            "faker": "date"
-                        },
-                        "type": "edtf"
-                    },
                     "events": {
                         "items": {
                             "label.cs": "Ud\u00e1lost",
                             "label.en": "Event",
                             "marshmallow": {
                                 "class": "nr_metadata.common.services.records.schema_datatypes.NREventSchema",
                                 "generate": true
@@ -1508,46 +2183,14 @@
                                 }
                             }
                         },
                         "label.cs": "Ud\u00e1losti",
                         "label.en": "Events",
                         "type": "array"
                     },
-                    "externalLocation": {
-                        "label.cs": "Extern\u00ed um\u00edst\u011bn\u00ed",
-                        "label.en": "External location",
-                        "marshmallow": {
-                            "class": "nr_metadata.common.services.records.schema_datatypes.NRExternalLocationSchema",
-                            "generate": true
-                        },
-                        "properties": {
-                            "externalLocationNote": {
-                                "label.cs": "Pozn\u00e1mka",
-                                "label.en": "Note",
-                                "type": "fulltext"
-                            },
-                            "externalLocationURL": {
-                                "label.cs": "Extern\u00ed um\u00edst\u011bn\u00ed zdroje",
-                                "label.en": "Resource external location",
-                                "required": true,
-                                "sample": {
-                                    "faker": "url"
-                                },
-                                "type": "url"
-                            }
-                        },
-                        "type": "object",
-                        "ui": {
-                            "detail": "external_location",
-                            "marshmallow": {
-                                "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRExternalLocationUISchema",
-                                "generate": true
-                            }
-                        }
-                    },
                     "fundingReferences": {
                         "items": {
                             "label.cs": "Projekt nebo financov\u00e1n\u00ed",
                             "label.en": "Funding",
                             "marshmallow": {
                                 "class": "nr_metadata.common.services.records.schema_datatypes.NRFundingReferenceSchema",
                                 "generate": true
@@ -1700,15 +2343,14 @@
                             "marshmallow": {
                                 "class": "nr_metadata.common.services.records.schema_datatypes.NRGeoLocationSchema",
                                 "generate": true
                             },
                             "properties": {
                                 "geoLocationPlace": {
                                     "description": "Free description of the location; ie. Atlantic Ocean",
-                                    "required": true,
                                     "type": "keyword"
                                 },
                                 "geoLocationPoint": {
                                     "marshmallow": {
                                         "class": "nr_metadata.common.services.records.schema_datatypes.NRGeoLocationPointSchema",
                                         "generate": true
                                     },
@@ -1879,21 +2521,14 @@
                                     "unknown": "INCLUDE"
                                 }
                             },
                             "vocabulary-type": "languages"
                         },
                         "label.cs": "Jazyk",
                         "label.en": "Language",
-                        "marshmallow": {
-                            "validators": [
-                                "ma.validate.Length(min=1)"
-                            ]
-                        },
-                        "minItems": 1,
-                        "required": true,
                         "type": "array"
                     },
                     "methods": {
                         "items": {
                             "marshmallow": {
                                 "class": null,
                                 "field-class": "oarepo_runtime.services.schema.i18n.I18nStrField",
@@ -1963,15 +2598,16 @@
                                 },
                                 "scheme": {
                                     "enum": [
                                         "DOI",
                                         "Handle",
                                         "ISBN",
                                         "ISSN",
-                                        "RIV"
+                                        "RIV",
+                                        "IGSN"
                                     ],
                                     "label.cs": "Typ identifik\u00e1toru",
                                     "label.en": "Identifier type",
                                     "required": true,
                                     "type": "keyword"
                                 }
                             },
@@ -1992,37 +2628,29 @@
                         "label.cs": "Odkaz na p\u016fvodn\u00ed z\u00e1znam",
                         "label.en": "Original record URL",
                         "sample": {
                             "faker": "url"
                         },
                         "type": "url"
                     },
-                    "publishers": {
-                        "items": {
-                            "sample": {
-                                "faker": "company"
-                            },
-                            "type": "fulltext"
-                        },
-                        "label.cs": "Vydavatel\u00e9",
-                        "label.en": "Publishers",
-                        "type": "array"
-                    },
                     "relatedItems": {
                         "items": {
                             "description": "linkdata, propojen\u00ed p\u0159idru\u017een\u00fdch dokument\u016f a dataset\u016f.",
                             "label.cs": "Vazba na/z dal\u0161\u00edch zdroj\u016f:",
                             "label.en": "Link to/from other resources:",
                             "marshmallow": {
                                 "class": "nr_metadata.common.services.records.schema_datatypes.NRRelatedItemSchema",
                                 "generate": true
                             },
                             "properties": {
                                 "itemContributors": {
                                     "items": {
+                                        "discriminator": "nameType",
+                                        "hint.cs": "Jako tv\u016frce je mo\u017en\u00e9 ozna\u010dit osobu nebo instituci.",
+                                        "hint.en": "It is possible to designate a person or an institution as the creator/contributor.",
                                         "marshmallow": {
                                             "class": "nr_metadata.common.services.records.schema_datatypes.NRRelatedItemContributorSchema",
                                             "generate": true
                                         },
                                         "properties": {
                                             "affiliations": {
                                                 "items": {
@@ -2037,14 +2665,21 @@
                                                             "import": "invenio_vocabularies.records.api.Vocabulary"
                                                         }
                                                     ],
                                                     "keys": [
                                                         "id",
                                                         "title",
                                                         {
+                                                            "key": "props.ror",
+                                                            "model": {
+                                                                "type": "keyword"
+                                                            },
+                                                            "target": "ror"
+                                                        },
+                                                        {
                                                             "key": "hierarchy",
                                                             "model": {
                                                                 "marshmallow": {
                                                                     "class": "oarepo_vocabularies.services.schema.HierarchySchema",
                                                                     "generate": false,
                                                                     "imports": [
                                                                         {
@@ -2232,14 +2867,17 @@
                                                                 "marshmallow": {
                                                                     "field-class": "marshmallow.fields.String",
                                                                     "imports": [],
                                                                     "validators": []
                                                                 }
                                                             }
                                                         },
+                                                        "ror": {
+                                                            "type": "keyword"
+                                                        },
                                                         "title": {
                                                             "additionalProperties": {
                                                                 "type": "string"
                                                             },
                                                             "mapping": {
                                                                 "dynamic": true,
                                                                 "properties": {
@@ -2279,22 +2917,20 @@
                                                             "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRAffiliationVocabularyUISchema",
                                                             "generate": false,
                                                             "unknown": "INCLUDE"
                                                         }
                                                     },
                                                     "vocabulary-type": "institutions"
                                                 },
-                                                "label.cs": "Afiliace",
-                                                "label.en": "Affiliation",
                                                 "type": "array"
                                             },
                                             "authorityIdentifiers": {
                                                 "items": {
                                                     "marshmallow": {
-                                                        "class": "nr_metadata.schema.identifiers.NRAuthorityIdentifierSchema",
+                                                        "class": "nr_metadata.schema.identifiers.NROrganizationIdentifierSchema",
                                                         "generate": false
                                                     },
                                                     "properties": {
                                                         "identifier": {
                                                             "i18n.key": "identifier",
                                                             "label.cs": "Identifik\u00e1tor",
                                                             "label.en": "Identifier",
@@ -2302,20 +2938,14 @@
                                                             "sample": {
                                                                 "faker": "isbn13"
                                                             },
                                                             "type": "keyword"
                                                         },
                                                         "scheme": {
                                                             "enum": [
-                                                                "orcid",
-                                                                "scopusID",
-                                                                "researcherID",
-                                                                "czenasAutID",
-                                                                "vedidk",
-                                                                "institutionalID",
                                                                 "ISNI",
                                                                 "ROR",
                                                                 "ICO",
                                                                 "DOI"
                                                             ],
                                                             "hint.cs": "Doporu\u010dujeme zadat alespo\u0148 jeden z typ\u016f identifik\u00e1tor\u016f.\nPokud pot\u0159ebujete roz\u0161\u00ed\u0159it nab\u00eddku typ\u016f identifik\u00e1tor\u016f, kontaktujte n\u00e1s na support@narodni-repozitar.cz.\n",
                                                             "hint.en": "We recommend providing at least one of the identifier types.\nIf you need to expand the range of identifier types, contact us at support@narodni-repozitar.cz.\n",
@@ -2324,71 +2954,47 @@
                                                             "label.en": "Identifier type",
                                                             "required": true,
                                                             "type": "keyword"
                                                         }
                                                     },
                                                     "type": "object",
                                                     "ui": {
-                                                        "detail": "nr_authority_identifier",
+                                                        "detail": "nr_organization_identifier",
                                                         "marshmallow": {
-                                                            "class": "nr_metadata.ui_schema.identifiers.NRAuthorityIdentifierUISchema",
+                                                            "class": "nr_metadata.ui_schema.identifiers.NROrganizationIdentifierUISchema",
                                                             "generate": false
                                                         }
                                                     }
                                                 },
                                                 "type": "array"
                                             },
-                                            "fullName": {
-                                                "label.cs": "Jm\u00e9no autora",
-                                                "label.en": "Author name",
-                                                "required": true,
-                                                "sample": {
-                                                    "faker": "name"
-                                                },
-                                                "type": "keyword"
-                                            },
-                                            "nameType": {
-                                                "enum": [
-                                                    "Organizational",
-                                                    "Personal"
-                                                ],
-                                                "hint.cs": "Jako tv\u016frce je mo\u017en\u00e9 ozna\u010dit osobu nebo instituci.",
-                                                "hint.en": "It is possible to designate a person or an institution as the creator/contributor.",
-                                                "label.cs": "Typ",
-                                                "label.en": "Type",
-                                                "sample": [
-                                                    "Organizational",
-                                                    "Personal"
-                                                ],
-                                                "type": "keyword"
-                                            },
-                                            "role": {
+                                            "contributorType": {
                                                 "facets": {
                                                     "args": [
-                                                        "vocabulary='contributor-roles'"
+                                                        "vocabulary='contributor-types'"
                                                     ]
                                                 },
                                                 "imports": [
                                                     {
                                                         "import": "invenio_vocabularies.records.api.Vocabulary"
                                                     }
                                                 ],
                                                 "keys": [
                                                     "id",
                                                     "title"
                                                 ],
-                                                "label.cs": "Role p\u0159isp\u011bvatele",
-                                                "label.en": "Contributor's role",
+                                                "label.cs": "Typ p\u0159isp\u011bvatele",
+                                                "label.en": "Contributor's type",
                                                 "marshmallow": {
-                                                    "class": "nr_metadata.common.services.records.schema_datatypes.NRAuthorityRoleVocabularySchema",
+                                                    "class": "nr_metadata.common.services.records.schema_datatypes.NRContributorTypeVocabularySchema",
                                                     "generate": false,
                                                     "unknown": "INCLUDE"
                                                 },
                                                 "model": "vocabularies",
-                                                "pid-field": "Vocabulary.pid.with_type_ctx(\"contributor-roles\")",
+                                                "pid-field": "Vocabulary.pid.with_type_ctx(\"contributor-types\")",
                                                 "properties": {
                                                     "@v": {
                                                         "facets": {
                                                             "facet": false
                                                         },
                                                         "marshmallow": {
                                                             "field-class": "marshmallow.fields.String",
@@ -2460,37 +3066,433 @@
                                                     }
                                                 },
                                                 "type": "vocabulary",
                                                 "ui": {
                                                     "detail": "vocabulary_item",
                                                     "edit": "vocabulary_item",
                                                     "marshmallow": {
-                                                        "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRAuthorityRoleVocabularyUISchema",
+                                                        "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRContributorTypeVocabularyUISchema",
                                                         "generate": false,
                                                         "unknown": "INCLUDE"
                                                     }
                                                 },
-                                                "vocabulary-type": "contributor-roles"
+                                                "vocabulary-type": "contributor-types"
+                                            },
+                                            "familyName": {
+                                                "type": "keyword"
+                                            },
+                                            "fullName": {
+                                                "label.cs": "Jm\u00e9no autora",
+                                                "label.en": "Author name",
+                                                "required": true,
+                                                "sample": {
+                                                    "faker": "name"
+                                                },
+                                                "type": "keyword"
+                                            },
+                                            "givenName": {
+                                                "type": "keyword"
+                                            },
+                                            "nameType": {
+                                                "enum": [
+                                                    "Organizational"
+                                                ],
+                                                "label.cs": "Typ",
+                                                "label.en": "Type",
+                                                "sample": [
+                                                    "Organizational"
+                                                ],
+                                                "type": "keyword"
                                             }
                                         },
-                                        "type": "object",
+                                        "schemas": {
+                                            "Organizational": {
+                                                "marshmallow": {
+                                                    "class": "nr_metadata.common.services.records.schema_datatypes.NRRelatedItemContributorOrganizationSchema",
+                                                    "generate": true
+                                                },
+                                                "properties": {
+                                                    "authorityIdentifiers": {
+                                                        "items": {
+                                                            "marshmallow": {
+                                                                "class": "nr_metadata.schema.identifiers.NROrganizationIdentifierSchema",
+                                                                "generate": false
+                                                            },
+                                                            "properties": {
+                                                                "identifier": {
+                                                                    "i18n.key": "identifier",
+                                                                    "label.cs": "Identifik\u00e1tor",
+                                                                    "label.en": "Identifier",
+                                                                    "required": true,
+                                                                    "sample": {
+                                                                        "faker": "isbn13"
+                                                                    },
+                                                                    "type": "keyword"
+                                                                },
+                                                                "scheme": {
+                                                                    "enum": [
+                                                                        "ISNI",
+                                                                        "ROR",
+                                                                        "ICO",
+                                                                        "DOI"
+                                                                    ],
+                                                                    "hint.cs": "Doporu\u010dujeme zadat alespo\u0148 jeden z typ\u016f identifik\u00e1tor\u016f.\nPokud pot\u0159ebujete roz\u0161\u00ed\u0159it nab\u00eddku typ\u016f identifik\u00e1tor\u016f, kontaktujte n\u00e1s na support@narodni-repozitar.cz.\n",
+                                                                    "hint.en": "We recommend providing at least one of the identifier types.\nIf you need to expand the range of identifier types, contact us at support@narodni-repozitar.cz.\n",
+                                                                    "i18n.key": "identifier_type",
+                                                                    "label.cs": "Typ identifik\u00e1toru",
+                                                                    "label.en": "Identifier type",
+                                                                    "required": true,
+                                                                    "type": "keyword"
+                                                                }
+                                                            },
+                                                            "type": "object",
+                                                            "ui": {
+                                                                "detail": "nr_organization_identifier",
+                                                                "marshmallow": {
+                                                                    "class": "nr_metadata.ui_schema.identifiers.NROrganizationIdentifierUISchema",
+                                                                    "generate": false
+                                                                }
+                                                            }
+                                                        },
+                                                        "type": "array"
+                                                    },
+                                                    "contributorType": {
+                                                        "facets": {
+                                                            "args": [
+                                                                "vocabulary='contributor-types'"
+                                                            ]
+                                                        },
+                                                        "imports": [
+                                                            {
+                                                                "import": "invenio_vocabularies.records.api.Vocabulary"
+                                                            }
+                                                        ],
+                                                        "keys": [
+                                                            "id",
+                                                            "title"
+                                                        ],
+                                                        "label.cs": "Typ p\u0159isp\u011bvatele",
+                                                        "label.en": "Contributor's type",
+                                                        "marshmallow": {
+                                                            "class": "nr_metadata.common.services.records.schema_datatypes.NRContributorTypeVocabularySchema",
+                                                            "generate": false,
+                                                            "unknown": "INCLUDE"
+                                                        },
+                                                        "model": "vocabularies",
+                                                        "pid-field": "Vocabulary.pid.with_type_ctx(\"contributor-types\")",
+                                                        "properties": {},
+                                                        "type": "vocabulary",
+                                                        "ui": {
+                                                            "detail": "vocabulary_item",
+                                                            "edit": "vocabulary_item",
+                                                            "marshmallow": {
+                                                                "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRContributorTypeVocabularyUISchema",
+                                                                "generate": false,
+                                                                "unknown": "INCLUDE"
+                                                            }
+                                                        },
+                                                        "vocabulary-type": "contributor-types"
+                                                    },
+                                                    "fullName": {
+                                                        "label.cs": "Jm\u00e9no autora",
+                                                        "label.en": "Author name",
+                                                        "required": true,
+                                                        "sample": {
+                                                            "faker": "name"
+                                                        },
+                                                        "type": "keyword"
+                                                    },
+                                                    "nameType": {
+                                                        "enum": [
+                                                            "Organizational"
+                                                        ],
+                                                        "label.cs": "Typ",
+                                                        "label.en": "Type",
+                                                        "sample": [
+                                                            "Organizational"
+                                                        ],
+                                                        "type": "keyword"
+                                                    }
+                                                },
+                                                "type": "object",
+                                                "ui": {
+                                                    "detail": "nr_contributor_organization",
+                                                    "marshmallow": {
+                                                        "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRRelatedItemContributorOrganizationUISchema",
+                                                        "generate": true
+                                                    }
+                                                }
+                                            },
+                                            "Personal": {
+                                                "marshmallow": {
+                                                    "class": "nr_metadata.common.services.records.schema_datatypes.NRRelatedItemContributorPersonSchema",
+                                                    "generate": true
+                                                },
+                                                "properties": {
+                                                    "affiliations": {
+                                                        "items": {
+                                                            "facets": {
+                                                                "args": [
+                                                                    "vocabulary='institutions'"
+                                                                ]
+                                                            },
+                                                            "hint.cs": "Uve\u010fte instituci/instituce, pod jej\u00ed\u017e z\u00e1\u0161titou jste se na tvorb\u011b objektu pod\u00edleli.",
+                                                            "imports": [
+                                                                {
+                                                                    "import": "invenio_vocabularies.records.api.Vocabulary"
+                                                                }
+                                                            ],
+                                                            "keys": [
+                                                                "id",
+                                                                "title",
+                                                                {
+                                                                    "key": "props.ror",
+                                                                    "model": {
+                                                                        "type": "keyword"
+                                                                    },
+                                                                    "target": "ror"
+                                                                },
+                                                                {
+                                                                    "key": "hierarchy",
+                                                                    "model": {
+                                                                        "marshmallow": {
+                                                                            "class": "oarepo_vocabularies.services.schema.HierarchySchema",
+                                                                            "generate": false,
+                                                                            "imports": [
+                                                                                {
+                                                                                    "import": "oarepo_vocabularies.services.schema.HierarchySchema"
+                                                                                }
+                                                                            ]
+                                                                        },
+                                                                        "properties": {
+                                                                            "ancestors": {
+                                                                                "items": {
+                                                                                    "type": "keyword"
+                                                                                },
+                                                                                "type": "array"
+                                                                            },
+                                                                            "ancestors_or_self": {
+                                                                                "items": {
+                                                                                    "type": "keyword"
+                                                                                },
+                                                                                "type": "array"
+                                                                            },
+                                                                            "level": {
+                                                                                "type": "integer"
+                                                                            },
+                                                                            "parent": {
+                                                                                "type": "keyword"
+                                                                            },
+                                                                            "title": {
+                                                                                "items": {
+                                                                                    "additionalProperties": {
+                                                                                        "type": "string"
+                                                                                    },
+                                                                                    "mapping": {
+                                                                                        "dynamic": true
+                                                                                    },
+                                                                                    "marshmallow": {
+                                                                                        "class": "nr_metadata.common.services.records.schema.TitleItemSchema",
+                                                                                        "field": "i18n_strings",
+                                                                                        "generate": false
+                                                                                    },
+                                                                                    "propertyNames": {
+                                                                                        "pattern": "^[a-z]{2}$"
+                                                                                    },
+                                                                                    "type": "object",
+                                                                                    "ui": {
+                                                                                        "marshmallow": {
+                                                                                            "class": "nr_metadata.common.services.records.ui_schema.TitleItemUISchema",
+                                                                                            "field": "i18n_strings",
+                                                                                            "generate": false
+                                                                                        }
+                                                                                    }
+                                                                                },
+                                                                                "type": "array"
+                                                                            }
+                                                                        },
+                                                                        "type": "object",
+                                                                        "ui": {
+                                                                            "marshmallow": {
+                                                                                "class": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema",
+                                                                                "generate": false,
+                                                                                "imports": [
+                                                                                    {
+                                                                                        "import": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema"
+                                                                                    }
+                                                                                ]
+                                                                            }
+                                                                        }
+                                                                    },
+                                                                    "target": "hierarchy"
+                                                                }
+                                                            ],
+                                                            "label.cs": "Afiliace",
+                                                            "label.en": "Affiliation",
+                                                            "marshmallow": {
+                                                                "class": "nr_metadata.common.services.records.schema_datatypes.NRAffiliationVocabularySchema",
+                                                                "generate": false,
+                                                                "unknown": "INCLUDE"
+                                                            },
+                                                            "model": "vocabularies",
+                                                            "pid-field": "Vocabulary.pid.with_type_ctx(\"institutions\")",
+                                                            "properties": {},
+                                                            "sample": {
+                                                                "faker": "company"
+                                                            },
+                                                            "type": "taxonomy",
+                                                            "ui": {
+                                                                "detail": "taxonomy_item",
+                                                                "edit": "taxonomy_item",
+                                                                "marshmallow": {
+                                                                    "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRAffiliationVocabularyUISchema",
+                                                                    "generate": false,
+                                                                    "unknown": "INCLUDE"
+                                                                }
+                                                            },
+                                                            "vocabulary-type": "institutions"
+                                                        },
+                                                        "type": "array"
+                                                    },
+                                                    "authorityIdentifiers": {
+                                                        "items": {
+                                                            "marshmallow": {
+                                                                "class": "nr_metadata.schema.identifiers.NRPersonIdentifierSchema",
+                                                                "generate": false
+                                                            },
+                                                            "properties": {
+                                                                "identifier": {
+                                                                    "i18n.key": "identifier",
+                                                                    "label.cs": "Identifik\u00e1tor",
+                                                                    "label.en": "Identifier",
+                                                                    "required": true,
+                                                                    "sample": {
+                                                                        "faker": "isbn13"
+                                                                    },
+                                                                    "type": "keyword"
+                                                                },
+                                                                "scheme": {
+                                                                    "enum": [
+                                                                        "orcid",
+                                                                        "scopusID",
+                                                                        "researcherID",
+                                                                        "czenasAutID",
+                                                                        "vedidk",
+                                                                        "institutionalID",
+                                                                        "ISNI"
+                                                                    ],
+                                                                    "hint.cs": "Doporu\u010dujeme zadat alespo\u0148 jeden z typ\u016f identifik\u00e1tor\u016f.\nPokud pot\u0159ebujete roz\u0161\u00ed\u0159it nab\u00eddku typ\u016f identifik\u00e1tor\u016f, kontaktujte n\u00e1s na support@narodni-repozitar.cz.\n",
+                                                                    "hint.en": "We recommend providing at least one of the identifier types.\nIf you need to expand the range of identifier types, contact us at support@narodni-repozitar.cz.\n",
+                                                                    "i18n.key": "identifier_type",
+                                                                    "label.cs": "Typ identifik\u00e1toru",
+                                                                    "label.en": "Identifier type",
+                                                                    "required": true,
+                                                                    "type": "keyword"
+                                                                }
+                                                            },
+                                                            "type": "object",
+                                                            "ui": {
+                                                                "detail": "nr_person_identifier",
+                                                                "marshmallow": {
+                                                                    "class": "nr_metadata.ui_schema.identifiers.NRPersonIdentifierUISchema",
+                                                                    "generate": false
+                                                                }
+                                                            }
+                                                        },
+                                                        "type": "array"
+                                                    },
+                                                    "contributorType": {
+                                                        "facets": {
+                                                            "args": [
+                                                                "vocabulary='contributor-types'"
+                                                            ]
+                                                        },
+                                                        "imports": [
+                                                            {
+                                                                "import": "invenio_vocabularies.records.api.Vocabulary"
+                                                            }
+                                                        ],
+                                                        "keys": [
+                                                            "id",
+                                                            "title"
+                                                        ],
+                                                        "label.cs": "Typ p\u0159isp\u011bvatele",
+                                                        "label.en": "Contributor's type",
+                                                        "marshmallow": {
+                                                            "class": "nr_metadata.common.services.records.schema_datatypes.NRContributorTypeVocabularySchema",
+                                                            "generate": false,
+                                                            "unknown": "INCLUDE"
+                                                        },
+                                                        "model": "vocabularies",
+                                                        "pid-field": "Vocabulary.pid.with_type_ctx(\"contributor-types\")",
+                                                        "properties": {},
+                                                        "type": "vocabulary",
+                                                        "ui": {
+                                                            "detail": "vocabulary_item",
+                                                            "edit": "vocabulary_item",
+                                                            "marshmallow": {
+                                                                "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRContributorTypeVocabularyUISchema",
+                                                                "generate": false,
+                                                                "unknown": "INCLUDE"
+                                                            }
+                                                        },
+                                                        "vocabulary-type": "contributor-types"
+                                                    },
+                                                    "familyName": {
+                                                        "type": "keyword"
+                                                    },
+                                                    "fullName": {
+                                                        "label.cs": "Jm\u00e9no autora",
+                                                        "label.en": "Author name",
+                                                        "required": true,
+                                                        "sample": {
+                                                            "faker": "name"
+                                                        },
+                                                        "type": "keyword"
+                                                    },
+                                                    "givenName": {
+                                                        "type": "keyword"
+                                                    },
+                                                    "nameType": {
+                                                        "enum": [
+                                                            "Personal"
+                                                        ],
+                                                        "label.cs": "Typ",
+                                                        "label.en": "Type",
+                                                        "type": "keyword"
+                                                    }
+                                                },
+                                                "type": "object",
+                                                "ui": {
+                                                    "detail": "nr_contributor_person",
+                                                    "marshmallow": {
+                                                        "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRRelatedItemContributorPersonUISchema",
+                                                        "generate": true
+                                                    }
+                                                }
+                                            }
+                                        },
+                                        "type": "polymorphic",
                                         "ui": {
                                             "detail": "contributor",
                                             "marshmallow": {
                                                 "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRRelatedItemContributorUISchema",
                                                 "generate": true
                                             }
                                         }
                                     },
                                     "label.cs": "P\u0159isp\u011bvatel\u00e9",
                                     "label.en": "Contributors",
                                     "type": "array"
                                 },
                                 "itemCreators": {
                                     "items": {
+                                        "discriminator": "nameType",
+                                        "hint.cs": "Jako tv\u016frce je mo\u017en\u00e9 ozna\u010dit osobu nebo instituci.",
+                                        "hint.en": "It is possible to designate a person or an institution as the creator/contributor.",
                                         "marshmallow": {
                                             "class": "nr_metadata.common.services.records.schema_datatypes.NRRelatedItemCreatorSchema",
                                             "generate": true
                                         },
                                         "properties": {
                                             "affiliations": {
                                                 "items": {
@@ -2505,14 +3507,21 @@
                                                             "import": "invenio_vocabularies.records.api.Vocabulary"
                                                         }
                                                     ],
                                                     "keys": [
                                                         "id",
                                                         "title",
                                                         {
+                                                            "key": "props.ror",
+                                                            "model": {
+                                                                "type": "keyword"
+                                                            },
+                                                            "target": "ror"
+                                                        },
+                                                        {
                                                             "key": "hierarchy",
                                                             "model": {
                                                                 "marshmallow": {
                                                                     "class": "oarepo_vocabularies.services.schema.HierarchySchema",
                                                                     "generate": false,
                                                                     "imports": [
                                                                         {
@@ -2700,14 +3709,17 @@
                                                                 "marshmallow": {
                                                                     "field-class": "marshmallow.fields.String",
                                                                     "imports": [],
                                                                     "validators": []
                                                                 }
                                                             }
                                                         },
+                                                        "ror": {
+                                                            "type": "keyword"
+                                                        },
                                                         "title": {
                                                             "additionalProperties": {
                                                                 "type": "string"
                                                             },
                                                             "mapping": {
                                                                 "dynamic": true,
                                                                 "properties": {
@@ -2747,22 +3759,20 @@
                                                             "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRAffiliationVocabularyUISchema",
                                                             "generate": false,
                                                             "unknown": "INCLUDE"
                                                         }
                                                     },
                                                     "vocabulary-type": "institutions"
                                                 },
-                                                "label.cs": "Afiliace",
-                                                "label.en": "Affiliation",
                                                 "type": "array"
                                             },
                                             "authorityIdentifiers": {
                                                 "items": {
                                                     "marshmallow": {
-                                                        "class": "nr_metadata.schema.identifiers.NRAuthorityIdentifierSchema",
+                                                        "class": "nr_metadata.schema.identifiers.NROrganizationIdentifierSchema",
                                                         "generate": false
                                                     },
                                                     "properties": {
                                                         "identifier": {
                                                             "i18n.key": "identifier",
                                                             "label.cs": "Identifik\u00e1tor",
                                                             "label.en": "Identifier",
@@ -2770,20 +3780,14 @@
                                                             "sample": {
                                                                 "faker": "isbn13"
                                                             },
                                                             "type": "keyword"
                                                         },
                                                         "scheme": {
                                                             "enum": [
-                                                                "orcid",
-                                                                "scopusID",
-                                                                "researcherID",
-                                                                "czenasAutID",
-                                                                "vedidk",
-                                                                "institutionalID",
                                                                 "ISNI",
                                                                 "ROR",
                                                                 "ICO",
                                                                 "DOI"
                                                             ],
                                                             "hint.cs": "Doporu\u010dujeme zadat alespo\u0148 jeden z typ\u016f identifik\u00e1tor\u016f.\nPokud pot\u0159ebujete roz\u0161\u00ed\u0159it nab\u00eddku typ\u016f identifik\u00e1tor\u016f, kontaktujte n\u00e1s na support@narodni-repozitar.cz.\n",
                                                             "hint.en": "We recommend providing at least one of the identifier types.\nIf you need to expand the range of identifier types, contact us at support@narodni-repozitar.cz.\n",
@@ -2792,49 +3796,344 @@
                                                             "label.en": "Identifier type",
                                                             "required": true,
                                                             "type": "keyword"
                                                         }
                                                     },
                                                     "type": "object",
                                                     "ui": {
-                                                        "detail": "nr_authority_identifier",
+                                                        "detail": "nr_organization_identifier",
                                                         "marshmallow": {
-                                                            "class": "nr_metadata.ui_schema.identifiers.NRAuthorityIdentifierUISchema",
+                                                            "class": "nr_metadata.ui_schema.identifiers.NROrganizationIdentifierUISchema",
                                                             "generate": false
                                                         }
                                                     }
                                                 },
                                                 "type": "array"
                                             },
+                                            "familyName": {
+                                                "type": "keyword"
+                                            },
                                             "fullName": {
                                                 "label.cs": "Jm\u00e9no autora",
                                                 "label.en": "Author name",
                                                 "required": true,
                                                 "sample": {
                                                     "faker": "name"
                                                 },
                                                 "type": "keyword"
                                             },
+                                            "givenName": {
+                                                "type": "keyword"
+                                            },
                                             "nameType": {
                                                 "enum": [
-                                                    "Organizational",
-                                                    "Personal"
+                                                    "Organizational"
                                                 ],
-                                                "hint.cs": "Jako tv\u016frce je mo\u017en\u00e9 ozna\u010dit osobu nebo instituci.",
-                                                "hint.en": "It is possible to designate a person or an institution as the creator/contributor.",
                                                 "label.cs": "Typ",
                                                 "label.en": "Type",
                                                 "sample": [
-                                                    "Organizational",
-                                                    "Personal"
+                                                    "Organizational"
                                                 ],
                                                 "type": "keyword"
                                             }
                                         },
-                                        "type": "object",
+                                        "schemas": {
+                                            "Organizational": {
+                                                "marshmallow": {
+                                                    "class": "nr_metadata.common.services.records.schema_datatypes.NROrganizationSchema",
+                                                    "generate": false
+                                                },
+                                                "properties": {
+                                                    "authorityIdentifiers": {
+                                                        "items": {
+                                                            "marshmallow": {
+                                                                "class": "nr_metadata.schema.identifiers.NROrganizationIdentifierSchema",
+                                                                "generate": false
+                                                            },
+                                                            "properties": {
+                                                                "identifier": {
+                                                                    "i18n.key": "identifier",
+                                                                    "label.cs": "Identifik\u00e1tor",
+                                                                    "label.en": "Identifier",
+                                                                    "required": true,
+                                                                    "sample": {
+                                                                        "faker": "isbn13"
+                                                                    },
+                                                                    "type": "keyword"
+                                                                },
+                                                                "scheme": {
+                                                                    "enum": [
+                                                                        "ISNI",
+                                                                        "ROR",
+                                                                        "ICO",
+                                                                        "DOI"
+                                                                    ],
+                                                                    "hint.cs": "Doporu\u010dujeme zadat alespo\u0148 jeden z typ\u016f identifik\u00e1tor\u016f.\nPokud pot\u0159ebujete roz\u0161\u00ed\u0159it nab\u00eddku typ\u016f identifik\u00e1tor\u016f, kontaktujte n\u00e1s na support@narodni-repozitar.cz.\n",
+                                                                    "hint.en": "We recommend providing at least one of the identifier types.\nIf you need to expand the range of identifier types, contact us at support@narodni-repozitar.cz.\n",
+                                                                    "i18n.key": "identifier_type",
+                                                                    "label.cs": "Typ identifik\u00e1toru",
+                                                                    "label.en": "Identifier type",
+                                                                    "required": true,
+                                                                    "type": "keyword"
+                                                                }
+                                                            },
+                                                            "type": "object",
+                                                            "ui": {
+                                                                "detail": "nr_organization_identifier",
+                                                                "marshmallow": {
+                                                                    "class": "nr_metadata.ui_schema.identifiers.NROrganizationIdentifierUISchema",
+                                                                    "generate": false
+                                                                }
+                                                            }
+                                                        },
+                                                        "type": "array"
+                                                    },
+                                                    "fullName": {
+                                                        "label.cs": "Jm\u00e9no autora",
+                                                        "label.en": "Author name",
+                                                        "required": true,
+                                                        "sample": {
+                                                            "faker": "name"
+                                                        },
+                                                        "type": "keyword"
+                                                    },
+                                                    "nameType": {
+                                                        "enum": [
+                                                            "Organizational"
+                                                        ],
+                                                        "label.cs": "Typ",
+                                                        "label.en": "Type",
+                                                        "sample": [
+                                                            "Organizational"
+                                                        ],
+                                                        "type": "keyword"
+                                                    }
+                                                },
+                                                "type": "object",
+                                                "ui": {
+                                                    "detail": "nr_organization",
+                                                    "marshmallow": {
+                                                        "class": "nr_metadata.common.services.records.ui_schema_datatypes.NROrganizationUISchema",
+                                                        "generate": false
+                                                    }
+                                                }
+                                            },
+                                            "Personal": {
+                                                "marshmallow": {
+                                                    "class": "nr_metadata.common.services.records.schema_datatypes.NRPersonSchema",
+                                                    "generate": false
+                                                },
+                                                "properties": {
+                                                    "affiliations": {
+                                                        "items": {
+                                                            "facets": {
+                                                                "args": [
+                                                                    "vocabulary='institutions'"
+                                                                ]
+                                                            },
+                                                            "hint.cs": "Uve\u010fte instituci/instituce, pod jej\u00ed\u017e z\u00e1\u0161titou jste se na tvorb\u011b objektu pod\u00edleli.",
+                                                            "imports": [
+                                                                {
+                                                                    "import": "invenio_vocabularies.records.api.Vocabulary"
+                                                                }
+                                                            ],
+                                                            "keys": [
+                                                                "id",
+                                                                "title",
+                                                                {
+                                                                    "key": "props.ror",
+                                                                    "model": {
+                                                                        "type": "keyword"
+                                                                    },
+                                                                    "target": "ror"
+                                                                },
+                                                                {
+                                                                    "key": "hierarchy",
+                                                                    "model": {
+                                                                        "marshmallow": {
+                                                                            "class": "oarepo_vocabularies.services.schema.HierarchySchema",
+                                                                            "generate": false,
+                                                                            "imports": [
+                                                                                {
+                                                                                    "import": "oarepo_vocabularies.services.schema.HierarchySchema"
+                                                                                }
+                                                                            ]
+                                                                        },
+                                                                        "properties": {
+                                                                            "ancestors": {
+                                                                                "items": {
+                                                                                    "type": "keyword"
+                                                                                },
+                                                                                "type": "array"
+                                                                            },
+                                                                            "ancestors_or_self": {
+                                                                                "items": {
+                                                                                    "type": "keyword"
+                                                                                },
+                                                                                "type": "array"
+                                                                            },
+                                                                            "level": {
+                                                                                "type": "integer"
+                                                                            },
+                                                                            "parent": {
+                                                                                "type": "keyword"
+                                                                            },
+                                                                            "title": {
+                                                                                "items": {
+                                                                                    "additionalProperties": {
+                                                                                        "type": "string"
+                                                                                    },
+                                                                                    "mapping": {
+                                                                                        "dynamic": true
+                                                                                    },
+                                                                                    "marshmallow": {
+                                                                                        "class": "nr_metadata.common.services.records.schema.TitleItemSchema",
+                                                                                        "field": "i18n_strings",
+                                                                                        "generate": false
+                                                                                    },
+                                                                                    "propertyNames": {
+                                                                                        "pattern": "^[a-z]{2}$"
+                                                                                    },
+                                                                                    "type": "object",
+                                                                                    "ui": {
+                                                                                        "marshmallow": {
+                                                                                            "class": "nr_metadata.common.services.records.ui_schema.TitleItemUISchema",
+                                                                                            "field": "i18n_strings",
+                                                                                            "generate": false
+                                                                                        }
+                                                                                    }
+                                                                                },
+                                                                                "type": "array"
+                                                                            }
+                                                                        },
+                                                                        "type": "object",
+                                                                        "ui": {
+                                                                            "marshmallow": {
+                                                                                "class": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema",
+                                                                                "generate": false,
+                                                                                "imports": [
+                                                                                    {
+                                                                                        "import": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema"
+                                                                                    }
+                                                                                ]
+                                                                            }
+                                                                        }
+                                                                    },
+                                                                    "target": "hierarchy"
+                                                                }
+                                                            ],
+                                                            "label.cs": "Afiliace",
+                                                            "label.en": "Affiliation",
+                                                            "marshmallow": {
+                                                                "class": "nr_metadata.common.services.records.schema_datatypes.NRAffiliationVocabularySchema",
+                                                                "generate": false,
+                                                                "unknown": "INCLUDE"
+                                                            },
+                                                            "model": "vocabularies",
+                                                            "pid-field": "Vocabulary.pid.with_type_ctx(\"institutions\")",
+                                                            "properties": {},
+                                                            "sample": {
+                                                                "faker": "company"
+                                                            },
+                                                            "type": "taxonomy",
+                                                            "ui": {
+                                                                "detail": "taxonomy_item",
+                                                                "edit": "taxonomy_item",
+                                                                "marshmallow": {
+                                                                    "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRAffiliationVocabularyUISchema",
+                                                                    "generate": false,
+                                                                    "unknown": "INCLUDE"
+                                                                }
+                                                            },
+                                                            "vocabulary-type": "institutions"
+                                                        },
+                                                        "type": "array"
+                                                    },
+                                                    "authorityIdentifiers": {
+                                                        "items": {
+                                                            "marshmallow": {
+                                                                "class": "nr_metadata.schema.identifiers.NRPersonIdentifierSchema",
+                                                                "generate": false
+                                                            },
+                                                            "properties": {
+                                                                "identifier": {
+                                                                    "i18n.key": "identifier",
+                                                                    "label.cs": "Identifik\u00e1tor",
+                                                                    "label.en": "Identifier",
+                                                                    "required": true,
+                                                                    "sample": {
+                                                                        "faker": "isbn13"
+                                                                    },
+                                                                    "type": "keyword"
+                                                                },
+                                                                "scheme": {
+                                                                    "enum": [
+                                                                        "orcid",
+                                                                        "scopusID",
+                                                                        "researcherID",
+                                                                        "czenasAutID",
+                                                                        "vedidk",
+                                                                        "institutionalID",
+                                                                        "ISNI"
+                                                                    ],
+                                                                    "hint.cs": "Doporu\u010dujeme zadat alespo\u0148 jeden z typ\u016f identifik\u00e1tor\u016f.\nPokud pot\u0159ebujete roz\u0161\u00ed\u0159it nab\u00eddku typ\u016f identifik\u00e1tor\u016f, kontaktujte n\u00e1s na support@narodni-repozitar.cz.\n",
+                                                                    "hint.en": "We recommend providing at least one of the identifier types.\nIf you need to expand the range of identifier types, contact us at support@narodni-repozitar.cz.\n",
+                                                                    "i18n.key": "identifier_type",
+                                                                    "label.cs": "Typ identifik\u00e1toru",
+                                                                    "label.en": "Identifier type",
+                                                                    "required": true,
+                                                                    "type": "keyword"
+                                                                }
+                                                            },
+                                                            "type": "object",
+                                                            "ui": {
+                                                                "detail": "nr_person_identifier",
+                                                                "marshmallow": {
+                                                                    "class": "nr_metadata.ui_schema.identifiers.NRPersonIdentifierUISchema",
+                                                                    "generate": false
+                                                                }
+                                                            }
+                                                        },
+                                                        "type": "array"
+                                                    },
+                                                    "familyName": {
+                                                        "type": "keyword"
+                                                    },
+                                                    "fullName": {
+                                                        "label.cs": "Jm\u00e9no autora",
+                                                        "label.en": "Author name",
+                                                        "required": true,
+                                                        "sample": {
+                                                            "faker": "name"
+                                                        },
+                                                        "type": "keyword"
+                                                    },
+                                                    "givenName": {
+                                                        "type": "keyword"
+                                                    },
+                                                    "nameType": {
+                                                        "enum": [
+                                                            "Personal"
+                                                        ],
+                                                        "label.cs": "Typ",
+                                                        "label.en": "Type",
+                                                        "type": "keyword"
+                                                    }
+                                                },
+                                                "type": "object",
+                                                "ui": {
+                                                    "detail": "nr_person",
+                                                    "marshmallow": {
+                                                        "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRPersonUISchema",
+                                                        "generate": false
+                                                    }
+                                                }
+                                            }
+                                        },
+                                        "type": "polymorphic",
                                         "ui": {
                                             "detail": "creator",
                                             "marshmallow": {
                                                 "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRRelatedItemCreatorUISchema",
                                                 "generate": true
                                             }
                                         }
@@ -2873,15 +4172,16 @@
                                             },
                                             "scheme": {
                                                 "enum": [
                                                     "DOI",
                                                     "Handle",
                                                     "ISBN",
                                                     "ISSN",
-                                                    "RIV"
+                                                    "RIV",
+                                                    "IGSN"
                                                 ],
                                                 "label.cs": "Typ identifik\u00e1toru",
                                                 "label.en": "Identifier type",
                                                 "required": true,
                                                 "type": "keyword"
                                             }
                                         },
@@ -3286,35 +4586,35 @@
                             }
                         },
                         "vocabulary-type": "resource-types"
                     },
                     "rights": {
                         "facets": {
                             "args": [
-                                "vocabulary='licenses'"
+                                "vocabulary='rights'"
                             ]
                         },
                         "imports": [
                             {
                                 "import": "invenio_vocabularies.records.api.Vocabulary"
                             }
                         ],
                         "keys": [
                             "id",
                             "title"
                         ],
-                        "label.cs": "Licence",
-                        "label.en": "License",
+                        "label.cs": "Pr\u00e1va/Licence",
+                        "label.en": "Rights/Licenses",
                         "marshmallow": {
-                            "class": "nr_metadata.common.services.records.schema_datatypes.NRLicenseVocabularySchema",
+                            "class": "nr_metadata.common.services.records.schema_datatypes.NRRightsVocabularySchema",
                             "generate": true,
                             "unknown": "INCLUDE"
                         },
                         "model": "vocabularies",
-                        "pid-field": "Vocabulary.pid.with_type_ctx(\"licenses\")",
+                        "pid-field": "Vocabulary.pid.with_type_ctx(\"rights\")",
                         "properties": {
                             "@v": {
                                 "facets": {
                                     "facet": false
                                 },
                                 "marshmallow": {
                                     "field-class": "marshmallow.fields.String",
@@ -3394,24 +4694,24 @@
                             "CC BY-NC-ND"
                         ],
                         "type": "vocabulary",
                         "ui": {
                             "detail": "vocabulary_item",
                             "edit": "vocabulary_item",
                             "marshmallow": {
-                                "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRLicenseVocabularyUISchema",
+                                "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRRightsVocabularyUISchema",
                                 "generate": true,
                                 "unknown": "INCLUDE"
                             }
                         },
-                        "vocabulary-type": "licenses"
+                        "vocabulary-type": "rights"
                     },
                     "series": {
                         "items": {
-                            "label.cs": "S\u00e9rie",
+                            "label.cs": "Edice",
                             "label.en": "Series",
                             "marshmallow": {
                                 "class": "nr_metadata.common.services.records.schema_datatypes.NRSeriesSchema",
                                 "generate": true
                             },
                             "properties": {
                                 "seriesTitle": {
@@ -3442,15 +4742,15 @@
                                 "detail": "series",
                                 "marshmallow": {
                                     "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRSeriesUISchema",
                                     "generate": true
                                 }
                             }
                         },
-                        "label.cs": "S\u00e9rie",
+                        "label.cs": "Edice",
                         "label.en": "Series",
                         "type": "array"
                     },
                     "subjectCategories": {
                         "items": {
                             "facets": {
                                 "args": [
@@ -3803,14 +5103,15 @@
         },
         "record": {
             "base-classes": [
                 "invenio_records_resources.records.api.Record{InvenioRecord}"
             ],
             "class": "nr_metadata.common.records.api.CommonRecord",
             "extra-code": "",
+            "fields": {},
             "generate": true,
             "imports": [],
             "module": "nr_metadata.common.records.api"
         },
         "record-dumper": {
             "base-classes": [
                 "oarepo_runtime.records.dumpers.SearchDumper"
@@ -3821,14 +5122,36 @@
                 "{{nr_metadata.common.records.dumpers.edtf.CommonEDTFIntervalDumperExt}}()"
             ],
             "extra-code": "",
             "generate": true,
             "imports": [],
             "module": "nr_metadata.common.records.dumpers.dumper"
         },
+        "record-item": {
+            "base-classes": [
+                "oarepo_runtime.services.results.RecordItem"
+            ],
+            "class": "nr_metadata.common.services.records.results.CommonRecordItem",
+            "components": [],
+            "extra-code": "",
+            "generate": true,
+            "imports": [],
+            "module": "nr_metadata.common.services.records.results"
+        },
+        "record-list": {
+            "base-classes": [
+                "oarepo_runtime.services.results.RecordList"
+            ],
+            "class": "nr_metadata.common.services.records.results.CommonRecordList",
+            "components": [],
+            "extra-code": "",
+            "generate": true,
+            "imports": [],
+            "module": "nr_metadata.common.services.records.results"
+        },
         "record-metadata": {
             "alembic": "nr_metadata.common.alembic",
             "alias": "common",
             "base-classes": [
                 "invenio_db.db{db.Model}",
                 "invenio_records.models.RecordMetadataBase"
             ],
@@ -3837,26 +5160,28 @@
             "generate": true,
             "imports": [],
             "module": "nr_metadata.common.records.models",
             "table": "common_metadata",
             "use-versioning": true
         },
         "resource": {
+            "additional-args": [],
             "base-classes": [
                 "invenio_records_resources.resources.RecordResource"
             ],
             "class": "nr_metadata.common.resources.records.resource.CommonResource",
             "config-key": "COMMON_RECORD_RESOURCE_CLASS",
             "extra-code": "",
             "generate": true,
             "imports": [],
             "module": "nr_metadata.common.resources.records.resource",
             "proxy": "current_resource"
         },
         "resource-config": {
+            "additional-args": [],
             "base-classes": [
                 "invenio_records_resources.resources.RecordResourceConfig"
             ],
             "base-html-url": "/nr-metadata-common/",
             "base-url": "/nr-metadata-common/",
             "class": "nr_metadata.common.resources.records.config.CommonResourceConfig",
             "config-key": "COMMON_RECORD_RESOURCE_CONFIG",
@@ -3875,46 +5200,48 @@
         },
         "search-options": {
             "base-classes": [
                 "invenio_records_resources.services.SearchOptions{InvenioSearchOptions}"
             ],
             "class": "nr_metadata.common.services.records.search.CommonSearchOptions",
             "extra-code": "",
+            "fields": {},
             "generate": true,
             "imports": [],
             "module": "nr_metadata.common.services.records.search",
             "sort-options-field": "sort_options"
         },
         "searchable": true,
         "service": {
+            "additional-args": [],
             "base-classes": [
                 "invenio_records_resources.services.RecordService{InvenioRecordService}"
             ],
             "class": "nr_metadata.common.services.records.service.CommonService",
             "config-key": "COMMON_RECORD_SERVICE_CLASS",
             "extra-code": "",
             "generate": true,
             "imports": [],
             "module": "nr_metadata.common.services.records.service",
             "proxy": "current_service"
         },
         "service-config": {
+            "additional-args": [],
             "base-classes": [
                 "oarepo_runtime.services.config.service.PermissionsPresetsConfigMixin",
                 "invenio_records_resources.services.RecordServiceConfig{InvenioRecordServiceConfig}"
             ],
             "class": "nr_metadata.common.services.records.config.CommonServiceConfig",
             "components": [
                 "{{invenio_records_resources.services.records.components.DataComponent}}"
             ],
             "config-key": "COMMON_RECORD_SERVICE_CONFIG",
             "extra-code": "",
             "generate": true,
             "module": "nr_metadata.common.services.records.config",
-            "result-list-class": "oarepo_runtime.services.results.RecordList",
             "service-id": "common"
         },
         "sortable": [],
         "tests": {
             "extra-code": "",
             "extra-fixtures": [],
             "module": "tests"
```

### Comparing `nr-metadata-2.0.8/nr_metadata/common/records/api.py` & `nr-metadata-2.0.9/nr_metadata/common/records/api.py`

 * *Files 17% similar despite different names*

```diff
@@ -30,25 +30,30 @@
         accessRights=PIDRelation(
             "metadata.accessRights",
             keys=["id", "title"],
             pid_field=Vocabulary.pid.with_type_ctx("access-rights"),
         ),
         affiliations=PIDRelation(
             "metadata.contributors.affiliations",
-            keys=["id", "title", "hierarchy"],
+            keys=["id", "title", {"key": "props.ror", "target": "ror"}, "hierarchy"],
             pid_field=Vocabulary.pid.with_type_ctx("institutions"),
         ),
-        role=PIDRelation(
-            "metadata.contributors.role",
+        contributorType=PIDRelation(
+            "metadata.contributors.contributorType",
             keys=["id", "title"],
-            pid_field=Vocabulary.pid.with_type_ctx("contributor-roles"),
+            pid_field=Vocabulary.pid.with_type_ctx("contributor-types"),
         ),
-        creators_affiliations=PIDRelation(
+        Organizational_contributorType=PIDRelation(
+            "metadata.contributors.contributorType",
+            keys=["id", "title"],
+            pid_field=Vocabulary.pid.with_type_ctx("contributor-types"),
+        ),
+        Personal_affiliations=PIDRelation(
             "metadata.creators.affiliations",
-            keys=["id", "title", "hierarchy"],
+            keys=["id", "title", {"key": "props.ror", "target": "ror"}, "hierarchy"],
             pid_field=Vocabulary.pid.with_type_ctx("institutions"),
         ),
         country=PIDRelation(
             "metadata.events.eventLocation.country",
             keys=["id", "title"],
             pid_field=Vocabulary.pid.with_type_ctx("countries"),
         ),
@@ -58,27 +63,32 @@
             pid_field=Vocabulary.pid.with_type_ctx("funders"),
         ),
         languages=PIDRelation(
             "metadata.languages",
             keys=["id", "title"],
             pid_field=Vocabulary.pid.with_type_ctx("languages"),
         ),
-        itemContributors_affiliations=PIDRelation(
+        itemContributors_Personal_affiliations=PIDRelation(
             "metadata.relatedItems.itemContributors.affiliations",
-            keys=["id", "title", "hierarchy"],
+            keys=["id", "title", {"key": "props.ror", "target": "ror"}, "hierarchy"],
             pid_field=Vocabulary.pid.with_type_ctx("institutions"),
         ),
-        itemContributors_role=PIDRelation(
-            "metadata.relatedItems.itemContributors.role",
+        Personal_contributorType=PIDRelation(
+            "metadata.relatedItems.itemContributors.contributorType",
+            keys=["id", "title"],
+            pid_field=Vocabulary.pid.with_type_ctx("contributor-types"),
+        ),
+        itemContributors_Organizational_contributorType=PIDRelation(
+            "metadata.relatedItems.itemContributors.contributorType",
             keys=["id", "title"],
-            pid_field=Vocabulary.pid.with_type_ctx("contributor-roles"),
+            pid_field=Vocabulary.pid.with_type_ctx("contributor-types"),
         ),
-        itemCreators_affiliations=PIDRelation(
+        itemCreators_Personal_affiliations=PIDRelation(
             "metadata.relatedItems.itemCreators.affiliations",
-            keys=["id", "title", "hierarchy"],
+            keys=["id", "title", {"key": "props.ror", "target": "ror"}, "hierarchy"],
             pid_field=Vocabulary.pid.with_type_ctx("institutions"),
         ),
         itemRelationType=PIDRelation(
             "metadata.relatedItems.itemRelationType",
             keys=["id", "title"],
             pid_field=Vocabulary.pid.with_type_ctx("item-relation-types"),
         ),
@@ -91,15 +101,15 @@
             "metadata.resourceType",
             keys=["id", "title"],
             pid_field=Vocabulary.pid.with_type_ctx("resource-types"),
         ),
         rights=PIDRelation(
             "metadata.rights",
             keys=["id", "title"],
-            pid_field=Vocabulary.pid.with_type_ctx("licenses"),
+            pid_field=Vocabulary.pid.with_type_ctx("rights"),
         ),
         subjectCategories=PIDRelation(
             "metadata.subjectCategories",
             keys=["id", "title"],
             pid_field=Vocabulary.pid.with_type_ctx("subject-categories"),
         ),
     )
```

### Comparing `nr-metadata-2.0.8/nr_metadata/common/records/dumpers/multilingual.py` & `nr-metadata-2.0.9/nr_metadata/common/records/dumpers/multilingual.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-2.0.8/nr_metadata/common/records/jsonschemas/common-1.0.0.json` & `nr-metadata-2.0.9/nr_metadata/common/records/jsonschemas/common-1.0.0.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993208703944159%*

 * *Differences: {"'properties'": "{'metadata': {'properties': {'contributors': {'items': {'properties': "*

 * *                 "{'affiliations': {'items': {'properties': {'ror': OrderedDict([('type', "*

 * *                 "'string')])}}}, 'contributorType': OrderedDict([('type', 'object'), "*

 * *                 "('properties', OrderedDict([('id', OrderedDict([('type', 'string')])), ('title', "*

 * *                 "OrderedDict([('type', 'object')])), ('@v', OrderedDict([('type', "*

 * *                 "'string')]))]))]), 'familyName': Order […]*

```diff
@@ -113,14 +113,17 @@
                                                 }
                                             },
                                             "type": "object"
                                         },
                                         "id": {
                                             "type": "string"
                                         },
+                                        "ror": {
+                                            "type": "string"
+                                        },
                                         "title": {
                                             "type": "object"
                                         }
                                     },
                                     "type": "object"
                                 },
                                 "type": "array"
@@ -135,33 +138,39 @@
                                             "type": "string"
                                         }
                                     },
                                     "type": "object"
                                 },
                                 "type": "array"
                             },
-                            "fullName": {
-                                "type": "string"
-                            },
-                            "nameType": {
-                                "type": "string"
-                            },
-                            "role": {
+                            "contributorType": {
                                 "properties": {
                                     "@v": {
                                         "type": "string"
                                     },
                                     "id": {
                                         "type": "string"
                                     },
                                     "title": {
                                         "type": "object"
                                     }
                                 },
                                 "type": "object"
+                            },
+                            "familyName": {
+                                "type": "string"
+                            },
+                            "fullName": {
+                                "type": "string"
+                            },
+                            "givenName": {
+                                "type": "string"
+                            },
+                            "nameType": {
+                                "type": "string"
                             }
                         },
                         "type": "object"
                     },
                     "type": "array"
                 },
                 "creators": {
@@ -201,14 +210,17 @@
                                                 }
                                             },
                                             "type": "object"
                                         },
                                         "id": {
                                             "type": "string"
                                         },
+                                        "ror": {
+                                            "type": "string"
+                                        },
                                         "title": {
                                             "type": "object"
                                         }
                                     },
                                     "type": "object"
                                 },
                                 "type": "array"
@@ -223,37 +235,39 @@
                                             "type": "string"
                                         }
                                     },
                                     "type": "object"
                                 },
                                 "type": "array"
                             },
+                            "familyName": {
+                                "type": "string"
+                            },
                             "fullName": {
                                 "type": "string"
                             },
+                            "givenName": {
+                                "type": "string"
+                            },
                             "nameType": {
                                 "type": "string"
                             }
                         },
                         "type": "object"
                     },
                     "type": "array"
                 },
                 "dateAvailable": {
-                    "format": "date-time",
+                    "format": "date",
                     "type": "string"
                 },
                 "dateIssued": {
                     "format": "date-time",
                     "type": "string"
                 },
-                "dateModified": {
-                    "format": "date-time",
-                    "type": "string"
-                },
                 "events": {
                     "items": {
                         "properties": {
                             "eventDate": {
                                 "format": "date-time",
                                 "type": "string"
                             },
@@ -289,25 +303,14 @@
                                 "type": "string"
                             }
                         },
                         "type": "object"
                     },
                     "type": "array"
                 },
-                "externalLocation": {
-                    "properties": {
-                        "externalLocationNote": {
-                            "type": "string"
-                        },
-                        "externalLocationURL": {
-                            "type": "string"
-                        }
-                    },
-                    "type": "object"
-                },
                 "fundingReferences": {
                     "items": {
                         "properties": {
                             "funder": {
                                 "properties": {
                                     "@v": {
                                         "type": "string"
@@ -407,20 +410,14 @@
                         "type": "object"
                     },
                     "type": "array"
                 },
                 "originalRecord": {
                     "type": "string"
                 },
-                "publishers": {
-                    "items": {
-                        "type": "string"
-                    },
-                    "type": "array"
-                },
                 "relatedItems": {
                     "items": {
                         "properties": {
                             "itemContributors": {
                                 "items": {
                                     "properties": {
                                         "affiliations": {
@@ -457,14 +454,17 @@
                                                             }
                                                         },
                                                         "type": "object"
                                                     },
                                                     "id": {
                                                         "type": "string"
                                                     },
+                                                    "ror": {
+                                                        "type": "string"
+                                                    },
                                                     "title": {
                                                         "type": "object"
                                                     }
                                                 },
                                                 "type": "object"
                                             },
                                             "type": "array"
@@ -479,33 +479,39 @@
                                                         "type": "string"
                                                     }
                                                 },
                                                 "type": "object"
                                             },
                                             "type": "array"
                                         },
-                                        "fullName": {
-                                            "type": "string"
-                                        },
-                                        "nameType": {
-                                            "type": "string"
-                                        },
-                                        "role": {
+                                        "contributorType": {
                                             "properties": {
                                                 "@v": {
                                                     "type": "string"
                                                 },
                                                 "id": {
                                                     "type": "string"
                                                 },
                                                 "title": {
                                                     "type": "object"
                                                 }
                                             },
                                             "type": "object"
+                                        },
+                                        "familyName": {
+                                            "type": "string"
+                                        },
+                                        "fullName": {
+                                            "type": "string"
+                                        },
+                                        "givenName": {
+                                            "type": "string"
+                                        },
+                                        "nameType": {
+                                            "type": "string"
                                         }
                                     },
                                     "type": "object"
                                 },
                                 "type": "array"
                             },
                             "itemCreators": {
@@ -545,14 +551,17 @@
                                                             }
                                                         },
                                                         "type": "object"
                                                     },
                                                     "id": {
                                                         "type": "string"
                                                     },
+                                                    "ror": {
+                                                        "type": "string"
+                                                    },
                                                     "title": {
                                                         "type": "object"
                                                     }
                                                 },
                                                 "type": "object"
                                             },
                                             "type": "array"
@@ -567,17 +576,23 @@
                                                         "type": "string"
                                                     }
                                                 },
                                                 "type": "object"
                                             },
                                             "type": "array"
                                         },
+                                        "familyName": {
+                                            "type": "string"
+                                        },
                                         "fullName": {
                                             "type": "string"
                                         },
+                                        "givenName": {
+                                            "type": "string"
+                                        },
                                         "nameType": {
                                             "type": "string"
                                         }
                                     },
                                     "type": "object"
                                 },
                                 "type": "array"
```

### Comparing `nr-metadata-2.0.8/nr_metadata/common/records/mappings/os-v2/common/common-1.0.0.json` & `nr-metadata-2.0.9/nr_metadata/common/records/mappings/os-v2/common/common-1.0.0.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994542080250699%*

 * *Differences: {"'mappings'": "{'properties': {'metadata': {'properties': {'contributors': {'properties': "*

 * *               "{'affiliations': {'properties': {'ror': OrderedDict([('type', 'keyword'), "*

 * *               "('ignore_above', 1024)])}}, 'contributorType': OrderedDict([('type', 'object'), "*

 * *               "('properties', OrderedDict([('id', OrderedDict([('fields', OrderedDict([('text', "*

 * *               "OrderedDict([('type', 'search_as_you_type')]))])), ('type', 'keyword'), "*

 * *               "('ignore_above', 1024)]) […]*

```diff
@@ -200,14 +200,18 @@
                                             "text": {
                                                 "type": "search_as_you_type"
                                             }
                                         },
                                         "ignore_above": 1024,
                                         "type": "keyword"
                                     },
+                                    "ror": {
+                                        "ignore_above": 1024,
+                                        "type": "keyword"
+                                    },
                                     "title": {
                                         "dynamic": true,
                                         "properties": {
                                             "en": {
                                                 "copy_to": "title_sort",
                                                 "type": "search_as_you_type"
                                             }
@@ -226,23 +230,15 @@
                                     "scheme": {
                                         "ignore_above": 1024,
                                         "type": "keyword"
                                     }
                                 },
                                 "type": "object"
                             },
-                            "fullName": {
-                                "ignore_above": 1024,
-                                "type": "keyword"
-                            },
-                            "nameType": {
-                                "ignore_above": 1024,
-                                "type": "keyword"
-                            },
-                            "role": {
+                            "contributorType": {
                                 "properties": {
                                     "@v": {
                                         "ignore_above": 1024,
                                         "type": "keyword"
                                     },
                                     "id": {
                                         "fields": {
@@ -261,14 +257,30 @@
                                                 "type": "search_as_you_type"
                                             }
                                         },
                                         "type": "object"
                                     }
                                 },
                                 "type": "object"
+                            },
+                            "familyName": {
+                                "ignore_above": 1024,
+                                "type": "keyword"
+                            },
+                            "fullName": {
+                                "ignore_above": 1024,
+                                "type": "keyword"
+                            },
+                            "givenName": {
+                                "ignore_above": 1024,
+                                "type": "keyword"
+                            },
+                            "nameType": {
+                                "ignore_above": 1024,
+                                "type": "keyword"
                             }
                         },
                         "type": "object"
                     },
                     "creators": {
                         "properties": {
                             "affiliations": {
@@ -306,14 +318,18 @@
                                             "text": {
                                                 "type": "search_as_you_type"
                                             }
                                         },
                                         "ignore_above": 1024,
                                         "type": "keyword"
                                     },
+                                    "ror": {
+                                        "ignore_above": 1024,
+                                        "type": "keyword"
+                                    },
                                     "title": {
                                         "dynamic": true,
                                         "properties": {
                                             "en": {
                                                 "copy_to": "title_sort",
                                                 "type": "search_as_you_type"
                                             }
@@ -332,37 +348,41 @@
                                     "scheme": {
                                         "ignore_above": 1024,
                                         "type": "keyword"
                                     }
                                 },
                                 "type": "object"
                             },
+                            "familyName": {
+                                "ignore_above": 1024,
+                                "type": "keyword"
+                            },
                             "fullName": {
                                 "ignore_above": 1024,
                                 "type": "keyword"
                             },
+                            "givenName": {
+                                "ignore_above": 1024,
+                                "type": "keyword"
+                            },
                             "nameType": {
                                 "ignore_above": 1024,
                                 "type": "keyword"
                             }
                         },
                         "type": "object"
                     },
                     "dateAvailable": {
-                        "format": "strict_date_time||strict_date_time_no_millis||strict_date||yyyy-MM||yyyy",
+                        "format": "basic_date||strict_date",
                         "type": "date"
                     },
                     "dateIssued": {
                         "format": "strict_date_time||strict_date_time_no_millis||strict_date||yyyy-MM||yyyy",
                         "type": "date"
                     },
-                    "dateModified": {
-                        "format": "strict_date_time||strict_date_time_no_millis||strict_date||yyyy-MM||yyyy",
-                        "type": "date"
-                    },
                     "events": {
                         "properties": {
                             "eventDate": {
                                 "format": "strict_date_time||strict_date_time_no_millis||strict_date||yyyy-MM||yyyy",
                                 "index": false,
                                 "type": "date_range"
                             },
@@ -408,26 +428,14 @@
                             },
                             "eventNameOriginal": {
                                 "type": "text"
                             }
                         },
                         "type": "object"
                     },
-                    "externalLocation": {
-                        "properties": {
-                            "externalLocationNote": {
-                                "type": "text"
-                            },
-                            "externalLocationURL": {
-                                "ignore_above": 1024,
-                                "type": "keyword"
-                            }
-                        },
-                        "type": "object"
-                    },
                     "fundingReferences": {
                         "properties": {
                             "funder": {
                                 "properties": {
                                     "@v": {
                                         "ignore_above": 1024,
                                         "type": "keyword"
@@ -568,17 +576,14 @@
                         },
                         "type": "object"
                     },
                     "originalRecord": {
                         "ignore_above": 1024,
                         "type": "keyword"
                     },
-                    "publishers": {
-                        "type": "text"
-                    },
                     "relatedItems": {
                         "properties": {
                             "itemContributors": {
                                 "properties": {
                                     "affiliations": {
                                         "properties": {
                                             "@v": {
@@ -614,14 +619,18 @@
                                                     "text": {
                                                         "type": "search_as_you_type"
                                                     }
                                                 },
                                                 "ignore_above": 1024,
                                                 "type": "keyword"
                                             },
+                                            "ror": {
+                                                "ignore_above": 1024,
+                                                "type": "keyword"
+                                            },
                                             "title": {
                                                 "dynamic": true,
                                                 "properties": {
                                                     "en": {
                                                         "copy_to": "title_sort",
                                                         "type": "search_as_you_type"
                                                     }
@@ -640,23 +649,15 @@
                                             "scheme": {
                                                 "ignore_above": 1024,
                                                 "type": "keyword"
                                             }
                                         },
                                         "type": "object"
                                     },
-                                    "fullName": {
-                                        "ignore_above": 1024,
-                                        "type": "keyword"
-                                    },
-                                    "nameType": {
-                                        "ignore_above": 1024,
-                                        "type": "keyword"
-                                    },
-                                    "role": {
+                                    "contributorType": {
                                         "properties": {
                                             "@v": {
                                                 "ignore_above": 1024,
                                                 "type": "keyword"
                                             },
                                             "id": {
                                                 "fields": {
@@ -675,14 +676,30 @@
                                                         "type": "search_as_you_type"
                                                     }
                                                 },
                                                 "type": "object"
                                             }
                                         },
                                         "type": "object"
+                                    },
+                                    "familyName": {
+                                        "ignore_above": 1024,
+                                        "type": "keyword"
+                                    },
+                                    "fullName": {
+                                        "ignore_above": 1024,
+                                        "type": "keyword"
+                                    },
+                                    "givenName": {
+                                        "ignore_above": 1024,
+                                        "type": "keyword"
+                                    },
+                                    "nameType": {
+                                        "ignore_above": 1024,
+                                        "type": "keyword"
                                     }
                                 },
                                 "type": "object"
                             },
                             "itemCreators": {
                                 "properties": {
                                     "affiliations": {
@@ -720,14 +737,18 @@
                                                     "text": {
                                                         "type": "search_as_you_type"
                                                     }
                                                 },
                                                 "ignore_above": 1024,
                                                 "type": "keyword"
                                             },
+                                            "ror": {
+                                                "ignore_above": 1024,
+                                                "type": "keyword"
+                                            },
                                             "title": {
                                                 "dynamic": true,
                                                 "properties": {
                                                     "en": {
                                                         "copy_to": "title_sort",
                                                         "type": "search_as_you_type"
                                                     }
@@ -746,18 +767,26 @@
                                             "scheme": {
                                                 "ignore_above": 1024,
                                                 "type": "keyword"
                                             }
                                         },
                                         "type": "object"
                                     },
+                                    "familyName": {
+                                        "ignore_above": 1024,
+                                        "type": "keyword"
+                                    },
                                     "fullName": {
                                         "ignore_above": 1024,
                                         "type": "keyword"
                                     },
+                                    "givenName": {
+                                        "ignore_above": 1024,
+                                        "type": "keyword"
+                                    },
                                     "nameType": {
                                         "ignore_above": 1024,
                                         "type": "keyword"
                                     }
                                 },
                                 "type": "object"
                             },
```

### Comparing `nr-metadata-2.0.8/nr_metadata/common/resources/records/config.py` & `nr-metadata-2.0.9/nr_metadata/common/resources/records/config.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-2.0.8/nr_metadata/common/resources/records/ui.py` & `nr-metadata-2.0.9/nr_metadata/common/resources/records/ui.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from flask import g
 from flask_resources import BaseListSchema
 from flask_resources.serializers import JSONSerializer
 from oarepo_runtime.resources import LocalizedUIJSONSerializer
 
 from nr_metadata.common.services.records.ui_schema_common import NRCommonRecordUISchema
 
 
@@ -10,9 +11,9 @@
 
     def __init__(self):
         """Initialise Serializer."""
         super().__init__(
             format_serializer_cls=JSONSerializer,
             object_schema_cls=NRCommonRecordUISchema,
             list_schema_cls=BaseListSchema,
-            schema_context={"object_key": "ui"},
+            schema_context={"object_key": "ui", "identity": g.identity},
         )
```

### Comparing `nr-metadata-2.0.8/nr_metadata/common/services/records/config.py` & `nr-metadata-2.0.9/nr_metadata/data/services/records/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 from invenio_records_resources.services import RecordLink
 from invenio_records_resources.services import (
     RecordServiceConfig as InvenioRecordServiceConfig,
 )
 from invenio_records_resources.services import pagination_links
 from invenio_records_resources.services.records.components import DataComponent
 from oarepo_runtime.services.config.service import PermissionsPresetsConfigMixin
-from oarepo_runtime.services.results import RecordList
 
-from nr_metadata.common.records.api import CommonRecord
-from nr_metadata.common.services.records.permissions import CommonPermissionPolicy
-from nr_metadata.common.services.records.schema_common import NRCommonRecordSchema
-from nr_metadata.common.services.records.search import CommonSearchOptions
+from nr_metadata.data.records.api import DataRecord
+from nr_metadata.data.services.records.permissions import DataPermissionPolicy
+from nr_metadata.data.services.records.results import DataRecordItem, DataRecordList
+from nr_metadata.data.services.records.schema import NRDataRecordSchema
+from nr_metadata.data.services.records.search import DataSearchOptions
 
 
-class CommonServiceConfig(PermissionsPresetsConfigMixin, InvenioRecordServiceConfig):
-    """CommonRecord service config."""
+class DataServiceConfig(PermissionsPresetsConfigMixin, InvenioRecordServiceConfig):
+    """DataRecord service config."""
 
-    result_list_cls = RecordList
+    result_item_cls = DataRecordItem
+
+    result_list_cls = DataRecordList
 
     PERMISSIONS_PRESETS = ["everyone"]
 
-    url_prefix = "/nr-metadata-common/"
+    url_prefix = "/nr-metadata-data/"
 
-    base_permission_policy_cls = CommonPermissionPolicy
+    base_permission_policy_cls = DataPermissionPolicy
 
-    schema = NRCommonRecordSchema
+    schema = NRDataRecordSchema
 
-    search = CommonSearchOptions
+    search = DataSearchOptions
 
-    record_cls = CommonRecord
+    record_cls = DataRecord
 
-    service_id = "common"
+    service_id = "data"
 
     components = [
         *PermissionsPresetsConfigMixin.components,
         *InvenioRecordServiceConfig.components,
         DataComponent,
     ]
 
-    model = "nr_metadata.common"
+    model = "nr_metadata.data"
 
     @property
     def links_item(self):
         return {
-            "self": RecordLink("{+api}/nr-metadata-common/{id}"),
-            "self_html": RecordLink("{+ui}/nr-metadata-common/{id}"),
+            "self": RecordLink("{+api}/nr-metadata-data/{id}"),
+            "self_html": RecordLink("{+ui}/nr-metadata-data/{id}"),
         }
 
     @property
     def links_search(self):
         return {
-            **pagination_links("{+api}/nr-metadata-common/{?args*}"),
+            **pagination_links("{+api}/nr-metadata-data/{?args*}"),
         }
```

### Comparing `nr-metadata-2.0.8/nr_metadata/common/services/records/facets.py` & `nr-metadata-2.0.9/nr_metadata/common/services/records/facets.py`

 * *Files 8% similar despite different names*

```diff
@@ -81,30 +81,40 @@
 )
 
 metadata_contributors_authorityIdentifiers_scheme = TermsFacet(
     field="metadata.contributors.authorityIdentifiers.scheme",
     label=_("metadata/contributors/authorityIdentifiers/scheme.label"),
 )
 
+metadata_contributors_contributorType = VocabularyFacet(
+    field="metadata.contributors.contributorType",
+    label=_("metadata/contributors/contributorType.label"),
+    vocabulary="contributor-types",
+)
+
+metadata_contributors_familyName = TermsFacet(
+    field="metadata.contributors.familyName",
+    label=_("metadata/contributors/familyName.label"),
+)
+
 metadata_contributors_fullName = TermsFacet(
     field="metadata.contributors.fullName",
     label=_("metadata/contributors/fullName.label"),
 )
 
+metadata_contributors_givenName = TermsFacet(
+    field="metadata.contributors.givenName",
+    label=_("metadata/contributors/givenName.label"),
+)
+
 metadata_contributors_nameType = TermsFacet(
     field="metadata.contributors.nameType",
     label=_("metadata/contributors/nameType.label"),
 )
 
-metadata_contributors_role = VocabularyFacet(
-    field="metadata.contributors.role",
-    label=_("metadata/contributors/role.label"),
-    vocabulary="contributor-roles",
-)
-
 metadata_creators_affiliations = HierarchyVocabularyFacet(
     field="metadata.creators.affiliations",
     label=_("metadata/creators/affiliations.label"),
     vocabulary="institutions",
 )
 
 metadata_creators_authorityIdentifiers_identifier = TermsFacet(
@@ -113,50 +123,49 @@
 )
 
 metadata_creators_authorityIdentifiers_scheme = TermsFacet(
     field="metadata.creators.authorityIdentifiers.scheme",
     label=_("metadata/creators/authorityIdentifiers/scheme.label"),
 )
 
+metadata_creators_familyName = TermsFacet(
+    field="metadata.creators.familyName", label=_("metadata/creators/familyName.label")
+)
+
 metadata_creators_fullName = TermsFacet(
     field="metadata.creators.fullName", label=_("metadata/creators/fullName.label")
 )
 
+metadata_creators_givenName = TermsFacet(
+    field="metadata.creators.givenName", label=_("metadata/creators/givenName.label")
+)
+
 metadata_creators_nameType = TermsFacet(
     field="metadata.creators.nameType", label=_("metadata/creators/nameType.label")
 )
 
 metadata_dateAvailable = DateTimeFacet(
     field="metadata.dateAvailable", label=_("metadata/dateAvailable.label")
 )
 
 metadata_dateIssued = DateTimeFacet(
     field="metadata.dateIssued", label=_("metadata/dateIssued.label")
 )
 
-metadata_dateModified = DateTimeFacet(
-    field="metadata.dateModified", label=_("metadata/dateModified.label")
-)
-
 metadata_events_eventLocation_country = VocabularyFacet(
     field="metadata.events.eventLocation.country",
     label=_("metadata/events/eventLocation/country.label"),
     vocabulary="countries",
 )
 
 metadata_events_eventLocation_place = TermsFacet(
     field="metadata.events.eventLocation.place",
     label=_("metadata/events/eventLocation/place.label"),
 )
 
-metadata_externalLocation_externalLocationURL = TermsFacet(
-    field="metadata.externalLocation.externalLocationURL",
-    label=_("metadata/externalLocation/externalLocationURL.label"),
-)
-
 metadata_fundingReferences_funder = VocabularyFacet(
     field="metadata.fundingReferences.funder",
     label=_("metadata/fundingReferences/funder.label"),
     vocabulary="funders",
 )
 
 metadata_fundingReferences_projectID = TermsFacet(
@@ -228,30 +237,40 @@
 )
 
 metadata_relatedItems_itemContributors_authorityIdentifiers_scheme = TermsFacet(
     field="metadata.relatedItems.itemContributors.authorityIdentifiers.scheme",
     label=_("metadata/relatedItems/itemContributors/authorityIdentifiers/scheme.label"),
 )
 
+metadata_relatedItems_itemContributors_contributorType = VocabularyFacet(
+    field="metadata.relatedItems.itemContributors.contributorType",
+    label=_("metadata/relatedItems/itemContributors/contributorType.label"),
+    vocabulary="contributor-types",
+)
+
+metadata_relatedItems_itemContributors_familyName = TermsFacet(
+    field="metadata.relatedItems.itemContributors.familyName",
+    label=_("metadata/relatedItems/itemContributors/familyName.label"),
+)
+
 metadata_relatedItems_itemContributors_fullName = TermsFacet(
     field="metadata.relatedItems.itemContributors.fullName",
     label=_("metadata/relatedItems/itemContributors/fullName.label"),
 )
 
+metadata_relatedItems_itemContributors_givenName = TermsFacet(
+    field="metadata.relatedItems.itemContributors.givenName",
+    label=_("metadata/relatedItems/itemContributors/givenName.label"),
+)
+
 metadata_relatedItems_itemContributors_nameType = TermsFacet(
     field="metadata.relatedItems.itemContributors.nameType",
     label=_("metadata/relatedItems/itemContributors/nameType.label"),
 )
 
-metadata_relatedItems_itemContributors_role = VocabularyFacet(
-    field="metadata.relatedItems.itemContributors.role",
-    label=_("metadata/relatedItems/itemContributors/role.label"),
-    vocabulary="contributor-roles",
-)
-
 metadata_relatedItems_itemCreators_affiliations = HierarchyVocabularyFacet(
     field="metadata.relatedItems.itemCreators.affiliations",
     label=_("metadata/relatedItems/itemCreators/affiliations.label"),
     vocabulary="institutions",
 )
 
 metadata_relatedItems_itemCreators_authorityIdentifiers_identifier = TermsFacet(
@@ -260,19 +279,29 @@
 )
 
 metadata_relatedItems_itemCreators_authorityIdentifiers_scheme = TermsFacet(
     field="metadata.relatedItems.itemCreators.authorityIdentifiers.scheme",
     label=_("metadata/relatedItems/itemCreators/authorityIdentifiers/scheme.label"),
 )
 
+metadata_relatedItems_itemCreators_familyName = TermsFacet(
+    field="metadata.relatedItems.itemCreators.familyName",
+    label=_("metadata/relatedItems/itemCreators/familyName.label"),
+)
+
 metadata_relatedItems_itemCreators_fullName = TermsFacet(
     field="metadata.relatedItems.itemCreators.fullName",
     label=_("metadata/relatedItems/itemCreators/fullName.label"),
 )
 
+metadata_relatedItems_itemCreators_givenName = TermsFacet(
+    field="metadata.relatedItems.itemCreators.givenName",
+    label=_("metadata/relatedItems/itemCreators/givenName.label"),
+)
+
 metadata_relatedItems_itemCreators_nameType = TermsFacet(
     field="metadata.relatedItems.itemCreators.nameType",
     label=_("metadata/relatedItems/itemCreators/nameType.label"),
 )
 
 metadata_relatedItems_itemEndPage = TermsFacet(
     field="metadata.relatedItems.itemEndPage",
@@ -334,15 +363,15 @@
 metadata_resourceType = VocabularyFacet(
     field="metadata.resourceType",
     label=_("metadata/resourceType.label"),
     vocabulary="resource-types",
 )
 
 metadata_rights = VocabularyFacet(
-    field="metadata.rights", label=_("metadata/rights.label"), vocabulary="licenses"
+    field="metadata.rights", label=_("metadata/rights.label"), vocabulary="rights"
 )
 
 metadata_series_seriesTitle = TermsFacet(
     field="metadata.series.seriesTitle", label=_("metadata/series/seriesTitle.label")
 )
 
 metadata_series_seriesVolume = TermsFacet(
```

### Comparing `nr-metadata-2.0.8/nr_metadata/common/services/records/schema_common.py` & `nr-metadata-2.0.9/nr_metadata/common/services/records/schema_common.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,35 +2,41 @@
 from edtf import Date as EDTFDate
 from marshmallow import Schema
 from marshmallow import fields as ma_fields
 from marshmallow.validate import OneOf
 from marshmallow_utils.fields import TrimmedString
 from oarepo_runtime.services.schema.i18n import I18nStrField, MultilingualField
 from oarepo_runtime.services.schema.marshmallow import BaseRecordSchema, DictOnlySchema
-from oarepo_runtime.services.schema.validation import CachedMultilayerEDTFValidator
+from oarepo_runtime.services.schema.polymorphic import PolymorphicSchema
+from oarepo_runtime.services.schema.validation import (
+    CachedMultilayerEDTFValidator,
+    validate_date,
+)
 
 from nr_metadata.common.services.records.schema_datatypes import (
     NRAccessRightsVocabularySchema,
     NRAffiliationVocabularySchema,
-    NRAuthorityRoleVocabularySchema,
+    NRContributorTypeVocabularySchema,
     NREventSchema,
-    NRExternalLocationSchema,
     NRFundingReferenceSchema,
     NRGeoLocationSchema,
     NRLanguageVocabularySchema,
-    NRLicenseVocabularySchema,
+    NROrganizationSchema,
+    NRPersonSchema,
     NRRelatedItemSchema,
     NRResourceTypeVocabularySchema,
+    NRRightsVocabularySchema,
     NRSeriesSchema,
     NRSubjectCategoryVocabularySchema,
     NRSubjectSchema,
 )
 from nr_metadata.schema.identifiers import (
-    NRAuthorityIdentifierSchema,
     NRObjectIdentifierSchema,
+    NROrganizationIdentifierSchema,
+    NRPersonIdentifierSchema,
     NRSystemIdentifierSchema,
 )
 
 
 class NRCommonRecordSchema(BaseRecordSchema):
     class Meta:
         unknown = ma.RAISE
@@ -56,61 +62,47 @@
 
     creators = ma_fields.List(
         ma_fields.Nested(lambda: NRCreatorSchema()),
         required=True,
         validate=[ma.validate.Length(min=1)],
     )
 
-    dateAvailable = TrimmedString(
-        validate=[CachedMultilayerEDTFValidator(types=(EDTFDate,))]
-    )
+    dateAvailable = ma_fields.String(validate=[validate_date("%Y-%m-%d")])
 
     dateIssued = TrimmedString(
         validate=[CachedMultilayerEDTFValidator(types=(EDTFDate,))]
     )
 
-    dateModified = TrimmedString(
-        validate=[CachedMultilayerEDTFValidator(types=(EDTFDate,))]
-    )
-
     events = ma_fields.List(ma_fields.Nested(lambda: NREventSchema()))
 
-    externalLocation = ma_fields.Nested(lambda: NRExternalLocationSchema())
-
     fundingReferences = ma_fields.List(
         ma_fields.Nested(lambda: NRFundingReferenceSchema())
     )
 
     geoLocations = ma_fields.List(ma_fields.Nested(lambda: NRGeoLocationSchema()))
 
-    languages = ma_fields.List(
-        ma_fields.Nested(lambda: NRLanguageVocabularySchema()),
-        required=True,
-        validate=[ma.validate.Length(min=1)],
-    )
+    languages = ma_fields.List(ma_fields.Nested(lambda: NRLanguageVocabularySchema()))
 
     methods = MultilingualField(I18nStrField())
 
     notes = ma_fields.List(ma_fields.String())
 
     objectIdentifiers = ma_fields.List(
         ma_fields.Nested(lambda: NRObjectIdentifierSchema())
     )
 
     originalRecord = ma_fields.String()
 
-    publishers = ma_fields.List(ma_fields.String())
-
     relatedItems = ma_fields.List(ma_fields.Nested(lambda: NRRelatedItemSchema()))
 
     resourceType = ma_fields.Nested(
         lambda: NRResourceTypeVocabularySchema(), required=True
     )
 
-    rights = ma_fields.Nested(lambda: NRLicenseVocabularySchema())
+    rights = ma_fields.Nested(lambda: NRRightsVocabularySchema())
 
     series = ma_fields.List(ma_fields.Nested(lambda: NRSeriesSchema()))
 
     subjectCategories = ma_fields.List(
         ma_fields.Nested(lambda: NRSubjectCategoryVocabularySchema())
     )
 
@@ -123,53 +115,77 @@
     technicalInfo = MultilingualField(I18nStrField())
 
     title = ma_fields.String(required=True)
 
     version = ma_fields.String()
 
 
+class NRContributorSchema(PolymorphicSchema):
+    class Meta:
+        unknown = ma.RAISE
+
+    Organizational = ma_fields.Nested(lambda: NRContributorOrganizationSchema())
+
+    Personal = ma_fields.Nested(lambda: NRContributorPersonSchema())
+
+    type_field = "nameType"
+
+
 class AdditionalTitlesSchema(DictOnlySchema):
     class Meta:
         unknown = ma.RAISE
 
     title = I18nStrField(required=True)
 
     titleType = ma_fields.String(
         required=True,
         validate=[OneOf(["translatedTitle", "alternativeTitle", "subtitle", "other"])],
     )
 
 
-class NRContributorSchema(DictOnlySchema):
+class NRContributorOrganizationSchema(DictOnlySchema):
     class Meta:
         unknown = ma.RAISE
 
-    affiliations = ma_fields.List(
-        ma_fields.Nested(lambda: NRAffiliationVocabularySchema())
-    )
-
     authorityIdentifiers = ma_fields.List(
-        ma_fields.Nested(lambda: NRAuthorityIdentifierSchema())
+        ma_fields.Nested(lambda: NROrganizationIdentifierSchema())
     )
 
-    fullName = ma_fields.String(required=True)
+    contributorType = ma_fields.Nested(lambda: NRContributorTypeVocabularySchema())
 
-    nameType = ma_fields.String(validate=[OneOf(["Organizational", "Personal"])])
+    fullName = ma_fields.String(required=True)
 
-    role = ma_fields.Nested(lambda: NRAuthorityRoleVocabularySchema())
+    nameType = ma_fields.String(validate=[OneOf(["Organizational"])])
 
 
-class NRCreatorSchema(DictOnlySchema):
+class NRContributorPersonSchema(DictOnlySchema):
     class Meta:
         unknown = ma.RAISE
 
     affiliations = ma_fields.List(
         ma_fields.Nested(lambda: NRAffiliationVocabularySchema())
     )
 
     authorityIdentifiers = ma_fields.List(
-        ma_fields.Nested(lambda: NRAuthorityIdentifierSchema())
+        ma_fields.Nested(lambda: NRPersonIdentifierSchema())
     )
 
+    contributorType = ma_fields.Nested(lambda: NRContributorTypeVocabularySchema())
+
+    familyName = ma_fields.String()
+
     fullName = ma_fields.String(required=True)
 
-    nameType = ma_fields.String(validate=[OneOf(["Organizational", "Personal"])])
+    givenName = ma_fields.String()
+
+    nameType = ma_fields.String(validate=[OneOf(["Personal"])])
+
+
+class NRCreatorSchema(PolymorphicSchema):
+    class Meta:
+        unknown = ma.RAISE
+
+    Organizational = ma_fields.Nested(lambda: NROrganizationSchema())
+
+    Personal = ma_fields.Nested(lambda: NRPersonSchema())
+
+    type_field = "nameType"
```

### Comparing `nr-metadata-2.0.8/nr_metadata/common/services/records/schema_datatypes.py` & `nr-metadata-2.0.9/nr_metadata/common/services/records/schema_datatypes.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,38 +3,25 @@
 from invenio_vocabularies.services.schema import i18n_strings
 from marshmallow import fields as ma_fields
 from marshmallow.fields import String
 from marshmallow.validate import OneOf
 from marshmallow_utils.fields import TrimmedString
 from oarepo_runtime.services.schema.i18n import I18nStrField, MultilingualField
 from oarepo_runtime.services.schema.marshmallow import DictOnlySchema
+from oarepo_runtime.services.schema.polymorphic import PolymorphicSchema
 from oarepo_runtime.services.schema.validation import CachedMultilayerEDTFValidator
 from oarepo_vocabularies.services.schema import HierarchySchema
 
 from nr_metadata.schema.identifiers import (
-    NRAuthorityIdentifierSchema,
     NRObjectIdentifierSchema,
+    NROrganizationIdentifierSchema,
+    NRPersonIdentifierSchema,
 )
 
 
-class NREventSchema(DictOnlySchema):
-    class Meta:
-        unknown = ma.RAISE
-
-    eventDate = TrimmedString(
-        required=True, validate=[CachedMultilayerEDTFValidator(types=(EDTFInterval,))]
-    )
-
-    eventLocation = ma_fields.Nested(lambda: NRLocationSchema(), required=True)
-
-    eventNameAlternate = ma_fields.List(ma_fields.String())
-
-    eventNameOriginal = ma_fields.String(required=True)
-
-
 class NRRelatedItemSchema(DictOnlySchema):
     class Meta:
         unknown = ma.RAISE
 
     itemContributors = ma_fields.List(
         ma_fields.Nested(lambda: NRRelatedItemContributorSchema())
     )
@@ -62,14 +49,53 @@
     itemURL = ma_fields.String()
 
     itemVolume = ma_fields.String()
 
     itemYear = ma_fields.Integer()
 
 
+class NREventSchema(DictOnlySchema):
+    class Meta:
+        unknown = ma.RAISE
+
+    eventDate = TrimmedString(
+        required=True, validate=[CachedMultilayerEDTFValidator(types=(EDTFInterval,))]
+    )
+
+    eventLocation = ma_fields.Nested(lambda: NRLocationSchema(), required=True)
+
+    eventNameAlternate = ma_fields.List(ma_fields.String())
+
+    eventNameOriginal = ma_fields.String(required=True)
+
+
+class NRRelatedItemContributorSchema(PolymorphicSchema):
+    class Meta:
+        unknown = ma.RAISE
+
+    Organizational = ma_fields.Nested(
+        lambda: NRRelatedItemContributorOrganizationSchema()
+    )
+
+    Personal = ma_fields.Nested(lambda: NRRelatedItemContributorPersonSchema())
+
+    type_field = "nameType"
+
+
+class NRRelatedItemCreatorSchema(PolymorphicSchema):
+    class Meta:
+        unknown = ma.RAISE
+
+    Organizational = ma_fields.Nested(lambda: NROrganizationSchema())
+
+    Personal = ma_fields.Nested(lambda: NRPersonSchema())
+
+    type_field = "nameType"
+
+
 class NRFundingReferenceSchema(DictOnlySchema):
     class Meta:
         unknown = ma.RAISE
 
     funder = ma_fields.Nested(lambda: NRFunderVocabularySchema())
 
     fundingProgram = ma_fields.String()
@@ -79,62 +105,85 @@
     projectName = ma_fields.String()
 
 
 class NRGeoLocationSchema(DictOnlySchema):
     class Meta:
         unknown = ma.RAISE
 
-    geoLocationPlace = ma_fields.String(required=True)
+    geoLocationPlace = ma_fields.String()
 
     geoLocationPoint = ma_fields.Nested(lambda: NRGeoLocationPointSchema())
 
 
 class NRLocationSchema(DictOnlySchema):
     class Meta:
         unknown = ma.RAISE
 
     country = ma_fields.Nested(lambda: NRCountryVocabularySchema())
 
     place = ma_fields.String(required=True)
 
 
-class NRRelatedItemContributorSchema(DictOnlySchema):
+class NRPersonSchema(DictOnlySchema):
     class Meta:
         unknown = ma.RAISE
 
     affiliations = ma_fields.List(
         ma_fields.Nested(lambda: NRAffiliationVocabularySchema())
     )
 
     authorityIdentifiers = ma_fields.List(
-        ma_fields.Nested(lambda: NRAuthorityIdentifierSchema())
+        ma_fields.Nested(lambda: NRPersonIdentifierSchema())
     )
 
+    familyName = ma_fields.String()
+
     fullName = ma_fields.String(required=True)
 
-    nameType = ma_fields.String(validate=[OneOf(["Organizational", "Personal"])])
+    givenName = ma_fields.String()
 
-    role = ma_fields.Nested(lambda: NRAuthorityRoleVocabularySchema())
+    nameType = ma_fields.String(validate=[OneOf(["Personal"])])
 
 
-class NRRelatedItemCreatorSchema(DictOnlySchema):
+class NRRelatedItemContributorOrganizationSchema(DictOnlySchema):
+    class Meta:
+        unknown = ma.RAISE
+
+    authorityIdentifiers = ma_fields.List(
+        ma_fields.Nested(lambda: NROrganizationIdentifierSchema())
+    )
+
+    contributorType = ma_fields.Nested(lambda: NRContributorTypeVocabularySchema())
+
+    fullName = ma_fields.String(required=True)
+
+    nameType = ma_fields.String(validate=[OneOf(["Organizational"])])
+
+
+class NRRelatedItemContributorPersonSchema(DictOnlySchema):
     class Meta:
         unknown = ma.RAISE
 
     affiliations = ma_fields.List(
         ma_fields.Nested(lambda: NRAffiliationVocabularySchema())
     )
 
     authorityIdentifiers = ma_fields.List(
-        ma_fields.Nested(lambda: NRAuthorityIdentifierSchema())
+        ma_fields.Nested(lambda: NRPersonIdentifierSchema())
     )
 
+    contributorType = ma_fields.Nested(lambda: NRContributorTypeVocabularySchema())
+
+    familyName = ma_fields.String()
+
     fullName = ma_fields.String(required=True)
 
-    nameType = ma_fields.String(validate=[OneOf(["Organizational", "Personal"])])
+    givenName = ma_fields.String()
+
+    nameType = ma_fields.String(validate=[OneOf(["Personal"])])
 
 
 class NRAccessRightsVocabularySchema(DictOnlySchema):
     class Meta:
         unknown = ma.INCLUDE
 
     _id = String(data_key="id", attribute="id")
@@ -150,18 +199,20 @@
 
     _id = String(data_key="id", attribute="id")
 
     _version = String(data_key="@v", attribute="@v")
 
     hierarchy = ma_fields.Nested(lambda: HierarchySchema())
 
+    ror = ma_fields.String()
+
     title = i18n_strings
 
 
-class NRAuthorityRoleVocabularySchema(DictOnlySchema):
+class NRContributorTypeVocabularySchema(DictOnlySchema):
     class Meta:
         unknown = ma.INCLUDE
 
     _id = String(data_key="id", attribute="id")
 
     _version = String(data_key="@v", attribute="@v")
 
@@ -175,23 +226,14 @@
     _id = String(data_key="id", attribute="id")
 
     _version = String(data_key="@v", attribute="@v")
 
     title = i18n_strings
 
 
-class NRExternalLocationSchema(DictOnlySchema):
-    class Meta:
-        unknown = ma.RAISE
-
-    externalLocationNote = ma_fields.String()
-
-    externalLocationURL = ma_fields.String(required=True)
-
-
 class NRFunderVocabularySchema(DictOnlySchema):
     class Meta:
         unknown = ma.INCLUDE
 
     _id = String(data_key="id", attribute="id")
 
     _version = String(data_key="@v", attribute="@v")
@@ -230,26 +272,39 @@
     _id = String(data_key="id", attribute="id")
 
     _version = String(data_key="@v", attribute="@v")
 
     title = i18n_strings
 
 
-class NRLicenseVocabularySchema(DictOnlySchema):
+class NROrganizationSchema(DictOnlySchema):
+    class Meta:
+        unknown = ma.RAISE
+
+    authorityIdentifiers = ma_fields.List(
+        ma_fields.Nested(lambda: NROrganizationIdentifierSchema())
+    )
+
+    fullName = ma_fields.String(required=True)
+
+    nameType = ma_fields.String(validate=[OneOf(["Organizational"])])
+
+
+class NRResourceTypeVocabularySchema(DictOnlySchema):
     class Meta:
         unknown = ma.INCLUDE
 
     _id = String(data_key="id", attribute="id")
 
     _version = String(data_key="@v", attribute="@v")
 
     title = i18n_strings
 
 
-class NRResourceTypeVocabularySchema(DictOnlySchema):
+class NRRightsVocabularySchema(DictOnlySchema):
     class Meta:
         unknown = ma.INCLUDE
 
     _id = String(data_key="id", attribute="id")
 
     _version = String(data_key="@v", attribute="@v")
 
@@ -283,7 +338,16 @@
     classificationCode = ma_fields.String()
 
     subject = MultilingualField(I18nStrField(), required=True)
 
     subjectScheme = ma_fields.String()
 
     valueURI = ma_fields.String()
+
+
+class NRExternalLocationSchema(DictOnlySchema):
+    class Meta:
+        unknown = ma.RAISE
+
+    externalLocationNote = ma_fields.String()
+
+    externalLocationURL = ma_fields.String(required=True)
```

### Comparing `nr-metadata-2.0.8/nr_metadata/common/services/records/search.py` & `nr-metadata-2.0.9/nr_metadata/data/services/records/search.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,178 +1,102 @@
 from invenio_records_resources.services import SearchOptions as InvenioSearchOptions
 
 from . import facets
 
 
-class CommonSearchOptions(InvenioSearchOptions):
-    """CommonRecord search options."""
+class DataSearchOptions(InvenioSearchOptions):
+    """DataRecord search options."""
 
-    facet_groups = {
-        "default": {
-            "metadata_abstract_cs": facets.metadata_abstract_cs,
-            "metadata_abstract_en": facets.metadata_abstract_en,
-            "metadata_accessibility_cs": facets.metadata_accessibility_cs,
-            "metadata_accessibility_en": facets.metadata_accessibility_en,
-            "metadata_additionalTitles_title_cs": (
-                facets.metadata_additionalTitles_title_cs
-            ),
-            "metadata_additionalTitles_title_en": (
-                facets.metadata_additionalTitles_title_en
-            ),
-            "metadata_methods_cs": facets.metadata_methods_cs,
-            "metadata_methods_en": facets.metadata_methods_en,
-            "metadata_subjects_subject_cs": facets.metadata_subjects_subject_cs,
-            "metadata_subjects_subject_en": facets.metadata_subjects_subject_en,
-            "metadata_technicalInfo_cs": facets.metadata_technicalInfo_cs,
-            "metadata_technicalInfo_en": facets.metadata_technicalInfo_en,
-            **getattr(InvenioSearchOptions, "facet_groups", {}).get("default", {}),
-        },
-    }
+    facet_groups = {}
 
     facets = {
         "metadata_abstract_cs": facets.metadata_abstract_cs,
         "metadata_abstract_en": facets.metadata_abstract_en,
         "metadata_abstract_lang": facets.metadata_abstract_lang,
         "metadata_accessRights": facets.metadata_accessRights,
         "metadata_accessibility_cs": facets.metadata_accessibility_cs,
         "metadata_accessibility_en": facets.metadata_accessibility_en,
         "metadata_accessibility_lang": facets.metadata_accessibility_lang,
         "metadata_additionalTitles_title_cs": facets.metadata_additionalTitles_title_cs,
         "metadata_additionalTitles_title_en": facets.metadata_additionalTitles_title_en,
-        "metadata_additionalTitles_title_lang": (
-            facets.metadata_additionalTitles_title_lang
-        ),
-        "metadata_additionalTitles_titleType": (
-            facets.metadata_additionalTitles_titleType
-        ),
+        "metadata_additionalTitles_title_lang": facets.metadata_additionalTitles_title_lang,
+        "metadata_additionalTitles_titleType": facets.metadata_additionalTitles_titleType,
         "metadata_contributors_affiliations": facets.metadata_contributors_affiliations,
-        "metadata_contributors_authorityIdentifiers_identifier": (
-            facets.metadata_contributors_authorityIdentifiers_identifier
-        ),
-        "metadata_contributors_authorityIdentifiers_scheme": (
-            facets.metadata_contributors_authorityIdentifiers_scheme
-        ),
+        "metadata_contributors_authorityIdentifiers_identifier": facets.metadata_contributors_authorityIdentifiers_identifier,
+        "metadata_contributors_authorityIdentifiers_scheme": facets.metadata_contributors_authorityIdentifiers_scheme,
+        "metadata_contributors_contributorType": facets.metadata_contributors_contributorType,
+        "metadata_contributors_familyName": facets.metadata_contributors_familyName,
         "metadata_contributors_fullName": facets.metadata_contributors_fullName,
+        "metadata_contributors_givenName": facets.metadata_contributors_givenName,
         "metadata_contributors_nameType": facets.metadata_contributors_nameType,
-        "metadata_contributors_role": facets.metadata_contributors_role,
         "metadata_creators_affiliations": facets.metadata_creators_affiliations,
-        "metadata_creators_authorityIdentifiers_identifier": (
-            facets.metadata_creators_authorityIdentifiers_identifier
-        ),
-        "metadata_creators_authorityIdentifiers_scheme": (
-            facets.metadata_creators_authorityIdentifiers_scheme
-        ),
+        "metadata_creators_authorityIdentifiers_identifier": facets.metadata_creators_authorityIdentifiers_identifier,
+        "metadata_creators_authorityIdentifiers_scheme": facets.metadata_creators_authorityIdentifiers_scheme,
+        "metadata_creators_familyName": facets.metadata_creators_familyName,
         "metadata_creators_fullName": facets.metadata_creators_fullName,
+        "metadata_creators_givenName": facets.metadata_creators_givenName,
         "metadata_creators_nameType": facets.metadata_creators_nameType,
         "metadata_dateAvailable": facets.metadata_dateAvailable,
         "metadata_dateIssued": facets.metadata_dateIssued,
-        "metadata_dateModified": facets.metadata_dateModified,
-        "metadata_events_eventLocation_country": (
-            facets.metadata_events_eventLocation_country
-        ),
-        "metadata_events_eventLocation_place": (
-            facets.metadata_events_eventLocation_place
-        ),
-        "metadata_externalLocation_externalLocationURL": (
-            facets.metadata_externalLocation_externalLocationURL
-        ),
+        "metadata_dateValidTo": facets.metadata_dateValidTo,
+        "metadata_dateWithdrawn_dateInformation": facets.metadata_dateWithdrawn_dateInformation,
+        "metadata_dateWithdrawn_type": facets.metadata_dateWithdrawn_type,
+        "metadata_events_eventLocation_country": facets.metadata_events_eventLocation_country,
+        "metadata_events_eventLocation_place": facets.metadata_events_eventLocation_place,
         "metadata_fundingReferences_funder": facets.metadata_fundingReferences_funder,
-        "metadata_fundingReferences_projectID": (
-            facets.metadata_fundingReferences_projectID
-        ),
-        "metadata_geoLocations_geoLocationPlace": (
-            facets.metadata_geoLocations_geoLocationPlace
-        ),
-        "metadata_geoLocations_geoLocationPoint_pointLatitude": (
-            facets.metadata_geoLocations_geoLocationPoint_pointLatitude
-        ),
-        "metadata_geoLocations_geoLocationPoint_pointLongitude": (
-            facets.metadata_geoLocations_geoLocationPoint_pointLongitude
-        ),
+        "metadata_fundingReferences_projectID": facets.metadata_fundingReferences_projectID,
+        "metadata_geoLocations_geoLocationPlace": facets.metadata_geoLocations_geoLocationPlace,
+        "metadata_geoLocations_geoLocationPoint_pointLatitude": facets.metadata_geoLocations_geoLocationPoint_pointLatitude,
+        "metadata_geoLocations_geoLocationPoint_pointLongitude": facets.metadata_geoLocations_geoLocationPoint_pointLongitude,
         "metadata_languages": facets.metadata_languages,
         "metadata_methods_cs": facets.metadata_methods_cs,
         "metadata_methods_en": facets.metadata_methods_en,
         "metadata_methods_lang": facets.metadata_methods_lang,
-        "metadata_objectIdentifiers_identifier": (
-            facets.metadata_objectIdentifiers_identifier
-        ),
+        "metadata_objectIdentifiers_identifier": facets.metadata_objectIdentifiers_identifier,
         "metadata_objectIdentifiers_scheme": facets.metadata_objectIdentifiers_scheme,
         "metadata_originalRecord": facets.metadata_originalRecord,
-        "metadata_relatedItems_itemContributors_affiliations": (
-            facets.metadata_relatedItems_itemContributors_affiliations
-        ),
-        "metadata_relatedItems_itemContributors_authorityIdentifiers_identifier": (
-            facets.metadata_relatedItems_itemContributors_authorityIdentifiers_identifier
-        ),
-        "metadata_relatedItems_itemContributors_authorityIdentifiers_scheme": (
-            facets.metadata_relatedItems_itemContributors_authorityIdentifiers_scheme
-        ),
-        "metadata_relatedItems_itemContributors_fullName": (
-            facets.metadata_relatedItems_itemContributors_fullName
-        ),
-        "metadata_relatedItems_itemContributors_nameType": (
-            facets.metadata_relatedItems_itemContributors_nameType
-        ),
-        "metadata_relatedItems_itemContributors_role": (
-            facets.metadata_relatedItems_itemContributors_role
-        ),
-        "metadata_relatedItems_itemCreators_affiliations": (
-            facets.metadata_relatedItems_itemCreators_affiliations
-        ),
-        "metadata_relatedItems_itemCreators_authorityIdentifiers_identifier": (
-            facets.metadata_relatedItems_itemCreators_authorityIdentifiers_identifier
-        ),
-        "metadata_relatedItems_itemCreators_authorityIdentifiers_scheme": (
-            facets.metadata_relatedItems_itemCreators_authorityIdentifiers_scheme
-        ),
-        "metadata_relatedItems_itemCreators_fullName": (
-            facets.metadata_relatedItems_itemCreators_fullName
-        ),
-        "metadata_relatedItems_itemCreators_nameType": (
-            facets.metadata_relatedItems_itemCreators_nameType
-        ),
+        "metadata_publishers": facets.metadata_publishers,
+        "metadata_relatedItems_itemContributors_affiliations": facets.metadata_relatedItems_itemContributors_affiliations,
+        "metadata_relatedItems_itemContributors_authorityIdentifiers_identifier": facets.metadata_relatedItems_itemContributors_authorityIdentifiers_identifier,
+        "metadata_relatedItems_itemContributors_authorityIdentifiers_scheme": facets.metadata_relatedItems_itemContributors_authorityIdentifiers_scheme,
+        "metadata_relatedItems_itemContributors_contributorType": facets.metadata_relatedItems_itemContributors_contributorType,
+        "metadata_relatedItems_itemContributors_familyName": facets.metadata_relatedItems_itemContributors_familyName,
+        "metadata_relatedItems_itemContributors_fullName": facets.metadata_relatedItems_itemContributors_fullName,
+        "metadata_relatedItems_itemContributors_givenName": facets.metadata_relatedItems_itemContributors_givenName,
+        "metadata_relatedItems_itemContributors_nameType": facets.metadata_relatedItems_itemContributors_nameType,
+        "metadata_relatedItems_itemCreators_affiliations": facets.metadata_relatedItems_itemCreators_affiliations,
+        "metadata_relatedItems_itemCreators_authorityIdentifiers_identifier": facets.metadata_relatedItems_itemCreators_authorityIdentifiers_identifier,
+        "metadata_relatedItems_itemCreators_authorityIdentifiers_scheme": facets.metadata_relatedItems_itemCreators_authorityIdentifiers_scheme,
+        "metadata_relatedItems_itemCreators_familyName": facets.metadata_relatedItems_itemCreators_familyName,
+        "metadata_relatedItems_itemCreators_fullName": facets.metadata_relatedItems_itemCreators_fullName,
+        "metadata_relatedItems_itemCreators_givenName": facets.metadata_relatedItems_itemCreators_givenName,
+        "metadata_relatedItems_itemCreators_nameType": facets.metadata_relatedItems_itemCreators_nameType,
         "metadata_relatedItems_itemEndPage": facets.metadata_relatedItems_itemEndPage,
         "metadata_relatedItems_itemIssue": facets.metadata_relatedItems_itemIssue,
-        "metadata_relatedItems_itemPIDs_identifier": (
-            facets.metadata_relatedItems_itemPIDs_identifier
-        ),
-        "metadata_relatedItems_itemPIDs_scheme": (
-            facets.metadata_relatedItems_itemPIDs_scheme
-        ),
-        "metadata_relatedItems_itemPublisher": (
-            facets.metadata_relatedItems_itemPublisher
-        ),
-        "metadata_relatedItems_itemRelationType": (
-            facets.metadata_relatedItems_itemRelationType
-        ),
-        "metadata_relatedItems_itemResourceType": (
-            facets.metadata_relatedItems_itemResourceType
-        ),
-        "metadata_relatedItems_itemStartPage": (
-            facets.metadata_relatedItems_itemStartPage
-        ),
+        "metadata_relatedItems_itemPIDs_identifier": facets.metadata_relatedItems_itemPIDs_identifier,
+        "metadata_relatedItems_itemPIDs_scheme": facets.metadata_relatedItems_itemPIDs_scheme,
+        "metadata_relatedItems_itemPublisher": facets.metadata_relatedItems_itemPublisher,
+        "metadata_relatedItems_itemRelationType": facets.metadata_relatedItems_itemRelationType,
+        "metadata_relatedItems_itemResourceType": facets.metadata_relatedItems_itemResourceType,
+        "metadata_relatedItems_itemStartPage": facets.metadata_relatedItems_itemStartPage,
         "metadata_relatedItems_itemURL": facets.metadata_relatedItems_itemURL,
         "metadata_relatedItems_itemVolume": facets.metadata_relatedItems_itemVolume,
         "metadata_relatedItems_itemYear": facets.metadata_relatedItems_itemYear,
         "metadata_resourceType": facets.metadata_resourceType,
         "metadata_rights": facets.metadata_rights,
         "metadata_series_seriesTitle": facets.metadata_series_seriesTitle,
         "metadata_series_seriesVolume": facets.metadata_series_seriesVolume,
         "metadata_subjectCategories": facets.metadata_subjectCategories,
-        "metadata_subjects_classificationCode": (
-            facets.metadata_subjects_classificationCode
-        ),
+        "metadata_subjects_classificationCode": facets.metadata_subjects_classificationCode,
         "metadata_subjects_subject_cs": facets.metadata_subjects_subject_cs,
         "metadata_subjects_subject_en": facets.metadata_subjects_subject_en,
         "metadata_subjects_subject_lang": facets.metadata_subjects_subject_lang,
         "metadata_subjects_subjectScheme": facets.metadata_subjects_subjectScheme,
         "metadata_subjects_valueURI": facets.metadata_subjects_valueURI,
-        "metadata_systemIdentifiers_identifier": (
-            facets.metadata_systemIdentifiers_identifier
-        ),
+        "metadata_systemIdentifiers_identifier": facets.metadata_systemIdentifiers_identifier,
         "metadata_systemIdentifiers_scheme": facets.metadata_systemIdentifiers_scheme,
         "metadata_technicalInfo_cs": facets.metadata_technicalInfo_cs,
         "metadata_technicalInfo_en": facets.metadata_technicalInfo_en,
         "metadata_technicalInfo_lang": facets.metadata_technicalInfo_lang,
         "metadata_version": facets.metadata_version,
         **getattr(InvenioSearchOptions, "facets", {}),
     }
```

### Comparing `nr-metadata-2.0.8/nr_metadata/common/services/records/ui_schema_common.py` & `nr-metadata-2.0.9/nr_metadata/common/services/records/ui_schema_common.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,35 +4,39 @@
 from marshmallow.validate import OneOf
 from oarepo_runtime.services.schema.i18n_ui import (
     I18nStrUIField,
     MultilingualLocalizedUIField,
     MultilingualUIField,
 )
 from oarepo_runtime.services.schema.marshmallow import DictOnlySchema
-from oarepo_runtime.services.schema.ui import InvenioUISchema, LocalizedEDTF
+from oarepo_runtime.services.schema.ui import (
+    InvenioUISchema,
+    LocalizedDate,
+    LocalizedEDTF,
+)
 
 from nr_metadata.common.services.records.ui_schema_datatypes import (
     NRAccessRightsVocabularyUISchema,
     NRAffiliationVocabularyUISchema,
-    NRAuthorityRoleVocabularyUISchema,
+    NRContributorTypeVocabularyUISchema,
     NREventUISchema,
-    NRExternalLocationUISchema,
     NRFundingReferenceUISchema,
     NRGeoLocationUISchema,
     NRLanguageVocabularyUISchema,
-    NRLicenseVocabularyUISchema,
     NRRelatedItemUISchema,
     NRResourceTypeVocabularyUISchema,
+    NRRightsVocabularyUISchema,
     NRSeriesUISchema,
     NRSubjectCategoryVocabularyUISchema,
     NRSubjectUISchema,
 )
 from nr_metadata.ui_schema.identifiers import (
-    NRAuthorityIdentifierUISchema,
     NRObjectIdentifierUISchema,
+    NROrganizationIdentifierUISchema,
+    NRPersonIdentifierUISchema,
     NRSystemIdentifierUISchema,
 )
 from nr_metadata.ui_schema.subjects import NRSubjectListField
 
 
 class NRCommonRecordUISchema(InvenioUISchema):
     class Meta:
@@ -57,53 +61,45 @@
 
     contributors = ma_fields.List(ma_fields.Nested(lambda: NRContributorUISchema()))
 
     creators = ma_fields.List(
         ma_fields.Nested(lambda: NRCreatorUISchema()), required=True
     )
 
-    dateAvailable = LocalizedEDTF()
+    dateAvailable = LocalizedDate()
 
     dateIssued = LocalizedEDTF()
 
-    dateModified = LocalizedEDTF()
-
     events = ma_fields.List(ma_fields.Nested(lambda: NREventUISchema()))
 
-    externalLocation = ma_fields.Nested(lambda: NRExternalLocationUISchema())
-
     fundingReferences = ma_fields.List(
         ma_fields.Nested(lambda: NRFundingReferenceUISchema())
     )
 
     geoLocations = ma_fields.List(ma_fields.Nested(lambda: NRGeoLocationUISchema()))
 
-    languages = ma_fields.List(
-        ma_fields.Nested(lambda: NRLanguageVocabularyUISchema()), required=True
-    )
+    languages = ma_fields.List(ma_fields.Nested(lambda: NRLanguageVocabularyUISchema()))
 
     methods = MultilingualUIField(I18nStrUIField())
 
     notes = ma_fields.List(ma_fields.String())
 
     objectIdentifiers = ma_fields.List(
         ma_fields.Nested(lambda: NRObjectIdentifierUISchema())
     )
 
     originalRecord = ma_fields.String()
 
-    publishers = ma_fields.List(ma_fields.String())
-
     relatedItems = ma_fields.List(ma_fields.Nested(lambda: NRRelatedItemUISchema()))
 
     resourceType = ma_fields.Nested(
         lambda: NRResourceTypeVocabularyUISchema(), required=True
     )
 
-    rights = ma_fields.Nested(lambda: NRLicenseVocabularyUISchema())
+    rights = ma_fields.Nested(lambda: NRRightsVocabularyUISchema())
 
     series = ma_fields.List(ma_fields.Nested(lambda: NRSeriesUISchema()))
 
     subjectCategories = ma_fields.List(
         ma_fields.Nested(lambda: NRSubjectCategoryVocabularyUISchema())
     )
 
@@ -128,41 +124,87 @@
 
     titleType = ma_fields.String(
         required=True,
         validate=[OneOf(["translatedTitle", "alternativeTitle", "subtitle", "other"])],
     )
 
 
+class NRContributorOrganizationUISchema(DictOnlySchema):
+    class Meta:
+        unknown = ma.RAISE
+
+    authorityIdentifiers = ma_fields.List(
+        ma_fields.Nested(lambda: NROrganizationIdentifierUISchema())
+    )
+
+    contributorType = ma_fields.Nested(lambda: NRContributorTypeVocabularyUISchema())
+
+    fullName = ma_fields.String(required=True)
+
+    nameType = ma_fields.String(validate=[OneOf(["Organizational"])])
+
+
+class NRContributorPersonUISchema(DictOnlySchema):
+    class Meta:
+        unknown = ma.RAISE
+
+    affiliations = ma_fields.List(
+        ma_fields.Nested(lambda: NRAffiliationVocabularyUISchema())
+    )
+
+    authorityIdentifiers = ma_fields.List(
+        ma_fields.Nested(lambda: NRPersonIdentifierUISchema())
+    )
+
+    contributorType = ma_fields.Nested(lambda: NRContributorTypeVocabularyUISchema())
+
+    familyName = ma_fields.String()
+
+    fullName = ma_fields.String(required=True)
+
+    givenName = ma_fields.String()
+
+    nameType = ma_fields.String(validate=[OneOf(["Personal"])])
+
+
 class NRContributorUISchema(DictOnlySchema):
     class Meta:
         unknown = ma.RAISE
 
     affiliations = ma_fields.List(
         ma_fields.Nested(lambda: NRAffiliationVocabularyUISchema())
     )
 
     authorityIdentifiers = ma_fields.List(
-        ma_fields.Nested(lambda: NRAuthorityIdentifierUISchema())
+        ma_fields.Nested(lambda: NROrganizationIdentifierUISchema())
     )
 
+    contributorType = ma_fields.Nested(lambda: NRContributorTypeVocabularyUISchema())
+
+    familyName = ma_fields.String()
+
     fullName = ma_fields.String(required=True)
 
-    nameType = ma_fields.String(validate=[OneOf(["Organizational", "Personal"])])
+    givenName = ma_fields.String()
 
-    role = ma_fields.Nested(lambda: NRAuthorityRoleVocabularyUISchema())
+    nameType = ma_fields.String(validate=[OneOf(["Organizational"])])
 
 
 class NRCreatorUISchema(DictOnlySchema):
     class Meta:
         unknown = ma.RAISE
 
     affiliations = ma_fields.List(
         ma_fields.Nested(lambda: NRAffiliationVocabularyUISchema())
     )
 
     authorityIdentifiers = ma_fields.List(
-        ma_fields.Nested(lambda: NRAuthorityIdentifierUISchema())
+        ma_fields.Nested(lambda: NROrganizationIdentifierUISchema())
     )
 
+    familyName = ma_fields.String()
+
     fullName = ma_fields.String(required=True)
 
-    nameType = ma_fields.String(validate=[OneOf(["Organizational", "Personal"])])
+    givenName = ma_fields.String()
+
+    nameType = ma_fields.String(validate=[OneOf(["Organizational"])])
```

### Comparing `nr-metadata-2.0.8/nr_metadata/common/services/records/ui_schema_datatypes.py` & `nr-metadata-2.0.9/nr_metadata/common/services/records/ui_schema_datatypes.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 from oarepo_runtime.services.schema.ui import LocalizedEDTFInterval
 from oarepo_vocabularies.services.ui_schema import (
     HierarchyUISchema,
     VocabularyI18nStrUIField,
 )
 
 from nr_metadata.ui_schema.identifiers import (
-    NRAuthorityIdentifierUISchema,
     NRObjectIdentifierUISchema,
+    NROrganizationIdentifierUISchema,
+    NRPersonIdentifierUISchema,
 )
 
 
 class NREventUISchema(DictOnlySchema):
     class Meta:
         unknown = ma.RAISE
 
@@ -77,62 +78,129 @@
     projectName = ma_fields.String()
 
 
 class NRGeoLocationUISchema(DictOnlySchema):
     class Meta:
         unknown = ma.RAISE
 
-    geoLocationPlace = ma_fields.String(required=True)
+    geoLocationPlace = ma_fields.String()
 
     geoLocationPoint = ma_fields.Nested(lambda: NRGeoLocationPointUISchema())
 
 
 class NRLocationUISchema(DictOnlySchema):
     class Meta:
         unknown = ma.RAISE
 
     country = ma_fields.Nested(lambda: NRCountryVocabularyUISchema())
 
     place = ma_fields.String(required=True)
 
 
+class NRPersonUISchema(DictOnlySchema):
+    class Meta:
+        unknown = ma.RAISE
+
+    affiliations = ma_fields.List(
+        ma_fields.Nested(lambda: NRAffiliationVocabularyUISchema())
+    )
+
+    authorityIdentifiers = ma_fields.List(
+        ma_fields.Nested(lambda: NRPersonIdentifierUISchema())
+    )
+
+    familyName = ma_fields.String()
+
+    fullName = ma_fields.String(required=True)
+
+    givenName = ma_fields.String()
+
+    nameType = ma_fields.String(validate=[OneOf(["Personal"])])
+
+
+class NRRelatedItemContributorOrganizationUISchema(DictOnlySchema):
+    class Meta:
+        unknown = ma.RAISE
+
+    authorityIdentifiers = ma_fields.List(
+        ma_fields.Nested(lambda: NROrganizationIdentifierUISchema())
+    )
+
+    contributorType = ma_fields.Nested(lambda: NRContributorTypeVocabularyUISchema())
+
+    fullName = ma_fields.String(required=True)
+
+    nameType = ma_fields.String(validate=[OneOf(["Organizational"])])
+
+
+class NRRelatedItemContributorPersonUISchema(DictOnlySchema):
+    class Meta:
+        unknown = ma.RAISE
+
+    affiliations = ma_fields.List(
+        ma_fields.Nested(lambda: NRAffiliationVocabularyUISchema())
+    )
+
+    authorityIdentifiers = ma_fields.List(
+        ma_fields.Nested(lambda: NRPersonIdentifierUISchema())
+    )
+
+    contributorType = ma_fields.Nested(lambda: NRContributorTypeVocabularyUISchema())
+
+    familyName = ma_fields.String()
+
+    fullName = ma_fields.String(required=True)
+
+    givenName = ma_fields.String()
+
+    nameType = ma_fields.String(validate=[OneOf(["Personal"])])
+
+
 class NRRelatedItemContributorUISchema(DictOnlySchema):
     class Meta:
         unknown = ma.RAISE
 
     affiliations = ma_fields.List(
         ma_fields.Nested(lambda: NRAffiliationVocabularyUISchema())
     )
 
     authorityIdentifiers = ma_fields.List(
-        ma_fields.Nested(lambda: NRAuthorityIdentifierUISchema())
+        ma_fields.Nested(lambda: NROrganizationIdentifierUISchema())
     )
 
+    contributorType = ma_fields.Nested(lambda: NRContributorTypeVocabularyUISchema())
+
+    familyName = ma_fields.String()
+
     fullName = ma_fields.String(required=True)
 
-    nameType = ma_fields.String(validate=[OneOf(["Organizational", "Personal"])])
+    givenName = ma_fields.String()
 
-    role = ma_fields.Nested(lambda: NRAuthorityRoleVocabularyUISchema())
+    nameType = ma_fields.String(validate=[OneOf(["Organizational"])])
 
 
 class NRRelatedItemCreatorUISchema(DictOnlySchema):
     class Meta:
         unknown = ma.RAISE
 
     affiliations = ma_fields.List(
         ma_fields.Nested(lambda: NRAffiliationVocabularyUISchema())
     )
 
     authorityIdentifiers = ma_fields.List(
-        ma_fields.Nested(lambda: NRAuthorityIdentifierUISchema())
+        ma_fields.Nested(lambda: NROrganizationIdentifierUISchema())
     )
 
+    familyName = ma_fields.String()
+
     fullName = ma_fields.String(required=True)
 
-    nameType = ma_fields.String(validate=[OneOf(["Organizational", "Personal"])])
+    givenName = ma_fields.String()
+
+    nameType = ma_fields.String(validate=[OneOf(["Organizational"])])
 
 
 class NRAccessRightsVocabularyUISchema(DictOnlySchema):
     class Meta:
         unknown = ma.INCLUDE
 
     _id = String(data_key="id", attribute="id")
@@ -148,18 +216,20 @@
 
     _id = String(data_key="id", attribute="id")
 
     _version = String(data_key="@v", attribute="@v")
 
     hierarchy = ma_fields.Nested(lambda: HierarchyUISchema())
 
+    ror = ma_fields.String()
+
     title = VocabularyI18nStrUIField()
 
 
-class NRAuthorityRoleVocabularyUISchema(DictOnlySchema):
+class NRContributorTypeVocabularyUISchema(DictOnlySchema):
     class Meta:
         unknown = ma.INCLUDE
 
     _id = String(data_key="id", attribute="id")
 
     _version = String(data_key="@v", attribute="@v")
 
@@ -173,23 +243,14 @@
     _id = String(data_key="id", attribute="id")
 
     _version = String(data_key="@v", attribute="@v")
 
     title = VocabularyI18nStrUIField()
 
 
-class NRExternalLocationUISchema(DictOnlySchema):
-    class Meta:
-        unknown = ma.RAISE
-
-    externalLocationNote = ma_fields.String()
-
-    externalLocationURL = ma_fields.String(required=True)
-
-
 class NRFunderVocabularyUISchema(DictOnlySchema):
     class Meta:
         unknown = ma.INCLUDE
 
     _id = String(data_key="id", attribute="id")
 
     _version = String(data_key="@v", attribute="@v")
@@ -224,26 +285,39 @@
     _id = String(data_key="id", attribute="id")
 
     _version = String(data_key="@v", attribute="@v")
 
     title = VocabularyI18nStrUIField()
 
 
-class NRLicenseVocabularyUISchema(DictOnlySchema):
+class NROrganizationUISchema(DictOnlySchema):
+    class Meta:
+        unknown = ma.RAISE
+
+    authorityIdentifiers = ma_fields.List(
+        ma_fields.Nested(lambda: NROrganizationIdentifierUISchema())
+    )
+
+    fullName = ma_fields.String(required=True)
+
+    nameType = ma_fields.String(validate=[OneOf(["Organizational"])])
+
+
+class NRResourceTypeVocabularyUISchema(DictOnlySchema):
     class Meta:
         unknown = ma.INCLUDE
 
     _id = String(data_key="id", attribute="id")
 
     _version = String(data_key="@v", attribute="@v")
 
     title = VocabularyI18nStrUIField()
 
 
-class NRResourceTypeVocabularyUISchema(DictOnlySchema):
+class NRRightsVocabularyUISchema(DictOnlySchema):
     class Meta:
         unknown = ma.INCLUDE
 
     _id = String(data_key="id", attribute="id")
 
     _version = String(data_key="@v", attribute="@v")
 
@@ -277,7 +351,16 @@
     classificationCode = ma_fields.String()
 
     subject = I18nStrUIField()
 
     subjectScheme = ma_fields.String()
 
     valueURI = ma_fields.String()
+
+
+class NRExternalLocationUISchema(DictOnlySchema):
+    class Meta:
+        unknown = ma.RAISE
+
+    externalLocationNote = ma_fields.String()
+
+    externalLocationURL = ma_fields.String(required=True)
```

### Comparing `nr-metadata-2.0.8/nr_metadata/common/views/records/api.py` & `nr-metadata-2.0.9/nr_metadata/common/views/records/api.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-2.0.8/nr_metadata/common/views/records/app.py` & `nr-metadata-2.0.9/nr_metadata/common/views/records/app.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-2.0.8/nr_metadata/documents/config.py` & `nr-metadata-2.0.9/nr_metadata/documents/config.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-2.0.8/nr_metadata/documents/ext.py` & `nr-metadata-2.0.9/nr_metadata/documents/ext.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 from functools import cached_property
 
 from nr_metadata.documents import config
 
 
 class DocumentsExt:
+
     def __init__(self, app=None):
 
         if app:
             self.init_app(app)
 
     def init_app(self, app):
         """Flask application initialization."""
```

### Comparing `nr-metadata-2.0.8/nr_metadata/documents/models/records.json` & `nr-metadata-2.0.9/nr_metadata/data/models/records.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9129095582301445%*

 * *Differences: {"'model'": "{'marshmallow': {'class': "*

 * *            "'nr_metadata.data.services.records.schema.NRDataRecordSchema', 'module': "*

 * *            "'nr_metadata.data.services.records.schema'}, 'ui': {'marshmallow': {'class': "*

 * *            "'nr_metadata.data.services.records.ui_schema.NRDataRecordUISchema', 'module': "*

 * *            "'nr_metadata.data.services.records.ui_schema'}, 'module': 'nr_metadata.data.models', "*

 * *            "'file': 'nr_metadata/data/models/ui.json', 'alias': 'data'}, 'module': {'qualified':  […]*

```diff
@@ -1,152 +1,157 @@
 {
     "model": {
         "api-blueprint": {
-            "alias": "documents",
+            "alias": "data",
             "extra_code": "",
-            "function": "nr_metadata.documents.views.records.api.create_api_blueprint",
+            "function": "nr_metadata.data.views.records.api.create_api_blueprint",
             "generate": true,
             "imports": [],
-            "module": "nr_metadata.documents.views.records.api"
+            "module": "nr_metadata.data.views.records.api"
         },
         "app-blueprint": {
-            "alias": "documents",
+            "alias": "data",
             "extra_code": "",
-            "function": "nr_metadata.documents.views.records.app.create_app_blueprint",
+            "function": "nr_metadata.data.views.records.app.create_app_blueprint",
             "generate": true,
             "imports": [],
-            "module": "nr_metadata.documents.views.records.app"
+            "module": "nr_metadata.data.views.records.app"
         },
         "config": {
             "extra_code": "",
             "generate": true,
             "imports": [],
-            "module": "nr_metadata.documents.config"
+            "module": "nr_metadata.data.config"
         },
         "edtf-interval-dumper": {
             "base-classes": [
                 "oarepo_runtime.records.dumpers.edtf_interval.EDTFIntervalDumperExt"
             ],
-            "class": "nr_metadata.documents.records.dumpers.edtf.DocumentsEDTFIntervalDumperExt",
+            "class": "nr_metadata.data.records.dumpers.edtf.DataEDTFIntervalDumperExt",
             "extensions": [],
             "extra-code": "",
             "generate": true,
             "imports": [],
-            "module": "nr_metadata.documents.records.dumpers.edtf"
+            "module": "nr_metadata.data.records.dumpers.edtf"
         },
         "ext": {
-            "alias": "nr_metadata.documents",
+            "alias": "nr_metadata.data",
             "base-classes": [],
-            "class": "nr_metadata.documents.ext.DocumentsExt",
+            "class": "nr_metadata.data.ext.DataExt",
             "extra_code": "",
             "generate": true,
             "imports": [],
-            "module": "nr_metadata.documents.ext"
+            "module": "nr_metadata.data.ext"
         },
         "ext-resource": {
             "generate": true,
             "skip": false
         },
         "facets": {
             "extra-code": "",
             "generate": true,
-            "module": "nr_metadata.documents.services.records.facets"
+            "groups": true,
+            "module": "nr_metadata.data.services.records.facets"
         },
         "json-schema-settings": {
-            "alias": "documents",
-            "file": "nr_metadata/documents/records/jsonschemas/documents-1.0.0.json",
+            "alias": "data",
+            "file": "nr_metadata/data/records/jsonschemas/data-1.0.0.json",
             "generate": true,
-            "module": "nr_metadata.documents.records.jsonschemas",
-            "name": "documents-1.0.0.json",
+            "module": "nr_metadata.data.records.jsonschemas",
+            "name": "data-1.0.0.json",
             "version": "1.0.0"
         },
         "json-serializer": {
             "base-classes": [
                 "oarepo_runtime.resources.LocalizedUIJSONSerializer"
             ],
-            "class": "nr_metadata.documents.resources.records.ui.DocumentsUIJSONSerializer",
+            "class": "nr_metadata.data.resources.records.ui.DataUIJSONSerializer",
             "extra-code": "",
             "format_serializer_cls": "flask_resources.serializers.JSONSerializer",
             "generate": true,
             "imports": [],
             "list_schema_cls": "flask_resources.BaseListSchema",
-            "module": "nr_metadata.documents.resources.records.ui"
+            "module": "nr_metadata.data.resources.records.ui",
+            "schema-context-args": {
+                "\"identity\"": "{{ flask.g{g.identity} }}",
+                "\"object_key\"": "\"ui\""
+            }
         },
         "mapping": {
-            "alias": "documents",
-            "file": "nr_metadata/documents/records/mappings/os-v2/documents/documents-1.0.0.json",
+            "alias": "data",
+            "file": "nr_metadata/data/records/mappings/os-v2/data/data-1.0.0.json",
             "generate": true,
-            "index": "documents-documents-1.0.0",
-            "module": "nr_metadata.documents.records.mappings"
+            "index": "data-data-1.0.0",
+            "module": "nr_metadata.data.records.mappings"
         },
         "marshmallow": {
             "base-classes": [
                 "oarepo_runtime.services.schema.marshmallow.BaseRecordSchema"
             ],
-            "class": "nr_metadata.documents.services.records.schema.NRDocumentRecordSchema",
+            "class": "nr_metadata.data.services.records.schema.NRDataRecordSchema",
             "extra-code": "",
             "generate": true,
             "imports": [],
-            "module": "nr_metadata.documents.services.records.schema"
+            "module": "nr_metadata.data.services.records.schema"
         },
-        "model-name": "Documents",
+        "model-name": "Data",
         "module": {
-            "alias": "documents",
-            "base": "documents",
-            "base-title": "Documents",
-            "base-upper": "DOCUMENTS",
-            "kebab-module": "nr-metadata-documents",
-            "path": "nr_metadata/documents",
-            "prefix": "Documents",
-            "prefix-snake": "documents",
-            "prefix-upper": "DOCUMENTS",
-            "qualified": "nr_metadata.documents",
-            "suffix": "documents",
-            "suffix-snake": "documents",
-            "suffix-upper": "DOCUMENTS"
+            "alias": "data",
+            "base": "data",
+            "base-title": "Data",
+            "base-upper": "DATA",
+            "kebab-module": "nr-metadata-data",
+            "path": "nr_metadata/data",
+            "prefix": "Data",
+            "prefix-snake": "data",
+            "prefix-upper": "DATA",
+            "qualified": "nr_metadata.data",
+            "suffix": "data",
+            "suffix-snake": "data",
+            "suffix-upper": "DATA"
         },
         "multilingual-dumper": {
             "base-classes": [
                 "oarepo_runtime.records.dumpers.multilingual_dumper.MultilingualDumper"
             ],
-            "class": "nr_metadata.documents.records.dumpers.multilingual.MultilingualSearchDumperExt",
+            "class": "nr_metadata.data.records.dumpers.multilingual.MultilingualSearchDumperExt",
             "extensions": [],
             "extra-code": "",
             "generate": true,
             "imports": [],
-            "module": "nr_metadata.documents.records.dumpers.multilingual"
+            "module": "nr_metadata.data.records.dumpers.multilingual"
         },
         "permissions": {
             "base-classes": [
                 "invenio_records_permissions.RecordPermissionPolicy"
             ],
-            "class": "nr_metadata.documents.services.records.permissions.DocumentsPermissionPolicy",
+            "class": "nr_metadata.data.services.records.permissions.DataPermissionPolicy",
             "extra-code": "",
             "generate": true,
             "imports": [],
-            "module": "nr_metadata.documents.services.records.permissions",
+            "module": "nr_metadata.data.services.records.permissions",
             "presets": [
                 "everyone"
             ]
         },
         "pid": {
             "context-class": "invenio_records_resources.records.systemfields.pid.PIDFieldContext",
             "extra-code": "",
             "field-args": [
                 "create=True"
             ],
             "field-class": "invenio_records_resources.records.systemfields.pid.PIDField",
             "generate": true,
             "imports": [],
-            "module": "nr_metadata.documents.records.api",
+            "module": "nr_metadata.data.records.api",
             "provider-base-classes": [
                 "invenio_pidstore.providers.recordid_v2.RecordIdProviderV2"
             ],
-            "provider-class": "nr_metadata.documents.records.api.DocumentsIdProvider",
-            "type": "dcmnts"
+            "provider-class": "nr_metadata.data.records.api.DataIdProvider",
+            "type": "data"
         },
         "properties": {
             "$schema": {
                 "facets": {
                     "facet": false,
                     "searchable": true
                 },
@@ -206,24 +211,18 @@
                 }
             },
             "metadata": {
                 "marshmallow": {
                     "base-classes": [
                         "nr_metadata.common.services.records.schema_common.NRCommonMetadataSchema"
                     ],
-                    "class": "nr_metadata.documents.services.records.schema.NRDocumentMetadataSchema",
+                    "class": "nr_metadata.data.services.records.schema.NRDataMetadataSchema",
                     "extra-code": "",
                     "generate": true,
-                    "imports": [
-                        {
-                            "alias": "nr_metadata.common.services.records.schema_common",
-                            "import": "nr_metadata.common.services.records.schema_common"
-                        }
-                    ],
-                    "module": "nr_metadata.documents.services.records.schema"
+                    "module": "nr_metadata.data.services.records.schema"
                 },
                 "properties": {
                     "abstract": {
                         "items": {
                             "marshmallow": {
                                 "class": null,
                                 "field-class": "oarepo_runtime.services.schema.i18n.I18nStrField",
@@ -255,14 +254,15 @@
                         "label.cs": "Abstrakt",
                         "label.en": "Abstract",
                         "marshmallow": {
                             "field-class": "oarepo_runtime.services.schema.i18n.MultilingualField",
                             "read": false,
                             "write": false
                         },
+                        "required": true,
                         "type": "array",
                         "ui": {
                             "detail": "multilingual",
                             "marshmallow": {
                                 "field-class": "oarepo_runtime.services.schema.i18n_ui.MultilingualUIField",
                                 "read": false,
                                 "write": false
@@ -283,25 +283,16 @@
                         "keys": [
                             "id",
                             "title"
                         ],
                         "label.cs": "P\u0159\u00edstupov\u00e1 pr\u00e1va",
                         "label.en": "Access rights",
                         "marshmallow": {
-                            "base-classes": [
-                                "nr_metadata.common.services.records.schema_datatypes.NRAccessRightsVocabularySchema"
-                            ],
-                            "class": "nr_metadata.documents.services.records.schema.AccessRightsSchema",
+                            "class": "nr_metadata.common.services.records.schema_datatypes.NRAccessRightsVocabularySchema",
                             "generate": true,
-                            "imports": [
-                                {
-                                    "alias": "nr_metadata.common.services.records.schema_datatypes",
-                                    "import": "nr_metadata.common.services.records.schema_datatypes"
-                                }
-                            ],
                             "read": false,
                             "unknown": "INCLUDE",
                             "write": false
                         },
                         "model": "vocabularies",
                         "pid-field": "Vocabulary.pid.with_type_ctx(\"access-rights\")",
                         "properties": {
@@ -385,25 +376,16 @@
                             "metadata only"
                         ],
                         "type": "vocabulary",
                         "ui": {
                             "detail": "vocabulary_item",
                             "edit": "vocabulary_item",
                             "marshmallow": {
-                                "base-classes": [
-                                    "nr_metadata.common.services.records.ui_schema_datatypes.NRAccessRightsVocabularyUISchema"
-                                ],
-                                "class": "nr_metadata.documents.services.records.ui_schema.AccessRightsUISchema",
+                                "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRAccessRightsVocabularyUISchema",
                                 "generate": true,
-                                "imports": [
-                                    {
-                                        "alias": "nr_metadata.common.services.records.ui_schema_datatypes",
-                                        "import": "nr_metadata.common.services.records.ui_schema_datatypes"
-                                    }
-                                ],
                                 "read": false,
                                 "unknown": "INCLUDE",
                                 "write": false
                             }
                         },
                         "vocabulary-type": "access-rights"
                     },
@@ -453,25 +435,16 @@
                                 "write": false
                             }
                         }
                     },
                     "additionalTitles": {
                         "items": {
                             "marshmallow": {
-                                "base-classes": [
-                                    "nr_metadata.common.services.records.schema_common.AdditionalTitlesSchema"
-                                ],
-                                "class": "nr_metadata.documents.services.records.schema.AdditionalTitlesItemSchema",
-                                "generate": true,
-                                "imports": [
-                                    {
-                                        "alias": "nr_metadata.common.services.records.schema_common",
-                                        "import": "nr_metadata.common.services.records.schema_common"
-                                    }
-                                ]
+                                "class": "nr_metadata.common.services.records.schema_common.AdditionalTitlesSchema",
+                                "generate": false
                             },
                             "properties": {
                                 "title": {
                                     "marshmallow": {
                                         "class": null,
                                         "field-class": "oarepo_runtime.services.schema.i18n.I18nStrField",
                                         "generate": false,
@@ -527,51 +500,33 @@
                                     }
                                 }
                             },
                             "type": "object",
                             "ui": {
                                 "detail": "additionalTitle",
                                 "marshmallow": {
-                                    "base-classes": [
-                                        "nr_metadata.common.services.records.ui_schema_common.AdditionalTitlesUISchema"
-                                    ],
-                                    "class": "nr_metadata.documents.services.records.ui_schema.AdditionalTitlesItemUISchema",
-                                    "generate": true,
-                                    "imports": [
-                                        {
-                                            "alias": "nr_metadata.common.services.records.ui_schema_common",
-                                            "import": "nr_metadata.common.services.records.ui_schema_common"
-                                        }
-                                    ]
+                                    "class": "nr_metadata.common.services.records.ui_schema_common.AdditionalTitlesUISchema",
+                                    "generate": false
                                 }
                             }
                         },
                         "label.cs": "Dal\u0161\u00ed n\u00e1zvy",
                         "label.en": "Additional titles",
                         "type": "array"
                     },
-                    "collection": {
-                        "label.cs": "Kolekce",
-                        "label.en": "Collection",
-                        "type": "keyword"
-                    },
                     "contributors": {
                         "items": {
+                            "discriminator": "nameType",
+                            "hint.cs": "Jako tv\u016frce je mo\u017en\u00e9 ozna\u010dit osobu nebo instituci.",
+                            "hint.en": "It is possible to designate a person or an institution as the creator/contributor.",
                             "marshmallow": {
-                                "base-classes": [
-                                    "nr_metadata.common.services.records.schema_common.NRContributorSchema"
-                                ],
-                                "class": "nr_metadata.documents.services.records.schema.ContributorsItemSchema",
+                                "class": "nr_metadata.common.services.records.schema_common.NRContributorSchema",
                                 "generate": true,
-                                "imports": [
-                                    {
-                                        "alias": "nr_metadata.common.services.records.schema_common",
-                                        "import": "nr_metadata.common.services.records.schema_common"
-                                    }
-                                ]
+                                "read": false,
+                                "write": false
                             },
                             "properties": {
                                 "affiliations": {
                                     "items": {
                                         "facets": {
                                             "args": [
                                                 "vocabulary='institutions'"
@@ -583,14 +538,21 @@
                                                 "import": "invenio_vocabularies.records.api.Vocabulary"
                                             }
                                         ],
                                         "keys": [
                                             "id",
                                             "title",
                                             {
+                                                "key": "props.ror",
+                                                "model": {
+                                                    "type": "keyword"
+                                                },
+                                                "target": "ror"
+                                            },
+                                            {
                                                 "key": "hierarchy",
                                                 "model": {
                                                     "marshmallow": {
                                                         "class": "oarepo_vocabularies.services.schema.HierarchySchema",
                                                         "generate": false,
                                                         "imports": [
                                                             {
@@ -622,25 +584,25 @@
                                                                 "additionalProperties": {
                                                                     "type": "string"
                                                                 },
                                                                 "mapping": {
                                                                     "dynamic": true
                                                                 },
                                                                 "marshmallow": {
-                                                                    "class": "nr_metadata.documents.services.records.schema.TitleItemSchema",
+                                                                    "class": "nr_metadata.data.services.records.schema.TitleItemSchema",
                                                                     "field": "i18n_strings",
                                                                     "generate": true
                                                                 },
                                                                 "propertyNames": {
                                                                     "pattern": "^[a-z]{2}$"
                                                                 },
                                                                 "type": "object",
                                                                 "ui": {
                                                                     "marshmallow": {
-                                                                        "class": "nr_metadata.documents.services.records.ui_schema.TitleItemUISchema",
+                                                                        "class": "nr_metadata.data.services.records.ui_schema.TitleItemUISchema",
                                                                         "field": "i18n_strings",
                                                                         "generate": true
                                                                     }
                                                                 }
                                                             },
                                                             "type": "array"
                                                         }
@@ -660,25 +622,16 @@
                                                 },
                                                 "target": "hierarchy"
                                             }
                                         ],
                                         "label.cs": "Afiliace",
                                         "label.en": "Affiliation",
                                         "marshmallow": {
-                                            "base-classes": [
-                                                "nr_metadata.common.services.records.schema_datatypes.NRAffiliationVocabularySchema"
-                                            ],
-                                            "class": "nr_metadata.documents.services.records.schema.AffiliationsItemSchema",
+                                            "class": "nr_metadata.common.services.records.schema_datatypes.NRAffiliationVocabularySchema",
                                             "generate": true,
-                                            "imports": [
-                                                {
-                                                    "alias": "nr_metadata.common.services.records.schema_datatypes",
-                                                    "import": "nr_metadata.common.services.records.schema_datatypes"
-                                                }
-                                            ],
                                             "read": false,
                                             "unknown": "INCLUDE",
                                             "write": false
                                         },
                                         "model": "vocabularies",
                                         "pid-field": "Vocabulary.pid.with_type_ctx(\"institutions\")",
                                         "properties": {
@@ -732,25 +685,25 @@
                                                             "additionalProperties": {
                                                                 "type": "string"
                                                             },
                                                             "mapping": {
                                                                 "dynamic": true
                                                             },
                                                             "marshmallow": {
-                                                                "class": "nr_metadata.documents.services.records.schema.TitleItemSchema",
+                                                                "class": "nr_metadata.data.services.records.schema.TitleItemSchema",
                                                                 "field": "i18n_strings",
                                                                 "generate": true
                                                             },
                                                             "propertyNames": {
                                                                 "pattern": "^[a-z]{2}$"
                                                             },
                                                             "type": "object",
                                                             "ui": {
                                                                 "marshmallow": {
-                                                                    "class": "nr_metadata.documents.services.records.ui_schema.TitleItemUISchema",
+                                                                    "class": "nr_metadata.data.services.records.ui_schema.TitleItemUISchema",
                                                                     "field": "i18n_strings",
                                                                     "generate": true
                                                                 }
                                                             }
                                                         },
                                                         "type": "array"
                                                     }
@@ -789,14 +742,17 @@
                                                     "marshmallow": {
                                                         "field-class": "marshmallow.fields.String",
                                                         "imports": [],
                                                         "validators": []
                                                     }
                                                 }
                                             },
+                                            "ror": {
+                                                "type": "keyword"
+                                            },
                                             "title": {
                                                 "additionalProperties": {
                                                     "type": "string"
                                                 },
                                                 "mapping": {
                                                     "dynamic": true,
                                                     "properties": {
@@ -829,50 +785,30 @@
                                             "faker": "company"
                                         },
                                         "type": "taxonomy",
                                         "ui": {
                                             "detail": "taxonomy_item",
                                             "edit": "taxonomy_item",
                                             "marshmallow": {
-                                                "base-classes": [
-                                                    "nr_metadata.common.services.records.ui_schema_datatypes.NRAffiliationVocabularyUISchema"
-                                                ],
-                                                "class": "nr_metadata.documents.services.records.ui_schema.AffiliationsItemUISchema",
+                                                "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRAffiliationVocabularyUISchema",
                                                 "generate": true,
-                                                "imports": [
-                                                    {
-                                                        "alias": "nr_metadata.common.services.records.ui_schema_datatypes",
-                                                        "import": "nr_metadata.common.services.records.ui_schema_datatypes"
-                                                    }
-                                                ],
                                                 "read": false,
                                                 "unknown": "INCLUDE",
                                                 "write": false
                                             }
                                         },
                                         "vocabulary-type": "institutions"
                                     },
                                     "type": "array"
                                 },
                                 "authorityIdentifiers": {
                                     "items": {
                                         "marshmallow": {
-                                            "base-classes": [
-                                                "nr_metadata.schema.identifiers.NRAuthorityIdentifierSchema"
-                                            ],
-                                            "class": "nr_metadata.documents.services.records.schema.AuthorityIdentifiersItemSchema",
-                                            "generate": true,
-                                            "imports": [
-                                                {
-                                                    "alias": "nr_metadata.schema.identifiers",
-                                                    "import": "nr_metadata.schema.identifiers"
-                                                }
-                                            ],
-                                            "read": false,
-                                            "write": false
+                                            "class": "nr_metadata.schema.identifiers.NROrganizationIdentifierSchema",
+                                            "generate": false
                                         },
                                         "properties": {
                                             "identifier": {
                                                 "i18n.key": "identifier",
                                                 "label.cs": "Identifik\u00e1tor",
                                                 "label.en": "Identifier",
                                                 "marshmallow": {
@@ -889,20 +825,14 @@
                                                         "read": false,
                                                         "write": false
                                                     }
                                                 }
                                             },
                                             "scheme": {
                                                 "enum": [
-                                                    "orcid",
-                                                    "scopusID",
-                                                    "researcherID",
-                                                    "czenasAutID",
-                                                    "vedidk",
-                                                    "institutionalID",
                                                     "ISNI",
                                                     "ROR",
                                                     "ICO",
                                                     "DOI"
                                                 ],
                                                 "hint.cs": "Doporu\u010dujeme zadat alespo\u0148 jeden z typ\u016f identifik\u00e1tor\u016f.\nPokud pot\u0159ebujete roz\u0161\u00ed\u0159it nab\u00eddku typ\u016f identifik\u00e1tor\u016f, kontaktujte n\u00e1s na support@narodni-repozitar.cz.\n",
                                                 "hint.en": "We recommend providing at least one of the identifier types.\nIf you need to expand the range of identifier types, contact us at support@narodni-repozitar.cz.\n",
@@ -921,113 +851,49 @@
                                                         "write": false
                                                     }
                                                 }
                                             }
                                         },
                                         "type": "object",
                                         "ui": {
-                                            "detail": "nr_authority_identifier",
+                                            "detail": "nr_organization_identifier",
                                             "marshmallow": {
-                                                "base-classes": [
-                                                    "nr_metadata.ui_schema.identifiers.NRAuthorityIdentifierUISchema"
-                                                ],
-                                                "class": "nr_metadata.documents.services.records.ui_schema.AuthorityIdentifiersItemUISchema",
-                                                "generate": true,
-                                                "imports": [
-                                                    {
-                                                        "alias": "nr_metadata.ui_schema.identifiers",
-                                                        "import": "nr_metadata.ui_schema.identifiers"
-                                                    }
-                                                ],
-                                                "read": false,
-                                                "write": false
+                                                "class": "nr_metadata.ui_schema.identifiers.NROrganizationIdentifierUISchema",
+                                                "generate": false
                                             }
                                         }
                                     },
                                     "type": "array"
                                 },
-                                "fullName": {
-                                    "label.cs": "Jm\u00e9no p\u0159isp\u011bvatele",
-                                    "label.en": "Contributor name",
-                                    "marshmallow": {
-                                        "read": false,
-                                        "write": false
-                                    },
-                                    "required": true,
-                                    "sample": {
-                                        "faker": "name"
-                                    },
-                                    "type": "keyword",
-                                    "ui": {
-                                        "marshmallow": {
-                                            "read": false,
-                                            "write": false
-                                        }
-                                    }
-                                },
-                                "nameType": {
-                                    "enum": [
-                                        "Organizational",
-                                        "Personal"
-                                    ],
-                                    "hint.cs": "Jako tv\u016frce je mo\u017en\u00e9 ozna\u010dit osobu nebo instituci.",
-                                    "hint.en": "It is possible to designate a person or an institution as the creator/contributor.",
-                                    "label.cs": "Typ",
-                                    "label.en": "Type",
-                                    "marshmallow": {
-                                        "read": false,
-                                        "write": false
-                                    },
-                                    "sample": [
-                                        "Organizational",
-                                        "Personal"
-                                    ],
-                                    "type": "keyword",
-                                    "ui": {
-                                        "marshmallow": {
-                                            "read": false,
-                                            "write": false
-                                        }
-                                    }
-                                },
-                                "role": {
+                                "contributorType": {
                                     "facets": {
                                         "args": [
-                                            "vocabulary='contributor-roles'"
+                                            "vocabulary='contributor-types'"
                                         ]
                                     },
                                     "imports": [
                                         {
                                             "import": "invenio_vocabularies.records.api.Vocabulary"
                                         }
                                     ],
                                     "keys": [
                                         "id",
                                         "title"
                                     ],
-                                    "label.cs": "Role p\u0159isp\u011bvatele",
-                                    "label.en": "Contributor's role",
+                                    "label.cs": "Typ p\u0159isp\u011bvatele",
+                                    "label.en": "Contributor's type",
                                     "marshmallow": {
-                                        "base-classes": [
-                                            "nr_metadata.common.services.records.schema_datatypes.NRAuthorityRoleVocabularySchema"
-                                        ],
-                                        "class": "nr_metadata.documents.services.records.schema.RoleSchema",
-                                        "generate": true,
-                                        "imports": [
-                                            {
-                                                "alias": "nr_metadata.common.services.records.schema_datatypes",
-                                                "import": "nr_metadata.common.services.records.schema_datatypes"
-                                            }
-                                        ],
+                                        "class": "nr_metadata.common.services.records.schema_datatypes.NRContributorTypeVocabularySchema",
+                                        "generate": false,
                                         "read": false,
                                         "unknown": "INCLUDE",
                                         "write": false
                                     },
                                     "model": "vocabularies",
-                                    "pid-field": "Vocabulary.pid.with_type_ctx(\"contributor-roles\")",
+                                    "pid-field": "Vocabulary.pid.with_type_ctx(\"contributor-types\")",
                                     "properties": {
                                         "@v": {
                                             "facets": {
                                                 "facet": false
                                             },
                                             "marshmallow": {
                                                 "field-class": "marshmallow.fields.String",
@@ -1099,69 +965,606 @@
                                         }
                                     },
                                     "type": "vocabulary",
                                     "ui": {
                                         "detail": "vocabulary_item",
                                         "edit": "vocabulary_item",
                                         "marshmallow": {
+                                            "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRContributorTypeVocabularyUISchema",
+                                            "generate": false,
+                                            "read": false,
+                                            "unknown": "INCLUDE",
+                                            "write": false
+                                        }
+                                    },
+                                    "vocabulary-type": "contributor-types"
+                                },
+                                "familyName": {
+                                    "marshmallow": {
+                                        "read": false,
+                                        "write": false
+                                    },
+                                    "type": "keyword",
+                                    "ui": {
+                                        "marshmallow": {
+                                            "read": false,
+                                            "write": false
+                                        }
+                                    }
+                                },
+                                "fullName": {
+                                    "label.cs": "Jm\u00e9no p\u0159isp\u011bvatele",
+                                    "label.en": "Contributor name",
+                                    "marshmallow": {
+                                        "read": false,
+                                        "write": false
+                                    },
+                                    "required": true,
+                                    "sample": {
+                                        "faker": "name"
+                                    },
+                                    "type": "keyword",
+                                    "ui": {
+                                        "marshmallow": {
+                                            "read": false,
+                                            "write": false
+                                        }
+                                    }
+                                },
+                                "givenName": {
+                                    "marshmallow": {
+                                        "read": false,
+                                        "write": false
+                                    },
+                                    "type": "keyword",
+                                    "ui": {
+                                        "marshmallow": {
+                                            "read": false,
+                                            "write": false
+                                        }
+                                    }
+                                },
+                                "nameType": {
+                                    "enum": [
+                                        "Organizational"
+                                    ],
+                                    "label.cs": "Typ",
+                                    "label.en": "Type",
+                                    "marshmallow": {
+                                        "read": false,
+                                        "write": false
+                                    },
+                                    "sample": [
+                                        "Organizational"
+                                    ],
+                                    "type": "keyword",
+                                    "ui": {
+                                        "marshmallow": {
+                                            "read": false,
+                                            "write": false
+                                        }
+                                    }
+                                }
+                            },
+                            "schemas": {
+                                "Organizational": {
+                                    "marshmallow": {
+                                        "base-classes": [
+                                            "nr_metadata.common.services.records.schema_datatypes.NROrganizationSchema"
+                                        ],
+                                        "class": "nr_metadata.common.services.records.schema_common.NRContributorOrganizationSchema",
+                                        "generate": true
+                                    },
+                                    "properties": {
+                                        "authorityIdentifiers": {
+                                            "items": {
+                                                "marshmallow": {
+                                                    "class": "nr_metadata.schema.identifiers.NROrganizationIdentifierSchema",
+                                                    "generate": false
+                                                },
+                                                "properties": {
+                                                    "identifier": {
+                                                        "i18n.key": "identifier",
+                                                        "label.cs": "Identifik\u00e1tor",
+                                                        "label.en": "Identifier",
+                                                        "marshmallow": {
+                                                            "read": false,
+                                                            "write": false
+                                                        },
+                                                        "required": true,
+                                                        "sample": {
+                                                            "faker": "isbn13"
+                                                        },
+                                                        "type": "keyword",
+                                                        "ui": {
+                                                            "marshmallow": {
+                                                                "read": false,
+                                                                "write": false
+                                                            }
+                                                        }
+                                                    },
+                                                    "scheme": {
+                                                        "enum": [
+                                                            "ISNI",
+                                                            "ROR",
+                                                            "ICO",
+                                                            "DOI"
+                                                        ],
+                                                        "hint.cs": "Doporu\u010dujeme zadat alespo\u0148 jeden z typ\u016f identifik\u00e1tor\u016f.\nPokud pot\u0159ebujete roz\u0161\u00ed\u0159it nab\u00eddku typ\u016f identifik\u00e1tor\u016f, kontaktujte n\u00e1s na support@narodni-repozitar.cz.\n",
+                                                        "hint.en": "We recommend providing at least one of the identifier types.\nIf you need to expand the range of identifier types, contact us at support@narodni-repozitar.cz.\n",
+                                                        "i18n.key": "identifier_type",
+                                                        "label.cs": "Typ identifik\u00e1toru",
+                                                        "label.en": "Identifier type",
+                                                        "marshmallow": {
+                                                            "read": false,
+                                                            "write": false
+                                                        },
+                                                        "required": true,
+                                                        "type": "keyword",
+                                                        "ui": {
+                                                            "marshmallow": {
+                                                                "read": false,
+                                                                "write": false
+                                                            }
+                                                        }
+                                                    }
+                                                },
+                                                "type": "object",
+                                                "ui": {
+                                                    "detail": "nr_organization_identifier",
+                                                    "marshmallow": {
+                                                        "class": "nr_metadata.ui_schema.identifiers.NROrganizationIdentifierUISchema",
+                                                        "generate": false
+                                                    }
+                                                }
+                                            },
+                                            "type": "array"
+                                        },
+                                        "contributorType": {
+                                            "facets": {
+                                                "args": [
+                                                    "vocabulary='contributor-types'"
+                                                ]
+                                            },
+                                            "imports": [
+                                                {
+                                                    "import": "invenio_vocabularies.records.api.Vocabulary"
+                                                }
+                                            ],
+                                            "keys": [
+                                                "id",
+                                                "title"
+                                            ],
+                                            "label.cs": "Typ p\u0159isp\u011bvatele",
+                                            "label.en": "Contributor's type",
+                                            "marshmallow": {
+                                                "class": "nr_metadata.common.services.records.schema_datatypes.NRContributorTypeVocabularySchema",
+                                                "generate": false,
+                                                "read": false,
+                                                "unknown": "INCLUDE",
+                                                "write": false
+                                            },
+                                            "model": "vocabularies",
+                                            "pid-field": "Vocabulary.pid.with_type_ctx(\"contributor-types\")",
+                                            "properties": {},
+                                            "type": "vocabulary",
+                                            "ui": {
+                                                "detail": "vocabulary_item",
+                                                "edit": "vocabulary_item",
+                                                "marshmallow": {
+                                                    "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRContributorTypeVocabularyUISchema",
+                                                    "generate": false,
+                                                    "read": false,
+                                                    "unknown": "INCLUDE",
+                                                    "write": false
+                                                }
+                                            },
+                                            "vocabulary-type": "contributor-types"
+                                        },
+                                        "fullName": {
+                                            "label.cs": "Jm\u00e9no p\u0159isp\u011bvatele",
+                                            "label.en": "Contributor name",
+                                            "marshmallow": {
+                                                "read": false,
+                                                "write": false
+                                            },
+                                            "required": true,
+                                            "sample": {
+                                                "faker": "name"
+                                            },
+                                            "type": "keyword",
+                                            "ui": {
+                                                "marshmallow": {
+                                                    "read": false,
+                                                    "write": false
+                                                }
+                                            }
+                                        },
+                                        "nameType": {
+                                            "enum": [
+                                                "Organizational"
+                                            ],
+                                            "label.cs": "Typ",
+                                            "label.en": "Type",
+                                            "marshmallow": {
+                                                "read": false,
+                                                "write": false
+                                            },
+                                            "sample": [
+                                                "Organizational"
+                                            ],
+                                            "type": "keyword",
+                                            "ui": {
+                                                "marshmallow": {
+                                                    "read": false,
+                                                    "write": false
+                                                }
+                                            }
+                                        }
+                                    },
+                                    "type": "object",
+                                    "ui": {
+                                        "detail": "nr_contributor_organization",
+                                        "marshmallow": {
                                             "base-classes": [
-                                                "nr_metadata.common.services.records.ui_schema_datatypes.NRAuthorityRoleVocabularyUISchema"
+                                                "nr_metadata.common.services.records.ui_schema_datatypes.NROrganizationUISchema"
                                             ],
-                                            "class": "nr_metadata.documents.services.records.ui_schema.RoleUISchema",
-                                            "generate": true,
+                                            "class": "nr_metadata.common.services.records.ui_schema_common.NRContributorOrganizationUISchema",
+                                            "generate": true
+                                        }
+                                    }
+                                },
+                                "Personal": {
+                                    "marshmallow": {
+                                        "base-classes": [
+                                            "nr_metadata.common.services.records.schema_datatypes.NRPersonSchema"
+                                        ],
+                                        "class": "nr_metadata.common.services.records.schema_common.NRContributorPersonSchema",
+                                        "generate": true
+                                    },
+                                    "properties": {
+                                        "affiliations": {
+                                            "items": {
+                                                "facets": {
+                                                    "args": [
+                                                        "vocabulary='institutions'"
+                                                    ]
+                                                },
+                                                "hint.cs": "Uve\u010fte instituci/instituce, pod jej\u00ed\u017e z\u00e1\u0161titou jste se na tvorb\u011b objektu pod\u00edleli.",
+                                                "imports": [
+                                                    {
+                                                        "import": "invenio_vocabularies.records.api.Vocabulary"
+                                                    }
+                                                ],
+                                                "keys": [
+                                                    "id",
+                                                    "title",
+                                                    {
+                                                        "key": "props.ror",
+                                                        "model": {
+                                                            "type": "keyword"
+                                                        },
+                                                        "target": "ror"
+                                                    },
+                                                    {
+                                                        "key": "hierarchy",
+                                                        "model": {
+                                                            "marshmallow": {
+                                                                "class": "oarepo_vocabularies.services.schema.HierarchySchema",
+                                                                "generate": false,
+                                                                "imports": [
+                                                                    {
+                                                                        "import": "oarepo_vocabularies.services.schema.HierarchySchema"
+                                                                    }
+                                                                ]
+                                                            },
+                                                            "properties": {
+                                                                "ancestors": {
+                                                                    "items": {
+                                                                        "type": "keyword"
+                                                                    },
+                                                                    "type": "array"
+                                                                },
+                                                                "ancestors_or_self": {
+                                                                    "items": {
+                                                                        "type": "keyword"
+                                                                    },
+                                                                    "type": "array"
+                                                                },
+                                                                "level": {
+                                                                    "type": "integer"
+                                                                },
+                                                                "parent": {
+                                                                    "type": "keyword"
+                                                                },
+                                                                "title": {
+                                                                    "items": {
+                                                                        "additionalProperties": {
+                                                                            "type": "string"
+                                                                        },
+                                                                        "mapping": {
+                                                                            "dynamic": true
+                                                                        },
+                                                                        "marshmallow": {
+                                                                            "class": "nr_metadata.data.services.records.schema.TitleItemSchema",
+                                                                            "field": "i18n_strings",
+                                                                            "generate": true
+                                                                        },
+                                                                        "propertyNames": {
+                                                                            "pattern": "^[a-z]{2}$"
+                                                                        },
+                                                                        "type": "object",
+                                                                        "ui": {
+                                                                            "marshmallow": {
+                                                                                "class": "nr_metadata.data.services.records.ui_schema.TitleItemUISchema",
+                                                                                "field": "i18n_strings",
+                                                                                "generate": true
+                                                                            }
+                                                                        }
+                                                                    },
+                                                                    "type": "array"
+                                                                }
+                                                            },
+                                                            "type": "object",
+                                                            "ui": {
+                                                                "marshmallow": {
+                                                                    "class": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema",
+                                                                    "generate": false,
+                                                                    "imports": [
+                                                                        {
+                                                                            "import": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema"
+                                                                        }
+                                                                    ]
+                                                                }
+                                                            }
+                                                        },
+                                                        "target": "hierarchy"
+                                                    }
+                                                ],
+                                                "label.cs": "Afiliace",
+                                                "label.en": "Affiliation",
+                                                "marshmallow": {
+                                                    "class": "nr_metadata.common.services.records.schema_datatypes.NRAffiliationVocabularySchema",
+                                                    "generate": true,
+                                                    "read": false,
+                                                    "unknown": "INCLUDE",
+                                                    "write": false
+                                                },
+                                                "model": "vocabularies",
+                                                "pid-field": "Vocabulary.pid.with_type_ctx(\"institutions\")",
+                                                "properties": {},
+                                                "sample": {
+                                                    "faker": "company"
+                                                },
+                                                "type": "taxonomy",
+                                                "ui": {
+                                                    "detail": "taxonomy_item",
+                                                    "edit": "taxonomy_item",
+                                                    "marshmallow": {
+                                                        "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRAffiliationVocabularyUISchema",
+                                                        "generate": true,
+                                                        "read": false,
+                                                        "unknown": "INCLUDE",
+                                                        "write": false
+                                                    }
+                                                },
+                                                "vocabulary-type": "institutions"
+                                            },
+                                            "type": "array"
+                                        },
+                                        "authorityIdentifiers": {
+                                            "items": {
+                                                "marshmallow": {
+                                                    "class": "nr_metadata.schema.identifiers.NRPersonIdentifierSchema",
+                                                    "generate": false
+                                                },
+                                                "properties": {
+                                                    "identifier": {
+                                                        "i18n.key": "identifier",
+                                                        "label.cs": "Identifik\u00e1tor",
+                                                        "label.en": "Identifier",
+                                                        "marshmallow": {
+                                                            "read": false,
+                                                            "write": false
+                                                        },
+                                                        "required": true,
+                                                        "sample": {
+                                                            "faker": "isbn13"
+                                                        },
+                                                        "type": "keyword",
+                                                        "ui": {
+                                                            "marshmallow": {
+                                                                "read": false,
+                                                                "write": false
+                                                            }
+                                                        }
+                                                    },
+                                                    "scheme": {
+                                                        "enum": [
+                                                            "orcid",
+                                                            "scopusID",
+                                                            "researcherID",
+                                                            "czenasAutID",
+                                                            "vedidk",
+                                                            "institutionalID",
+                                                            "ISNI"
+                                                        ],
+                                                        "hint.cs": "Doporu\u010dujeme zadat alespo\u0148 jeden z typ\u016f identifik\u00e1tor\u016f.\nPokud pot\u0159ebujete roz\u0161\u00ed\u0159it nab\u00eddku typ\u016f identifik\u00e1tor\u016f, kontaktujte n\u00e1s na support@narodni-repozitar.cz.\n",
+                                                        "hint.en": "We recommend providing at least one of the identifier types.\nIf you need to expand the range of identifier types, contact us at support@narodni-repozitar.cz.\n",
+                                                        "i18n.key": "identifier_type",
+                                                        "label.cs": "Typ identifik\u00e1toru",
+                                                        "label.en": "Identifier type",
+                                                        "marshmallow": {
+                                                            "read": false,
+                                                            "write": false
+                                                        },
+                                                        "required": true,
+                                                        "type": "keyword",
+                                                        "ui": {
+                                                            "marshmallow": {
+                                                                "read": false,
+                                                                "write": false
+                                                            }
+                                                        }
+                                                    }
+                                                },
+                                                "type": "object",
+                                                "ui": {
+                                                    "detail": "nr_person_identifier",
+                                                    "marshmallow": {
+                                                        "class": "nr_metadata.ui_schema.identifiers.NRPersonIdentifierUISchema",
+                                                        "generate": false
+                                                    }
+                                                }
+                                            },
+                                            "type": "array"
+                                        },
+                                        "contributorType": {
+                                            "facets": {
+                                                "args": [
+                                                    "vocabulary='contributor-types'"
+                                                ]
+                                            },
                                             "imports": [
                                                 {
-                                                    "alias": "nr_metadata.common.services.records.ui_schema_datatypes",
-                                                    "import": "nr_metadata.common.services.records.ui_schema_datatypes"
+                                                    "import": "invenio_vocabularies.records.api.Vocabulary"
                                                 }
                                             ],
-                                            "read": false,
-                                            "unknown": "INCLUDE",
-                                            "write": false
+                                            "keys": [
+                                                "id",
+                                                "title"
+                                            ],
+                                            "label.cs": "Typ p\u0159isp\u011bvatele",
+                                            "label.en": "Contributor's type",
+                                            "marshmallow": {
+                                                "class": "nr_metadata.common.services.records.schema_datatypes.NRContributorTypeVocabularySchema",
+                                                "generate": true,
+                                                "read": false,
+                                                "unknown": "INCLUDE",
+                                                "write": false
+                                            },
+                                            "model": "vocabularies",
+                                            "pid-field": "Vocabulary.pid.with_type_ctx(\"contributor-types\")",
+                                            "properties": {},
+                                            "type": "vocabulary",
+                                            "ui": {
+                                                "detail": "vocabulary_item",
+                                                "edit": "vocabulary_item",
+                                                "marshmallow": {
+                                                    "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRContributorTypeVocabularyUISchema",
+                                                    "generate": true,
+                                                    "read": false,
+                                                    "unknown": "INCLUDE",
+                                                    "write": false
+                                                }
+                                            },
+                                            "vocabulary-type": "contributor-types"
+                                        },
+                                        "familyName": {
+                                            "marshmallow": {
+                                                "read": false,
+                                                "write": false
+                                            },
+                                            "type": "keyword",
+                                            "ui": {
+                                                "marshmallow": {
+                                                    "read": false,
+                                                    "write": false
+                                                }
+                                            }
+                                        },
+                                        "fullName": {
+                                            "label.cs": "Jm\u00e9no p\u0159isp\u011bvatele",
+                                            "label.en": "Contributor name",
+                                            "marshmallow": {
+                                                "read": false,
+                                                "write": false
+                                            },
+                                            "required": true,
+                                            "sample": {
+                                                "faker": "name"
+                                            },
+                                            "type": "keyword",
+                                            "ui": {
+                                                "marshmallow": {
+                                                    "read": false,
+                                                    "write": false
+                                                }
+                                            }
+                                        },
+                                        "givenName": {
+                                            "marshmallow": {
+                                                "read": false,
+                                                "write": false
+                                            },
+                                            "type": "keyword",
+                                            "ui": {
+                                                "marshmallow": {
+                                                    "read": false,
+                                                    "write": false
+                                                }
+                                            }
+                                        },
+                                        "nameType": {
+                                            "enum": [
+                                                "Personal"
+                                            ],
+                                            "label.cs": "Typ",
+                                            "label.en": "Type",
+                                            "marshmallow": {
+                                                "read": false,
+                                                "write": false
+                                            },
+                                            "type": "keyword",
+                                            "ui": {
+                                                "marshmallow": {
+                                                    "read": false,
+                                                    "write": false
+                                                }
+                                            }
                                         }
                                     },
-                                    "vocabulary-type": "contributor-roles"
+                                    "type": "object",
+                                    "ui": {
+                                        "detail": "nr_contributor_person",
+                                        "marshmallow": {
+                                            "base-classes": [
+                                                "nr_metadata.common.services.records.ui_schema_datatypes.NRPersonUISchema"
+                                            ],
+                                            "class": "nr_metadata.common.services.records.ui_schema_common.NRContributorPersonUISchema",
+                                            "generate": true
+                                        }
+                                    }
                                 }
                             },
-                            "type": "object",
+                            "type": "polymorphic",
                             "ui": {
                                 "detail": "contributor",
                                 "marshmallow": {
-                                    "base-classes": [
-                                        "nr_metadata.common.services.records.ui_schema_common.NRContributorUISchema"
-                                    ],
-                                    "class": "nr_metadata.documents.services.records.ui_schema.ContributorsItemUISchema",
+                                    "class": "nr_metadata.common.services.records.ui_schema_common.NRContributorUISchema",
                                     "generate": true,
-                                    "imports": [
-                                        {
-                                            "alias": "nr_metadata.common.services.records.ui_schema_common",
-                                            "import": "nr_metadata.common.services.records.ui_schema_common"
-                                        }
-                                    ]
+                                    "read": false,
+                                    "write": false
                                 }
                             }
                         },
                         "label.cs": "P\u0159isp\u011bvatel\u00e9",
                         "label.en": "Contributors",
                         "type": "array"
                     },
                     "creators": {
                         "items": {
+                            "discriminator": "nameType",
+                            "hint.cs": "Jako tv\u016frce je mo\u017en\u00e9 ozna\u010dit osobu nebo instituci.",
+                            "hint.en": "It is possible to designate a person or an institution as the creator/contributor.",
                             "marshmallow": {
-                                "base-classes": [
-                                    "nr_metadata.common.services.records.schema_common.NRCreatorSchema"
-                                ],
-                                "class": "nr_metadata.documents.services.records.schema.CreatorsItemSchema",
+                                "class": "nr_metadata.common.services.records.schema_common.NRCreatorSchema",
                                 "generate": true,
-                                "imports": [
-                                    {
-                                        "alias": "nr_metadata.common.services.records.schema_common",
-                                        "import": "nr_metadata.common.services.records.schema_common"
-                                    }
-                                ]
+                                "read": false,
+                                "write": false
                             },
                             "properties": {
                                 "affiliations": {
                                     "items": {
                                         "facets": {
                                             "args": [
                                                 "vocabulary='institutions'"
@@ -1173,14 +1576,21 @@
                                                 "import": "invenio_vocabularies.records.api.Vocabulary"
                                             }
                                         ],
                                         "keys": [
                                             "id",
                                             "title",
                                             {
+                                                "key": "props.ror",
+                                                "model": {
+                                                    "type": "keyword"
+                                                },
+                                                "target": "ror"
+                                            },
+                                            {
                                                 "key": "hierarchy",
                                                 "model": {
                                                     "marshmallow": {
                                                         "class": "oarepo_vocabularies.services.schema.HierarchySchema",
                                                         "generate": false,
                                                         "imports": [
                                                             {
@@ -1212,25 +1622,25 @@
                                                                 "additionalProperties": {
                                                                     "type": "string"
                                                                 },
                                                                 "mapping": {
                                                                     "dynamic": true
                                                                 },
                                                                 "marshmallow": {
-                                                                    "class": "nr_metadata.documents.services.records.schema.TitleItemSchema",
+                                                                    "class": "nr_metadata.data.services.records.schema.TitleItemSchema",
                                                                     "field": "i18n_strings",
                                                                     "generate": false
                                                                 },
                                                                 "propertyNames": {
                                                                     "pattern": "^[a-z]{2}$"
                                                                 },
                                                                 "type": "object",
                                                                 "ui": {
                                                                     "marshmallow": {
-                                                                        "class": "nr_metadata.documents.services.records.ui_schema.TitleItemUISchema",
+                                                                        "class": "nr_metadata.data.services.records.ui_schema.TitleItemUISchema",
                                                                         "field": "i18n_strings",
                                                                         "generate": false
                                                                     }
                                                                 }
                                                             },
                                                             "type": "array"
                                                         }
@@ -1250,25 +1660,16 @@
                                                 },
                                                 "target": "hierarchy"
                                             }
                                         ],
                                         "label.cs": "Afiliace",
                                         "label.en": "Affiliation",
                                         "marshmallow": {
-                                            "base-classes": [
-                                                "nr_metadata.common.services.records.schema_datatypes.NRAffiliationVocabularySchema"
-                                            ],
-                                            "class": "nr_metadata.documents.services.records.schema.AffiliationsItemSchema",
+                                            "class": "nr_metadata.common.services.records.schema_datatypes.NRAffiliationVocabularySchema",
                                             "generate": false,
-                                            "imports": [
-                                                {
-                                                    "alias": "nr_metadata.common.services.records.schema_datatypes",
-                                                    "import": "nr_metadata.common.services.records.schema_datatypes"
-                                                }
-                                            ],
                                             "read": false,
                                             "unknown": "INCLUDE",
                                             "write": false
                                         },
                                         "model": "vocabularies",
                                         "pid-field": "Vocabulary.pid.with_type_ctx(\"institutions\")",
                                         "properties": {
@@ -1322,25 +1723,25 @@
                                                             "additionalProperties": {
                                                                 "type": "string"
                                                             },
                                                             "mapping": {
                                                                 "dynamic": true
                                                             },
                                                             "marshmallow": {
-                                                                "class": "nr_metadata.documents.services.records.schema.TitleItemSchema",
+                                                                "class": "nr_metadata.data.services.records.schema.TitleItemSchema",
                                                                 "field": "i18n_strings",
                                                                 "generate": false
                                                             },
                                                             "propertyNames": {
                                                                 "pattern": "^[a-z]{2}$"
                                                             },
                                                             "type": "object",
                                                             "ui": {
                                                                 "marshmallow": {
-                                                                    "class": "nr_metadata.documents.services.records.ui_schema.TitleItemUISchema",
+                                                                    "class": "nr_metadata.data.services.records.ui_schema.TitleItemUISchema",
                                                                     "field": "i18n_strings",
                                                                     "generate": false
                                                                 }
                                                             }
                                                         },
                                                         "type": "array"
                                                     }
@@ -1379,14 +1780,17 @@
                                                     "marshmallow": {
                                                         "field-class": "marshmallow.fields.String",
                                                         "imports": [],
                                                         "validators": []
                                                     }
                                                 }
                                             },
+                                            "ror": {
+                                                "type": "keyword"
+                                            },
                                             "title": {
                                                 "additionalProperties": {
                                                     "type": "string"
                                                 },
                                                 "mapping": {
                                                     "dynamic": true,
                                                     "properties": {
@@ -1419,50 +1823,30 @@
                                             "faker": "company"
                                         },
                                         "type": "taxonomy",
                                         "ui": {
                                             "detail": "taxonomy_item",
                                             "edit": "taxonomy_item",
                                             "marshmallow": {
-                                                "base-classes": [
-                                                    "nr_metadata.common.services.records.ui_schema_datatypes.NRAffiliationVocabularyUISchema"
-                                                ],
-                                                "class": "nr_metadata.documents.services.records.ui_schema.AffiliationsItemUISchema",
+                                                "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRAffiliationVocabularyUISchema",
                                                 "generate": false,
-                                                "imports": [
-                                                    {
-                                                        "alias": "nr_metadata.common.services.records.ui_schema_datatypes",
-                                                        "import": "nr_metadata.common.services.records.ui_schema_datatypes"
-                                                    }
-                                                ],
                                                 "read": false,
                                                 "unknown": "INCLUDE",
                                                 "write": false
                                             }
                                         },
                                         "vocabulary-type": "institutions"
                                     },
                                     "type": "array"
                                 },
                                 "authorityIdentifiers": {
                                     "items": {
                                         "marshmallow": {
-                                            "base-classes": [
-                                                "nr_metadata.schema.identifiers.NRAuthorityIdentifierSchema"
-                                            ],
-                                            "class": "nr_metadata.documents.services.records.schema.AuthorityIdentifiersItemSchema",
-                                            "generate": false,
-                                            "imports": [
-                                                {
-                                                    "alias": "nr_metadata.schema.identifiers",
-                                                    "import": "nr_metadata.schema.identifiers"
-                                                }
-                                            ],
-                                            "read": false,
-                                            "write": false
+                                            "class": "nr_metadata.schema.identifiers.NROrganizationIdentifierSchema",
+                                            "generate": false
                                         },
                                         "properties": {
                                             "identifier": {
                                                 "i18n.key": "identifier",
                                                 "label.cs": "Identifik\u00e1tor",
                                                 "label.en": "Identifier",
                                                 "marshmallow": {
@@ -1479,20 +1863,14 @@
                                                         "read": false,
                                                         "write": false
                                                     }
                                                 }
                                             },
                                             "scheme": {
                                                 "enum": [
-                                                    "orcid",
-                                                    "scopusID",
-                                                    "researcherID",
-                                                    "czenasAutID",
-                                                    "vedidk",
-                                                    "institutionalID",
                                                     "ISNI",
                                                     "ROR",
                                                     "ICO",
                                                     "DOI"
                                                 ],
                                                 "hint.cs": "Doporu\u010dujeme zadat alespo\u0148 jeden z typ\u016f identifik\u00e1tor\u016f.\nPokud pot\u0159ebujete roz\u0161\u00ed\u0159it nab\u00eddku typ\u016f identifik\u00e1tor\u016f, kontaktujte n\u00e1s na support@narodni-repozitar.cz.\n",
                                                 "hint.en": "We recommend providing at least one of the identifier types.\nIf you need to expand the range of identifier types, contact us at support@narodni-repozitar.cz.\n",
@@ -1511,34 +1889,36 @@
                                                         "write": false
                                                     }
                                                 }
                                             }
                                         },
                                         "type": "object",
                                         "ui": {
-                                            "detail": "nr_authority_identifier",
+                                            "detail": "nr_organization_identifier",
                                             "marshmallow": {
-                                                "base-classes": [
-                                                    "nr_metadata.ui_schema.identifiers.NRAuthorityIdentifierUISchema"
-                                                ],
-                                                "class": "nr_metadata.documents.services.records.ui_schema.AuthorityIdentifiersItemUISchema",
-                                                "generate": false,
-                                                "imports": [
-                                                    {
-                                                        "alias": "nr_metadata.ui_schema.identifiers",
-                                                        "import": "nr_metadata.ui_schema.identifiers"
-                                                    }
-                                                ],
-                                                "read": false,
-                                                "write": false
+                                                "class": "nr_metadata.ui_schema.identifiers.NROrganizationIdentifierUISchema",
+                                                "generate": false
                                             }
                                         }
                                     },
                                     "type": "array"
                                 },
+                                "familyName": {
+                                    "marshmallow": {
+                                        "read": false,
+                                        "write": false
+                                    },
+                                    "type": "keyword",
+                                    "ui": {
+                                        "marshmallow": {
+                                            "read": false,
+                                            "write": false
+                                        }
+                                    }
+                                },
                                 "fullName": {
                                     "label.cs": "Jm\u00e9no autora",
                                     "label.en": "Author name",
                                     "marshmallow": {
                                         "read": false,
                                         "write": false
                                     },
@@ -1550,55 +1930,454 @@
                                     "ui": {
                                         "marshmallow": {
                                             "read": false,
                                             "write": false
                                         }
                                     }
                                 },
+                                "givenName": {
+                                    "marshmallow": {
+                                        "read": false,
+                                        "write": false
+                                    },
+                                    "type": "keyword",
+                                    "ui": {
+                                        "marshmallow": {
+                                            "read": false,
+                                            "write": false
+                                        }
+                                    }
+                                },
                                 "nameType": {
                                     "enum": [
-                                        "Organizational",
-                                        "Personal"
+                                        "Organizational"
                                     ],
-                                    "hint.cs": "Jako tv\u016frce je mo\u017en\u00e9 ozna\u010dit osobu nebo instituci.",
-                                    "hint.en": "It is possible to designate a person or an institution as the creator/contributor.",
                                     "label.cs": "Typ",
                                     "label.en": "Type",
                                     "marshmallow": {
                                         "read": false,
                                         "write": false
                                     },
                                     "sample": [
-                                        "Organizational",
-                                        "Personal"
+                                        "Organizational"
                                     ],
                                     "type": "keyword",
                                     "ui": {
                                         "marshmallow": {
                                             "read": false,
                                             "write": false
                                         }
                                     }
                                 }
                             },
-                            "type": "object",
+                            "schemas": {
+                                "Organizational": {
+                                    "marshmallow": {
+                                        "class": "nr_metadata.common.services.records.schema_datatypes.NROrganizationSchema",
+                                        "generate": false
+                                    },
+                                    "properties": {
+                                        "authorityIdentifiers": {
+                                            "items": {
+                                                "marshmallow": {
+                                                    "class": "nr_metadata.schema.identifiers.NROrganizationIdentifierSchema",
+                                                    "generate": false
+                                                },
+                                                "properties": {
+                                                    "identifier": {
+                                                        "i18n.key": "identifier",
+                                                        "label.cs": "Identifik\u00e1tor",
+                                                        "label.en": "Identifier",
+                                                        "marshmallow": {
+                                                            "read": false,
+                                                            "write": false
+                                                        },
+                                                        "required": true,
+                                                        "sample": {
+                                                            "faker": "isbn13"
+                                                        },
+                                                        "type": "keyword",
+                                                        "ui": {
+                                                            "marshmallow": {
+                                                                "read": false,
+                                                                "write": false
+                                                            }
+                                                        }
+                                                    },
+                                                    "scheme": {
+                                                        "enum": [
+                                                            "ISNI",
+                                                            "ROR",
+                                                            "ICO",
+                                                            "DOI"
+                                                        ],
+                                                        "hint.cs": "Doporu\u010dujeme zadat alespo\u0148 jeden z typ\u016f identifik\u00e1tor\u016f.\nPokud pot\u0159ebujete roz\u0161\u00ed\u0159it nab\u00eddku typ\u016f identifik\u00e1tor\u016f, kontaktujte n\u00e1s na support@narodni-repozitar.cz.\n",
+                                                        "hint.en": "We recommend providing at least one of the identifier types.\nIf you need to expand the range of identifier types, contact us at support@narodni-repozitar.cz.\n",
+                                                        "i18n.key": "identifier_type",
+                                                        "label.cs": "Typ identifik\u00e1toru",
+                                                        "label.en": "Identifier type",
+                                                        "marshmallow": {
+                                                            "read": false,
+                                                            "write": false
+                                                        },
+                                                        "required": true,
+                                                        "type": "keyword",
+                                                        "ui": {
+                                                            "marshmallow": {
+                                                                "read": false,
+                                                                "write": false
+                                                            }
+                                                        }
+                                                    }
+                                                },
+                                                "type": "object",
+                                                "ui": {
+                                                    "detail": "nr_organization_identifier",
+                                                    "marshmallow": {
+                                                        "class": "nr_metadata.ui_schema.identifiers.NROrganizationIdentifierUISchema",
+                                                        "generate": false
+                                                    }
+                                                }
+                                            },
+                                            "type": "array"
+                                        },
+                                        "fullName": {
+                                            "label.cs": "Jm\u00e9no autora",
+                                            "label.en": "Author name",
+                                            "marshmallow": {
+                                                "read": false,
+                                                "write": false
+                                            },
+                                            "required": true,
+                                            "sample": {
+                                                "faker": "name"
+                                            },
+                                            "type": "keyword",
+                                            "ui": {
+                                                "marshmallow": {
+                                                    "read": false,
+                                                    "write": false
+                                                }
+                                            }
+                                        },
+                                        "nameType": {
+                                            "enum": [
+                                                "Organizational"
+                                            ],
+                                            "label.cs": "Typ",
+                                            "label.en": "Type",
+                                            "marshmallow": {
+                                                "read": false,
+                                                "write": false
+                                            },
+                                            "sample": [
+                                                "Organizational"
+                                            ],
+                                            "type": "keyword",
+                                            "ui": {
+                                                "marshmallow": {
+                                                    "read": false,
+                                                    "write": false
+                                                }
+                                            }
+                                        }
+                                    },
+                                    "type": "object",
+                                    "ui": {
+                                        "detail": "nr_organization",
+                                        "marshmallow": {
+                                            "class": "nr_metadata.common.services.records.ui_schema_datatypes.NROrganizationUISchema",
+                                            "generate": false
+                                        }
+                                    }
+                                },
+                                "Personal": {
+                                    "marshmallow": {
+                                        "class": "nr_metadata.common.services.records.schema_datatypes.NRPersonSchema",
+                                        "generate": false
+                                    },
+                                    "properties": {
+                                        "affiliations": {
+                                            "items": {
+                                                "facets": {
+                                                    "args": [
+                                                        "vocabulary='institutions'"
+                                                    ]
+                                                },
+                                                "hint.cs": "Uve\u010fte instituci/instituce, pod jej\u00ed\u017e z\u00e1\u0161titou jste se na tvorb\u011b objektu pod\u00edleli.",
+                                                "imports": [
+                                                    {
+                                                        "import": "invenio_vocabularies.records.api.Vocabulary"
+                                                    }
+                                                ],
+                                                "keys": [
+                                                    "id",
+                                                    "title",
+                                                    {
+                                                        "key": "props.ror",
+                                                        "model": {
+                                                            "type": "keyword"
+                                                        },
+                                                        "target": "ror"
+                                                    },
+                                                    {
+                                                        "key": "hierarchy",
+                                                        "model": {
+                                                            "marshmallow": {
+                                                                "class": "oarepo_vocabularies.services.schema.HierarchySchema",
+                                                                "generate": false,
+                                                                "imports": [
+                                                                    {
+                                                                        "import": "oarepo_vocabularies.services.schema.HierarchySchema"
+                                                                    }
+                                                                ]
+                                                            },
+                                                            "properties": {
+                                                                "ancestors": {
+                                                                    "items": {
+                                                                        "type": "keyword"
+                                                                    },
+                                                                    "type": "array"
+                                                                },
+                                                                "ancestors_or_self": {
+                                                                    "items": {
+                                                                        "type": "keyword"
+                                                                    },
+                                                                    "type": "array"
+                                                                },
+                                                                "level": {
+                                                                    "type": "integer"
+                                                                },
+                                                                "parent": {
+                                                                    "type": "keyword"
+                                                                },
+                                                                "title": {
+                                                                    "items": {
+                                                                        "additionalProperties": {
+                                                                            "type": "string"
+                                                                        },
+                                                                        "mapping": {
+                                                                            "dynamic": true
+                                                                        },
+                                                                        "marshmallow": {
+                                                                            "class": "nr_metadata.data.services.records.schema.TitleItemSchema",
+                                                                            "field": "i18n_strings",
+                                                                            "generate": false
+                                                                        },
+                                                                        "propertyNames": {
+                                                                            "pattern": "^[a-z]{2}$"
+                                                                        },
+                                                                        "type": "object",
+                                                                        "ui": {
+                                                                            "marshmallow": {
+                                                                                "class": "nr_metadata.data.services.records.ui_schema.TitleItemUISchema",
+                                                                                "field": "i18n_strings",
+                                                                                "generate": false
+                                                                            }
+                                                                        }
+                                                                    },
+                                                                    "type": "array"
+                                                                }
+                                                            },
+                                                            "type": "object",
+                                                            "ui": {
+                                                                "marshmallow": {
+                                                                    "class": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema",
+                                                                    "generate": false,
+                                                                    "imports": [
+                                                                        {
+                                                                            "import": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema"
+                                                                        }
+                                                                    ]
+                                                                }
+                                                            }
+                                                        },
+                                                        "target": "hierarchy"
+                                                    }
+                                                ],
+                                                "label.cs": "Afiliace",
+                                                "label.en": "Affiliation",
+                                                "marshmallow": {
+                                                    "class": "nr_metadata.common.services.records.schema_datatypes.NRAffiliationVocabularySchema",
+                                                    "generate": false,
+                                                    "read": false,
+                                                    "unknown": "INCLUDE",
+                                                    "write": false
+                                                },
+                                                "model": "vocabularies",
+                                                "pid-field": "Vocabulary.pid.with_type_ctx(\"institutions\")",
+                                                "properties": {},
+                                                "sample": {
+                                                    "faker": "company"
+                                                },
+                                                "type": "taxonomy",
+                                                "ui": {
+                                                    "detail": "taxonomy_item",
+                                                    "edit": "taxonomy_item",
+                                                    "marshmallow": {
+                                                        "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRAffiliationVocabularyUISchema",
+                                                        "generate": false,
+                                                        "read": false,
+                                                        "unknown": "INCLUDE",
+                                                        "write": false
+                                                    }
+                                                },
+                                                "vocabulary-type": "institutions"
+                                            },
+                                            "type": "array"
+                                        },
+                                        "authorityIdentifiers": {
+                                            "items": {
+                                                "marshmallow": {
+                                                    "class": "nr_metadata.schema.identifiers.NRPersonIdentifierSchema",
+                                                    "generate": false
+                                                },
+                                                "properties": {
+                                                    "identifier": {
+                                                        "i18n.key": "identifier",
+                                                        "label.cs": "Identifik\u00e1tor",
+                                                        "label.en": "Identifier",
+                                                        "marshmallow": {
+                                                            "read": false,
+                                                            "write": false
+                                                        },
+                                                        "required": true,
+                                                        "sample": {
+                                                            "faker": "isbn13"
+                                                        },
+                                                        "type": "keyword",
+                                                        "ui": {
+                                                            "marshmallow": {
+                                                                "read": false,
+                                                                "write": false
+                                                            }
+                                                        }
+                                                    },
+                                                    "scheme": {
+                                                        "enum": [
+                                                            "orcid",
+                                                            "scopusID",
+                                                            "researcherID",
+                                                            "czenasAutID",
+                                                            "vedidk",
+                                                            "institutionalID",
+                                                            "ISNI"
+                                                        ],
+                                                        "hint.cs": "Doporu\u010dujeme zadat alespo\u0148 jeden z typ\u016f identifik\u00e1tor\u016f.\nPokud pot\u0159ebujete roz\u0161\u00ed\u0159it nab\u00eddku typ\u016f identifik\u00e1tor\u016f, kontaktujte n\u00e1s na support@narodni-repozitar.cz.\n",
+                                                        "hint.en": "We recommend providing at least one of the identifier types.\nIf you need to expand the range of identifier types, contact us at support@narodni-repozitar.cz.\n",
+                                                        "i18n.key": "identifier_type",
+                                                        "label.cs": "Typ identifik\u00e1toru",
+                                                        "label.en": "Identifier type",
+                                                        "marshmallow": {
+                                                            "read": false,
+                                                            "write": false
+                                                        },
+                                                        "required": true,
+                                                        "type": "keyword",
+                                                        "ui": {
+                                                            "marshmallow": {
+                                                                "read": false,
+                                                                "write": false
+                                                            }
+                                                        }
+                                                    }
+                                                },
+                                                "type": "object",
+                                                "ui": {
+                                                    "detail": "nr_person_identifier",
+                                                    "marshmallow": {
+                                                        "class": "nr_metadata.ui_schema.identifiers.NRPersonIdentifierUISchema",
+                                                        "generate": false
+                                                    }
+                                                }
+                                            },
+                                            "type": "array"
+                                        },
+                                        "familyName": {
+                                            "marshmallow": {
+                                                "read": false,
+                                                "write": false
+                                            },
+                                            "type": "keyword",
+                                            "ui": {
+                                                "marshmallow": {
+                                                    "read": false,
+                                                    "write": false
+                                                }
+                                            }
+                                        },
+                                        "fullName": {
+                                            "label.cs": "Jm\u00e9no autora",
+                                            "label.en": "Author name",
+                                            "marshmallow": {
+                                                "read": false,
+                                                "write": false
+                                            },
+                                            "required": true,
+                                            "sample": {
+                                                "faker": "name"
+                                            },
+                                            "type": "keyword",
+                                            "ui": {
+                                                "marshmallow": {
+                                                    "read": false,
+                                                    "write": false
+                                                }
+                                            }
+                                        },
+                                        "givenName": {
+                                            "marshmallow": {
+                                                "read": false,
+                                                "write": false
+                                            },
+                                            "type": "keyword",
+                                            "ui": {
+                                                "marshmallow": {
+                                                    "read": false,
+                                                    "write": false
+                                                }
+                                            }
+                                        },
+                                        "nameType": {
+                                            "enum": [
+                                                "Personal"
+                                            ],
+                                            "label.cs": "Typ",
+                                            "label.en": "Type",
+                                            "marshmallow": {
+                                                "read": false,
+                                                "write": false
+                                            },
+                                            "type": "keyword",
+                                            "ui": {
+                                                "marshmallow": {
+                                                    "read": false,
+                                                    "write": false
+                                                }
+                                            }
+                                        }
+                                    },
+                                    "type": "object",
+                                    "ui": {
+                                        "detail": "nr_person",
+                                        "marshmallow": {
+                                            "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRPersonUISchema",
+                                            "generate": false
+                                        }
+                                    }
+                                }
+                            },
+                            "type": "polymorphic",
                             "ui": {
                                 "detail": "creator",
                                 "marshmallow": {
-                                    "base-classes": [
-                                        "nr_metadata.common.services.records.ui_schema_common.NRCreatorUISchema"
-                                    ],
-                                    "class": "nr_metadata.documents.services.records.ui_schema.CreatorsItemUISchema",
+                                    "class": "nr_metadata.common.services.records.ui_schema_common.NRCreatorUISchema",
                                     "generate": true,
-                                    "imports": [
-                                        {
-                                            "alias": "nr_metadata.common.services.records.ui_schema_common",
-                                            "import": "nr_metadata.common.services.records.ui_schema_common"
-                                        }
-                                    ]
+                                    "read": false,
+                                    "write": false
                                 }
                             }
                         },
                         "label.cs": "Auto\u0159i",
                         "label.en": "Authors",
                         "marshmallow": {
                             "validators": [
@@ -1615,22 +2394,28 @@
                         "marshmallow": {
                             "read": false,
                             "write": false
                         },
                         "sample": {
                             "faker": "date"
                         },
-                        "type": "edtf",
+                        "type": "date",
                         "ui": {
                             "marshmallow": {
                                 "read": false,
                                 "write": false
                             }
                         }
                     },
+                    "dateCollected": {
+                        "type": "edtf-interval"
+                    },
+                    "dateCreated": {
+                        "type": "edtf-interval"
+                    },
                     "dateIssued": {
                         "label.cs": "Datum vyd\u00e1n\u00ed",
                         "label.en": "Date issued",
                         "marshmallow": {
                             "read": false,
                             "write": false
                         },
@@ -1641,48 +2426,43 @@
                         "ui": {
                             "marshmallow": {
                                 "read": false,
                                 "write": false
                             }
                         }
                     },
-                    "dateModified": {
-                        "label.cs": "Datum zm\u011bny zdroje",
-                        "label.en": "Date modified",
+                    "dateValidTo": {
+                        "type": "date"
+                    },
+                    "dateWithdrawn": {
                         "marshmallow": {
-                            "read": false,
-                            "write": false
+                            "class": "nr_metadata.data.services.records.schema.DateWithdrawnSchema",
+                            "generate": true
                         },
-                        "sample": {
-                            "faker": "date"
+                        "properties": {
+                            "dateInformation": {
+                                "type": "keyword"
+                            },
+                            "type": {
+                                "type": "date"
+                            }
                         },
-                        "type": "edtf",
+                        "type": "object",
                         "ui": {
                             "marshmallow": {
-                                "read": false,
-                                "write": false
+                                "class": "nr_metadata.data.services.records.ui_schema.DateWithdrawnUISchema",
+                                "generate": true
                             }
                         }
                     },
                     "events": {
                         "items": {
                             "marshmallow": {
-                                "base-classes": [
-                                    "nr_metadata.common.services.records.schema_datatypes.NREventSchema"
-                                ],
-                                "class": "nr_metadata.documents.services.records.schema.EventsItemSchema",
-                                "generate": true,
-                                "imports": [
-                                    {
-                                        "alias": "nr_metadata.common.services.records.schema_datatypes",
-                                        "import": "nr_metadata.common.services.records.schema_datatypes"
-                                    }
-                                ],
-                                "read": false,
-                                "write": false
+                                "class": "nr_metadata.common.services.records.schema_datatypes.NREventSchema",
+                                "generate": false
                             },
                             "properties": {
                                 "eventDate": {
                                     "label.cs": "Datum kon\u00e1n\u00ed akce",
                                     "label.en": "Event date",
                                     "marshmallow": {
                                         "read": false,
@@ -1695,27 +2475,16 @@
                                             "read": false,
                                             "write": false
                                         }
                                     }
                                 },
                                 "eventLocation": {
                                     "marshmallow": {
-                                        "base-classes": [
-                                            "nr_metadata.common.services.records.schema_datatypes.NRLocationSchema"
-                                        ],
-                                        "class": "nr_metadata.documents.services.records.schema.EventLocationSchema",
-                                        "generate": true,
-                                        "imports": [
-                                            {
-                                                "alias": "nr_metadata.common.services.records.schema_datatypes",
-                                                "import": "nr_metadata.common.services.records.schema_datatypes"
-                                            }
-                                        ],
-                                        "read": false,
-                                        "write": false
+                                        "class": "nr_metadata.common.services.records.schema_datatypes.NRLocationSchema",
+                                        "generate": false
                                     },
                                     "properties": {
                                         "country": {
                                             "facets": {
                                                 "args": [
                                                     "vocabulary='countries'"
                                                 ]
@@ -1728,25 +2497,16 @@
                                             "keys": [
                                                 "id",
                                                 "title"
                                             ],
                                             "label.cs": "Zem\u011b",
                                             "label.en": "Country",
                                             "marshmallow": {
-                                                "base-classes": [
-                                                    "nr_metadata.common.services.records.schema_datatypes.NRCountryVocabularySchema"
-                                                ],
-                                                "class": "nr_metadata.documents.services.records.schema.CountrySchema",
+                                                "class": "nr_metadata.common.services.records.schema_datatypes.NRCountryVocabularySchema",
                                                 "generate": true,
-                                                "imports": [
-                                                    {
-                                                        "alias": "nr_metadata.common.services.records.schema_datatypes",
-                                                        "import": "nr_metadata.common.services.records.schema_datatypes"
-                                                    }
-                                                ],
                                                 "read": false,
                                                 "unknown": "INCLUDE",
                                                 "write": false
                                             },
                                             "model": "vocabularies",
                                             "pid-field": "Vocabulary.pid.with_type_ctx(\"countries\")",
                                             "properties": {
@@ -1824,25 +2584,16 @@
                                                 }
                                             },
                                             "type": "vocabulary",
                                             "ui": {
                                                 "detail": "vocabulary_item",
                                                 "edit": "vocabulary_item",
                                                 "marshmallow": {
-                                                    "base-classes": [
-                                                        "nr_metadata.common.services.records.ui_schema_datatypes.NRCountryVocabularyUISchema"
-                                                    ],
-                                                    "class": "nr_metadata.documents.services.records.ui_schema.CountryUISchema",
+                                                    "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRCountryVocabularyUISchema",
                                                     "generate": true,
-                                                    "imports": [
-                                                        {
-                                                            "alias": "nr_metadata.common.services.records.ui_schema_datatypes",
-                                                            "import": "nr_metadata.common.services.records.ui_schema_datatypes"
-                                                        }
-                                                    ],
                                                     "read": false,
                                                     "unknown": "INCLUDE",
                                                     "write": false
                                                 }
                                             },
                                             "vocabulary-type": "countries"
                                         },
@@ -1864,27 +2615,16 @@
                                         }
                                     },
                                     "required": true,
                                     "type": "object",
                                     "ui": {
                                         "detail": "location",
                                         "marshmallow": {
-                                            "base-classes": [
-                                                "nr_metadata.common.services.records.ui_schema_datatypes.NRLocationUISchema"
-                                            ],
-                                            "class": "nr_metadata.documents.services.records.ui_schema.EventLocationUISchema",
-                                            "generate": true,
-                                            "imports": [
-                                                {
-                                                    "alias": "nr_metadata.common.services.records.ui_schema_datatypes",
-                                                    "import": "nr_metadata.common.services.records.ui_schema_datatypes"
-                                                }
-                                            ],
-                                            "read": false,
-                                            "write": false
+                                            "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRLocationUISchema",
+                                            "generate": false
                                         }
                                     }
                                 },
                                 "eventNameAlternate": {
                                     "items": {
                                         "label.cs": "Alternativn\u00ed n\u00e1zev akce",
                                         "label.en": "Event alternate name",
@@ -1919,122 +2659,28 @@
                                     }
                                 }
                             },
                             "type": "object",
                             "ui": {
                                 "detail": "identifier",
                                 "marshmallow": {
-                                    "base-classes": [
-                                        "nr_metadata.common.services.records.ui_schema_datatypes.NREventUISchema"
-                                    ],
-                                    "class": "nr_metadata.documents.services.records.ui_schema.EventsItemUISchema",
-                                    "generate": true,
-                                    "imports": [
-                                        {
-                                            "alias": "nr_metadata.common.services.records.ui_schema_datatypes",
-                                            "import": "nr_metadata.common.services.records.ui_schema_datatypes"
-                                        }
-                                    ],
-                                    "read": false,
-                                    "write": false
+                                    "class": "nr_metadata.common.services.records.ui_schema_datatypes.NREventUISchema",
+                                    "generate": false
                                 }
                             }
                         },
                         "label.cs": "Ud\u00e1losti",
                         "label.en": "Events",
                         "type": "array"
                     },
-                    "externalLocation": {
-                        "marshmallow": {
-                            "base-classes": [
-                                "nr_metadata.common.services.records.schema_datatypes.NRExternalLocationSchema"
-                            ],
-                            "class": "nr_metadata.documents.services.records.schema.ExternalLocationSchema",
-                            "generate": true,
-                            "imports": [
-                                {
-                                    "alias": "nr_metadata.common.services.records.schema_datatypes",
-                                    "import": "nr_metadata.common.services.records.schema_datatypes"
-                                }
-                            ],
-                            "read": false,
-                            "write": false
-                        },
-                        "properties": {
-                            "externalLocationNote": {
-                                "label.cs": "Pozn\u00e1mka",
-                                "label.en": "Note",
-                                "marshmallow": {
-                                    "read": false,
-                                    "write": false
-                                },
-                                "type": "fulltext",
-                                "ui": {
-                                    "marshmallow": {
-                                        "read": false,
-                                        "write": false
-                                    }
-                                }
-                            },
-                            "externalLocationURL": {
-                                "label.cs": "Extern\u00ed um\u00edst\u011bn\u00ed zdroje",
-                                "label.en": "Resource external location",
-                                "marshmallow": {
-                                    "read": false,
-                                    "write": false
-                                },
-                                "required": true,
-                                "sample": {
-                                    "faker": "url"
-                                },
-                                "type": "url",
-                                "ui": {
-                                    "marshmallow": {
-                                        "read": false,
-                                        "write": false
-                                    }
-                                }
-                            }
-                        },
-                        "type": "object",
-                        "ui": {
-                            "detail": "external_location",
-                            "marshmallow": {
-                                "base-classes": [
-                                    "nr_metadata.common.services.records.ui_schema_datatypes.NRExternalLocationUISchema"
-                                ],
-                                "class": "nr_metadata.documents.services.records.ui_schema.ExternalLocationUISchema",
-                                "generate": true,
-                                "imports": [
-                                    {
-                                        "alias": "nr_metadata.common.services.records.ui_schema_datatypes",
-                                        "import": "nr_metadata.common.services.records.ui_schema_datatypes"
-                                    }
-                                ],
-                                "read": false,
-                                "write": false
-                            }
-                        }
-                    },
                     "fundingReferences": {
                         "items": {
                             "marshmallow": {
-                                "base-classes": [
-                                    "nr_metadata.common.services.records.schema_datatypes.NRFundingReferenceSchema"
-                                ],
-                                "class": "nr_metadata.documents.services.records.schema.FundingReferencesItemSchema",
-                                "generate": true,
-                                "imports": [
-                                    {
-                                        "alias": "nr_metadata.common.services.records.schema_datatypes",
-                                        "import": "nr_metadata.common.services.records.schema_datatypes"
-                                    }
-                                ],
-                                "read": false,
-                                "write": false
+                                "class": "nr_metadata.common.services.records.schema_datatypes.NRFundingReferenceSchema",
+                                "generate": false
                             },
                             "properties": {
                                 "funder": {
                                     "facets": {
                                         "args": [
                                             "vocabulary='funders'"
                                         ]
@@ -2047,25 +2693,16 @@
                                     "keys": [
                                         "id",
                                         "title"
                                     ],
                                     "label.cs": "Poskytovatel financ\u00ed",
                                     "label.en": "Funder",
                                     "marshmallow": {
-                                        "base-classes": [
-                                            "nr_metadata.common.services.records.schema_datatypes.NRFunderVocabularySchema"
-                                        ],
-                                        "class": "nr_metadata.documents.services.records.schema.FunderSchema",
+                                        "class": "nr_metadata.common.services.records.schema_datatypes.NRFunderVocabularySchema",
                                         "generate": true,
-                                        "imports": [
-                                            {
-                                                "alias": "nr_metadata.common.services.records.schema_datatypes",
-                                                "import": "nr_metadata.common.services.records.schema_datatypes"
-                                            }
-                                        ],
                                         "read": false,
                                         "unknown": "INCLUDE",
                                         "write": false
                                     },
                                     "model": "vocabularies",
                                     "pid-field": "Vocabulary.pid.with_type_ctx(\"funders\")",
                                     "properties": {
@@ -2143,25 +2780,16 @@
                                         }
                                     },
                                     "type": "vocabulary",
                                     "ui": {
                                         "detail": "vocabulary_item",
                                         "edit": "vocabulary_item",
                                         "marshmallow": {
-                                            "base-classes": [
-                                                "nr_metadata.common.services.records.ui_schema_datatypes.NRFunderVocabularyUISchema"
-                                            ],
-                                            "class": "nr_metadata.documents.services.records.ui_schema.FunderUISchema",
+                                            "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRFunderVocabularyUISchema",
                                             "generate": true,
-                                            "imports": [
-                                                {
-                                                    "alias": "nr_metadata.common.services.records.ui_schema_datatypes",
-                                                    "import": "nr_metadata.common.services.records.ui_schema_datatypes"
-                                                }
-                                            ],
                                             "read": false,
                                             "unknown": "INCLUDE",
                                             "write": false
                                         }
                                     },
                                     "vocabulary-type": "funders"
                                 },
@@ -2212,80 +2840,48 @@
                                     }
                                 }
                             },
                             "type": "object",
                             "ui": {
                                 "detail": "funding_reference",
                                 "marshmallow": {
-                                    "base-classes": [
-                                        "nr_metadata.common.services.records.ui_schema_datatypes.NRFundingReferenceUISchema"
-                                    ],
-                                    "class": "nr_metadata.documents.services.records.ui_schema.FundingReferencesItemUISchema",
-                                    "generate": true,
-                                    "imports": [
-                                        {
-                                            "alias": "nr_metadata.common.services.records.ui_schema_datatypes",
-                                            "import": "nr_metadata.common.services.records.ui_schema_datatypes"
-                                        }
-                                    ],
-                                    "read": false,
-                                    "write": false
+                                    "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRFundingReferenceUISchema",
+                                    "generate": false
                                 }
                             }
                         },
                         "label.cs": "Projekt nebo financov\u00e1n\u00ed",
                         "label.en": "Funding",
                         "type": "array"
                     },
                     "geoLocations": {
                         "items": {
                             "marshmallow": {
-                                "base-classes": [
-                                    "nr_metadata.common.services.records.schema_datatypes.NRGeoLocationSchema"
-                                ],
-                                "class": "nr_metadata.documents.services.records.schema.GeoLocationsItemSchema",
-                                "generate": true,
-                                "imports": [
-                                    {
-                                        "alias": "nr_metadata.common.services.records.schema_datatypes",
-                                        "import": "nr_metadata.common.services.records.schema_datatypes"
-                                    }
-                                ],
-                                "read": false,
-                                "write": false
+                                "class": "nr_metadata.common.services.records.schema_datatypes.NRGeoLocationSchema",
+                                "generate": false
                             },
                             "properties": {
                                 "geoLocationPlace": {
                                     "description": "Free description of the location; ie. Atlantic Ocean",
                                     "marshmallow": {
                                         "read": false,
                                         "write": false
                                     },
-                                    "required": true,
                                     "type": "keyword",
                                     "ui": {
                                         "marshmallow": {
                                             "read": false,
                                             "write": false
                                         }
                                     }
                                 },
                                 "geoLocationPoint": {
                                     "marshmallow": {
-                                        "base-classes": [
-                                            "nr_metadata.common.services.records.schema_datatypes.NRGeoLocationPointSchema"
-                                        ],
-                                        "class": "nr_metadata.documents.services.records.schema.GeoLocationPointSchema",
-                                        "generate": true,
-                                        "imports": [
-                                            {
-                                                "alias": "nr_metadata.common.services.records.schema_datatypes",
-                                                "import": "nr_metadata.common.services.records.schema_datatypes"
-                                            }
-                                        ]
+                                        "class": "nr_metadata.common.services.records.schema_datatypes.NRGeoLocationPointSchema",
+                                        "generate": false
                                     },
                                     "properties": {
                                         "pointLatitude": {
                                             "label.cs": "Zem\u011bpisn\u00e1 \u0161\u00ed\u0159ka",
                                             "label.en": "Latitude",
                                             "marshmallow": {
                                                 "read": false,
@@ -2327,46 +2923,26 @@
                                             }
                                         }
                                     },
                                     "type": "object",
                                     "ui": {
                                         "detail": "geolocation_point",
                                         "marshmallow": {
-                                            "base-classes": [
-                                                "nr_metadata.common.services.records.ui_schema_datatypes.NRGeoLocationPointUISchema"
-                                            ],
-                                            "class": "nr_metadata.documents.services.records.ui_schema.GeoLocationPointUISchema",
-                                            "generate": true,
-                                            "imports": [
-                                                {
-                                                    "alias": "nr_metadata.common.services.records.ui_schema_datatypes",
-                                                    "import": "nr_metadata.common.services.records.ui_schema_datatypes"
-                                                }
-                                            ]
+                                            "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRGeoLocationPointUISchema",
+                                            "generate": false
                                         }
                                     }
                                 }
                             },
                             "type": "object",
                             "ui": {
                                 "detail": "geolocation",
                                 "marshmallow": {
-                                    "base-classes": [
-                                        "nr_metadata.common.services.records.ui_schema_datatypes.NRGeoLocationUISchema"
-                                    ],
-                                    "class": "nr_metadata.documents.services.records.ui_schema.GeoLocationsItemUISchema",
-                                    "generate": true,
-                                    "imports": [
-                                        {
-                                            "alias": "nr_metadata.common.services.records.ui_schema_datatypes",
-                                            "import": "nr_metadata.common.services.records.ui_schema_datatypes"
-                                        }
-                                    ],
-                                    "read": false,
-                                    "write": false
+                                    "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRGeoLocationUISchema",
+                                    "generate": false
                                 }
                             }
                         },
                         "label.cs": "Geolokace",
                         "label.en": "Geolocation",
                         "type": "array"
                     },
@@ -2385,25 +2961,16 @@
                             "keys": [
                                 "id",
                                 "title"
                             ],
                             "label.cs": "Jazyk",
                             "label.en": "Language",
                             "marshmallow": {
-                                "base-classes": [
-                                    "nr_metadata.common.services.records.schema_datatypes.NRLanguageVocabularySchema"
-                                ],
-                                "class": "nr_metadata.documents.services.records.schema.LanguagesItemSchema",
+                                "class": "nr_metadata.common.services.records.schema_datatypes.NRLanguageVocabularySchema",
                                 "generate": true,
-                                "imports": [
-                                    {
-                                        "alias": "nr_metadata.common.services.records.schema_datatypes",
-                                        "import": "nr_metadata.common.services.records.schema_datatypes"
-                                    }
-                                ],
                                 "read": false,
                                 "unknown": "INCLUDE",
                                 "write": false
                             },
                             "model": "vocabularies",
                             "pid-field": "Vocabulary.pid.with_type_ctx(\"languages\")",
                             "properties": {
@@ -2488,41 +3055,25 @@
                                 "it"
                             ],
                             "type": "vocabulary",
                             "ui": {
                                 "detail": "vocabulary_item",
                                 "edit": "vocabulary_item",
                                 "marshmallow": {
-                                    "base-classes": [
-                                        "nr_metadata.common.services.records.ui_schema_datatypes.NRLanguageVocabularyUISchema"
-                                    ],
-                                    "class": "nr_metadata.documents.services.records.ui_schema.LanguagesItemUISchema",
+                                    "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRLanguageVocabularyUISchema",
                                     "generate": true,
-                                    "imports": [
-                                        {
-                                            "alias": "nr_metadata.common.services.records.ui_schema_datatypes",
-                                            "import": "nr_metadata.common.services.records.ui_schema_datatypes"
-                                        }
-                                    ],
                                     "read": false,
                                     "unknown": "INCLUDE",
                                     "write": false
                                 }
                             },
                             "vocabulary-type": "languages"
                         },
                         "label.cs": "Jazyk",
                         "label.en": "Language",
-                        "marshmallow": {
-                            "validators": [
-                                "ma.validate.Length(min=1)"
-                            ]
-                        },
-                        "minItems": 1,
-                        "required": true,
                         "type": "array"
                     },
                     "methods": {
                         "items": {
                             "marshmallow": {
                                 "class": null,
                                 "field-class": "oarepo_runtime.services.schema.i18n.I18nStrField",
@@ -2585,27 +3136,16 @@
                         "label.cs": "Pozn\u00e1mky",
                         "label.en": "Notes",
                         "type": "array"
                     },
                     "objectIdentifiers": {
                         "items": {
                             "marshmallow": {
-                                "base-classes": [
-                                    "nr_metadata.schema.identifiers.NRObjectIdentifierSchema"
-                                ],
-                                "class": "nr_metadata.documents.services.records.schema.ObjectIdentifiersItemSchema",
-                                "generate": true,
-                                "imports": [
-                                    {
-                                        "alias": "nr_metadata.schema.identifiers",
-                                        "import": "nr_metadata.schema.identifiers"
-                                    }
-                                ],
-                                "read": false,
-                                "write": false
+                                "class": "nr_metadata.schema.identifiers.NRObjectIdentifierSchema",
+                                "generate": false
                             },
                             "properties": {
                                 "identifier": {
                                     "label.cs": "Identifik\u00e1tor objektu",
                                     "label.en": "Object identifier",
                                     "marshmallow": {
                                         "read": false,
@@ -2625,15 +3165,16 @@
                                 },
                                 "scheme": {
                                     "enum": [
                                         "DOI",
                                         "Handle",
                                         "ISBN",
                                         "ISSN",
-                                        "RIV"
+                                        "RIV",
+                                        "IGSN"
                                     ],
                                     "label.cs": "Typ identifik\u00e1toru",
                                     "label.en": "Identifier type",
                                     "marshmallow": {
                                         "read": false,
                                         "write": false
                                     },
@@ -2647,27 +3188,16 @@
                                     }
                                 }
                             },
                             "type": "object",
                             "ui": {
                                 "detail": "nr_object_pid",
                                 "marshmallow": {
-                                    "base-classes": [
-                                        "nr_metadata.ui_schema.identifiers.NRObjectIdentifierUISchema"
-                                    ],
-                                    "class": "nr_metadata.documents.services.records.ui_schema.ObjectIdentifiersItemUISchema",
-                                    "generate": true,
-                                    "imports": [
-                                        {
-                                            "alias": "nr_metadata.ui_schema.identifiers",
-                                            "import": "nr_metadata.ui_schema.identifiers"
-                                        }
-                                    ],
-                                    "read": false,
-                                    "write": false
+                                    "class": "nr_metadata.ui_schema.identifiers.NRObjectIdentifierUISchema",
+                                    "generate": false
                                 }
                             }
                         },
                         "label.cs": "Identifik\u00e1tory objektu",
                         "label.en": "Object identifiers",
                         "type": "array"
                     },
@@ -2687,65 +3217,300 @@
                                 "read": false,
                                 "write": false
                             }
                         }
                     },
                     "publishers": {
                         "items": {
+                            "facets": {
+                                "args": [
+                                    "vocabulary='institutions'"
+                                ]
+                            },
+                            "imports": [
+                                {
+                                    "import": "invenio_vocabularies.records.api.Vocabulary"
+                                }
+                            ],
+                            "keys": [
+                                "id",
+                                "title",
+                                {
+                                    "key": "props.ror",
+                                    "model": {
+                                        "type": "keyword"
+                                    },
+                                    "target": "ror"
+                                },
+                                {
+                                    "key": "hierarchy",
+                                    "model": {
+                                        "marshmallow": {
+                                            "class": "oarepo_vocabularies.services.schema.HierarchySchema",
+                                            "generate": false,
+                                            "imports": [
+                                                {
+                                                    "import": "oarepo_vocabularies.services.schema.HierarchySchema"
+                                                }
+                                            ]
+                                        },
+                                        "properties": {
+                                            "ancestors": {
+                                                "items": {
+                                                    "type": "keyword"
+                                                },
+                                                "type": "array"
+                                            },
+                                            "ancestors_or_self": {
+                                                "items": {
+                                                    "type": "keyword"
+                                                },
+                                                "type": "array"
+                                            },
+                                            "level": {
+                                                "type": "integer"
+                                            },
+                                            "parent": {
+                                                "type": "keyword"
+                                            },
+                                            "title": {
+                                                "items": {
+                                                    "additionalProperties": {
+                                                        "type": "string"
+                                                    },
+                                                    "mapping": {
+                                                        "dynamic": true
+                                                    },
+                                                    "marshmallow": {
+                                                        "class": "nr_metadata.data.services.records.schema.TitleItemSchema",
+                                                        "field": "i18n_strings",
+                                                        "generate": false
+                                                    },
+                                                    "propertyNames": {
+                                                        "pattern": "^[a-z]{2}$"
+                                                    },
+                                                    "type": "object",
+                                                    "ui": {
+                                                        "marshmallow": {
+                                                            "class": "nr_metadata.data.services.records.ui_schema.TitleItemUISchema",
+                                                            "field": "i18n_strings",
+                                                            "generate": false
+                                                        }
+                                                    }
+                                                },
+                                                "type": "array"
+                                            }
+                                        },
+                                        "type": "object",
+                                        "ui": {
+                                            "marshmallow": {
+                                                "class": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema",
+                                                "generate": false,
+                                                "imports": [
+                                                    {
+                                                        "import": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema"
+                                                    }
+                                                ]
+                                            }
+                                        }
+                                    },
+                                    "target": "hierarchy"
+                                }
+                            ],
                             "marshmallow": {
-                                "read": false,
-                                "write": false
+                                "class": "nr_metadata.data.services.records.schema.PublishersItemSchema",
+                                "generate": true,
+                                "unknown": "INCLUDE"
                             },
-                            "sample": {
-                                "faker": "company"
+                            "model": "vocabularies",
+                            "pid-field": "Vocabulary.pid.with_type_ctx(\"institutions\")",
+                            "properties": {
+                                "@v": {
+                                    "facets": {
+                                        "facet": false
+                                    },
+                                    "marshmallow": {
+                                        "field-class": "marshmallow.fields.String",
+                                        "field-name": "_version"
+                                    },
+                                    "type": "keyword",
+                                    "ui": {
+                                        "marshmallow": {
+                                            "field-class": "marshmallow.fields.String",
+                                            "field-name": "_version"
+                                        }
+                                    }
+                                },
+                                "hierarchy": {
+                                    "marshmallow": {
+                                        "class": "oarepo_vocabularies.services.schema.HierarchySchema",
+                                        "generate": false,
+                                        "imports": [
+                                            {
+                                                "import": "oarepo_vocabularies.services.schema.HierarchySchema"
+                                            }
+                                        ]
+                                    },
+                                    "properties": {
+                                        "ancestors": {
+                                            "items": {
+                                                "type": "keyword"
+                                            },
+                                            "type": "array"
+                                        },
+                                        "ancestors_or_self": {
+                                            "items": {
+                                                "type": "keyword"
+                                            },
+                                            "type": "array"
+                                        },
+                                        "level": {
+                                            "type": "integer"
+                                        },
+                                        "parent": {
+                                            "type": "keyword"
+                                        },
+                                        "title": {
+                                            "items": {
+                                                "additionalProperties": {
+                                                    "type": "string"
+                                                },
+                                                "mapping": {
+                                                    "dynamic": true
+                                                },
+                                                "marshmallow": {
+                                                    "class": "nr_metadata.data.services.records.schema.TitleItemSchema",
+                                                    "field": "i18n_strings",
+                                                    "generate": false
+                                                },
+                                                "propertyNames": {
+                                                    "pattern": "^[a-z]{2}$"
+                                                },
+                                                "type": "object",
+                                                "ui": {
+                                                    "marshmallow": {
+                                                        "class": "nr_metadata.data.services.records.ui_schema.TitleItemUISchema",
+                                                        "field": "i18n_strings",
+                                                        "generate": false
+                                                    }
+                                                }
+                                            },
+                                            "type": "array"
+                                        }
+                                    },
+                                    "type": "object",
+                                    "ui": {
+                                        "marshmallow": {
+                                            "class": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema",
+                                            "generate": false,
+                                            "imports": [
+                                                {
+                                                    "import": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema"
+                                                }
+                                            ]
+                                        }
+                                    }
+                                },
+                                "id": {
+                                    "mapping": {
+                                        "fields": {
+                                            "text": {
+                                                "type": "search_as_you_type"
+                                            }
+                                        }
+                                    },
+                                    "marshmallow": {
+                                        "field-class": "marshmallow.fields.String",
+                                        "imports": [],
+                                        "validators": []
+                                    },
+                                    "sample": {
+                                        "skip": true
+                                    },
+                                    "type": "keyword",
+                                    "ui": {
+                                        "marshmallow": {
+                                            "field-class": "marshmallow.fields.String",
+                                            "imports": [],
+                                            "validators": []
+                                        }
+                                    }
+                                },
+                                "ror": {
+                                    "type": "keyword"
+                                },
+                                "title": {
+                                    "additionalProperties": {
+                                        "type": "string"
+                                    },
+                                    "mapping": {
+                                        "dynamic": true,
+                                        "properties": {
+                                            "en": {
+                                                "copy_to": "title_sort",
+                                                "type": "search_as_you_type"
+                                            }
+                                        }
+                                    },
+                                    "marshmallow": {
+                                        "class": "invenio_vocabularies.services.records.schema.TitleSchema",
+                                        "field": "{{invenio_vocabularies.services.schema.i18n_strings}}",
+                                        "field-class": "marshmallow.fields.Nested",
+                                        "generate": false,
+                                        "validators": []
+                                    },
+                                    "propertyNames": {
+                                        "pattern": "^[a-z]{2}$"
+                                    },
+                                    "type": "object",
+                                    "ui": {
+                                        "marshmallow": {
+                                            "field": "{{oarepo_vocabularies.services.ui_schema.VocabularyI18nStrUIField}}()",
+                                            "generate": false
+                                        }
+                                    }
+                                }
                             },
-                            "type": "fulltext",
+                            "type": "taxonomy",
                             "ui": {
+                                "detail": "taxonomy_item",
+                                "edit": "taxonomy_item",
                                 "marshmallow": {
-                                    "read": false,
-                                    "write": false
+                                    "class": "nr_metadata.data.services.records.ui_schema.PublishersItemUISchema",
+                                    "generate": true,
+                                    "unknown": "INCLUDE"
                                 }
-                            }
+                            },
+                            "vocabulary-type": "institutions"
                         },
-                        "label.cs": "Vydavatel\u00e9",
-                        "label.en": "Publishers",
+                        "marshmallow": {
+                            "validators": [
+                                "ma.validate.Length(min=1)"
+                            ]
+                        },
+                        "minItems": 1,
                         "type": "array"
                     },
                     "relatedItems": {
                         "items": {
                             "marshmallow": {
-                                "base-classes": [
-                                    "nr_metadata.common.services.records.schema_datatypes.NRRelatedItemSchema"
-                                ],
-                                "class": "nr_metadata.documents.services.records.schema.RelatedItemsItemSchema",
-                                "generate": true,
-                                "imports": [
-                                    {
-                                        "alias": "nr_metadata.common.services.records.schema_datatypes",
-                                        "import": "nr_metadata.common.services.records.schema_datatypes"
-                                    }
-                                ],
-                                "read": false,
-                                "write": false
+                                "class": "nr_metadata.common.services.records.schema_datatypes.NRRelatedItemSchema",
+                                "generate": false
                             },
                             "properties": {
                                 "itemContributors": {
                                     "items": {
+                                        "discriminator": "nameType",
+                                        "hint.cs": "Jako tv\u016frce je mo\u017en\u00e9 ozna\u010dit osobu nebo instituci.",
+                                        "hint.en": "It is possible to designate a person or an institution as the creator/contributor.",
                                         "marshmallow": {
-                                            "base-classes": [
-                                                "nr_metadata.common.services.records.schema_datatypes.NRRelatedItemContributorSchema"
-                                            ],
-                                            "class": "nr_metadata.documents.services.records.schema.ItemContributorsItemSchema",
+                                            "class": "nr_metadata.common.services.records.schema_datatypes.NRRelatedItemContributorSchema",
                                             "generate": true,
-                                            "imports": [
-                                                {
-                                                    "alias": "nr_metadata.common.services.records.schema_datatypes",
-                                                    "import": "nr_metadata.common.services.records.schema_datatypes"
-                                                }
-                                            ]
+                                            "read": false,
+                                            "write": false
                                         },
                                         "properties": {
                                             "affiliations": {
                                                 "items": {
                                                     "facets": {
                                                         "args": [
                                                             "vocabulary='institutions'"
@@ -2757,14 +3522,21 @@
                                                             "import": "invenio_vocabularies.records.api.Vocabulary"
                                                         }
                                                     ],
                                                     "keys": [
                                                         "id",
                                                         "title",
                                                         {
+                                                            "key": "props.ror",
+                                                            "model": {
+                                                                "type": "keyword"
+                                                            },
+                                                            "target": "ror"
+                                                        },
+                                                        {
                                                             "key": "hierarchy",
                                                             "model": {
                                                                 "marshmallow": {
                                                                     "class": "oarepo_vocabularies.services.schema.HierarchySchema",
                                                                     "generate": false,
                                                                     "imports": [
                                                                         {
@@ -2796,25 +3568,25 @@
                                                                             "additionalProperties": {
                                                                                 "type": "string"
                                                                             },
                                                                             "mapping": {
                                                                                 "dynamic": true
                                                                             },
                                                                             "marshmallow": {
-                                                                                "class": "nr_metadata.documents.services.records.schema.TitleItemSchema",
+                                                                                "class": "nr_metadata.data.services.records.schema.TitleItemSchema",
                                                                                 "field": "i18n_strings",
                                                                                 "generate": false
                                                                             },
                                                                             "propertyNames": {
                                                                                 "pattern": "^[a-z]{2}$"
                                                                             },
                                                                             "type": "object",
                                                                             "ui": {
                                                                                 "marshmallow": {
-                                                                                    "class": "nr_metadata.documents.services.records.ui_schema.TitleItemUISchema",
+                                                                                    "class": "nr_metadata.data.services.records.ui_schema.TitleItemUISchema",
                                                                                     "field": "i18n_strings",
                                                                                     "generate": false
                                                                                 }
                                                                             }
                                                                         },
                                                                         "type": "array"
                                                                     }
@@ -2834,25 +3606,16 @@
                                                             },
                                                             "target": "hierarchy"
                                                         }
                                                     ],
                                                     "label.cs": "Afiliace",
                                                     "label.en": "Affiliation",
                                                     "marshmallow": {
-                                                        "base-classes": [
-                                                            "nr_metadata.common.services.records.schema_datatypes.NRAffiliationVocabularySchema"
-                                                        ],
-                                                        "class": "nr_metadata.documents.services.records.schema.AffiliationsItemSchema",
+                                                        "class": "nr_metadata.common.services.records.schema_datatypes.NRAffiliationVocabularySchema",
                                                         "generate": false,
-                                                        "imports": [
-                                                            {
-                                                                "alias": "nr_metadata.common.services.records.schema_datatypes",
-                                                                "import": "nr_metadata.common.services.records.schema_datatypes"
-                                                            }
-                                                        ],
                                                         "read": false,
                                                         "unknown": "INCLUDE",
                                                         "write": false
                                                     },
                                                     "model": "vocabularies",
                                                     "pid-field": "Vocabulary.pid.with_type_ctx(\"institutions\")",
                                                     "properties": {
@@ -2906,25 +3669,25 @@
                                                                         "additionalProperties": {
                                                                             "type": "string"
                                                                         },
                                                                         "mapping": {
                                                                             "dynamic": true
                                                                         },
                                                                         "marshmallow": {
-                                                                            "class": "nr_metadata.documents.services.records.schema.TitleItemSchema",
+                                                                            "class": "nr_metadata.data.services.records.schema.TitleItemSchema",
                                                                             "field": "i18n_strings",
                                                                             "generate": false
                                                                         },
                                                                         "propertyNames": {
                                                                             "pattern": "^[a-z]{2}$"
                                                                         },
                                                                         "type": "object",
                                                                         "ui": {
                                                                             "marshmallow": {
-                                                                                "class": "nr_metadata.documents.services.records.ui_schema.TitleItemUISchema",
+                                                                                "class": "nr_metadata.data.services.records.ui_schema.TitleItemUISchema",
                                                                                 "field": "i18n_strings",
                                                                                 "generate": false
                                                                             }
                                                                         }
                                                                     },
                                                                     "type": "array"
                                                                 }
@@ -2963,14 +3726,17 @@
                                                                 "marshmallow": {
                                                                     "field-class": "marshmallow.fields.String",
                                                                     "imports": [],
                                                                     "validators": []
                                                                 }
                                                             }
                                                         },
+                                                        "ror": {
+                                                            "type": "keyword"
+                                                        },
                                                         "title": {
                                                             "additionalProperties": {
                                                                 "type": "string"
                                                             },
                                                             "mapping": {
                                                                 "dynamic": true,
                                                                 "properties": {
@@ -3003,52 +3769,30 @@
                                                         "faker": "company"
                                                     },
                                                     "type": "taxonomy",
                                                     "ui": {
                                                         "detail": "taxonomy_item",
                                                         "edit": "taxonomy_item",
                                                         "marshmallow": {
-                                                            "base-classes": [
-                                                                "nr_metadata.common.services.records.ui_schema_datatypes.NRAffiliationVocabularyUISchema"
-                                                            ],
-                                                            "class": "nr_metadata.documents.services.records.ui_schema.AffiliationsItemUISchema",
+                                                            "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRAffiliationVocabularyUISchema",
                                                             "generate": false,
-                                                            "imports": [
-                                                                {
-                                                                    "alias": "nr_metadata.common.services.records.ui_schema_datatypes",
-                                                                    "import": "nr_metadata.common.services.records.ui_schema_datatypes"
-                                                                }
-                                                            ],
                                                             "read": false,
                                                             "unknown": "INCLUDE",
                                                             "write": false
                                                         }
                                                     },
                                                     "vocabulary-type": "institutions"
                                                 },
-                                                "label.cs": "Afiliace",
-                                                "label.en": "Affiliation",
                                                 "type": "array"
                                             },
                                             "authorityIdentifiers": {
                                                 "items": {
                                                     "marshmallow": {
-                                                        "base-classes": [
-                                                            "nr_metadata.schema.identifiers.NRAuthorityIdentifierSchema"
-                                                        ],
-                                                        "class": "nr_metadata.documents.services.records.schema.AuthorityIdentifiersItemSchema",
-                                                        "generate": false,
-                                                        "imports": [
-                                                            {
-                                                                "alias": "nr_metadata.schema.identifiers",
-                                                                "import": "nr_metadata.schema.identifiers"
-                                                            }
-                                                        ],
-                                                        "read": false,
-                                                        "write": false
+                                                        "class": "nr_metadata.schema.identifiers.NROrganizationIdentifierSchema",
+                                                        "generate": false
                                                     },
                                                     "properties": {
                                                         "identifier": {
                                                             "i18n.key": "identifier",
                                                             "label.cs": "Identifik\u00e1tor",
                                                             "label.en": "Identifier",
                                                             "marshmallow": {
@@ -3065,20 +3809,14 @@
                                                                     "read": false,
                                                                     "write": false
                                                                 }
                                                             }
                                                         },
                                                         "scheme": {
                                                             "enum": [
-                                                                "orcid",
-                                                                "scopusID",
-                                                                "researcherID",
-                                                                "czenasAutID",
-                                                                "vedidk",
-                                                                "institutionalID",
                                                                 "ISNI",
                                                                 "ROR",
                                                                 "ICO",
                                                                 "DOI"
                                                             ],
                                                             "hint.cs": "Doporu\u010dujeme zadat alespo\u0148 jeden z typ\u016f identifik\u00e1tor\u016f.\nPokud pot\u0159ebujete roz\u0161\u00ed\u0159it nab\u00eddku typ\u016f identifik\u00e1tor\u016f, kontaktujte n\u00e1s na support@narodni-repozitar.cz.\n",
                                                             "hint.en": "We recommend providing at least one of the identifier types.\nIf you need to expand the range of identifier types, contact us at support@narodni-repozitar.cz.\n",
@@ -3097,113 +3835,49 @@
                                                                     "write": false
                                                                 }
                                                             }
                                                         }
                                                     },
                                                     "type": "object",
                                                     "ui": {
-                                                        "detail": "nr_authority_identifier",
+                                                        "detail": "nr_organization_identifier",
                                                         "marshmallow": {
-                                                            "base-classes": [
-                                                                "nr_metadata.ui_schema.identifiers.NRAuthorityIdentifierUISchema"
-                                                            ],
-                                                            "class": "nr_metadata.documents.services.records.ui_schema.AuthorityIdentifiersItemUISchema",
-                                                            "generate": false,
-                                                            "imports": [
-                                                                {
-                                                                    "alias": "nr_metadata.ui_schema.identifiers",
-                                                                    "import": "nr_metadata.ui_schema.identifiers"
-                                                                }
-                                                            ],
-                                                            "read": false,
-                                                            "write": false
+                                                            "class": "nr_metadata.ui_schema.identifiers.NROrganizationIdentifierUISchema",
+                                                            "generate": false
                                                         }
                                                     }
                                                 },
                                                 "type": "array"
                                             },
-                                            "fullName": {
-                                                "label.cs": "Jm\u00e9no autora",
-                                                "label.en": "Author name",
-                                                "marshmallow": {
-                                                    "read": false,
-                                                    "write": false
-                                                },
-                                                "required": true,
-                                                "sample": {
-                                                    "faker": "name"
-                                                },
-                                                "type": "keyword",
-                                                "ui": {
-                                                    "marshmallow": {
-                                                        "read": false,
-                                                        "write": false
-                                                    }
-                                                }
-                                            },
-                                            "nameType": {
-                                                "enum": [
-                                                    "Organizational",
-                                                    "Personal"
-                                                ],
-                                                "hint.cs": "Jako tv\u016frce je mo\u017en\u00e9 ozna\u010dit osobu nebo instituci.",
-                                                "hint.en": "It is possible to designate a person or an institution as the creator/contributor.",
-                                                "label.cs": "Typ",
-                                                "label.en": "Type",
-                                                "marshmallow": {
-                                                    "read": false,
-                                                    "write": false
-                                                },
-                                                "sample": [
-                                                    "Organizational",
-                                                    "Personal"
-                                                ],
-                                                "type": "keyword",
-                                                "ui": {
-                                                    "marshmallow": {
-                                                        "read": false,
-                                                        "write": false
-                                                    }
-                                                }
-                                            },
-                                            "role": {
+                                            "contributorType": {
                                                 "facets": {
                                                     "args": [
-                                                        "vocabulary='contributor-roles'"
+                                                        "vocabulary='contributor-types'"
                                                     ]
                                                 },
                                                 "imports": [
                                                     {
                                                         "import": "invenio_vocabularies.records.api.Vocabulary"
                                                     }
                                                 ],
                                                 "keys": [
                                                     "id",
                                                     "title"
                                                 ],
-                                                "label.cs": "Role p\u0159isp\u011bvatele",
-                                                "label.en": "Contributor's role",
+                                                "label.cs": "Typ p\u0159isp\u011bvatele",
+                                                "label.en": "Contributor's type",
                                                 "marshmallow": {
-                                                    "base-classes": [
-                                                        "nr_metadata.common.services.records.schema_datatypes.NRAuthorityRoleVocabularySchema"
-                                                    ],
-                                                    "class": "nr_metadata.documents.services.records.schema.RoleSchema",
+                                                    "class": "nr_metadata.common.services.records.schema_datatypes.NRContributorTypeVocabularySchema",
                                                     "generate": false,
-                                                    "imports": [
-                                                        {
-                                                            "alias": "nr_metadata.common.services.records.schema_datatypes",
-                                                            "import": "nr_metadata.common.services.records.schema_datatypes"
-                                                        }
-                                                    ],
                                                     "read": false,
                                                     "unknown": "INCLUDE",
                                                     "write": false
                                                 },
                                                 "model": "vocabularies",
-                                                "pid-field": "Vocabulary.pid.with_type_ctx(\"contributor-roles\")",
+                                                "pid-field": "Vocabulary.pid.with_type_ctx(\"contributor-types\")",
                                                 "properties": {
                                                     "@v": {
                                                         "facets": {
                                                             "facet": false
                                                         },
                                                         "marshmallow": {
                                                             "field-class": "marshmallow.fields.String",
@@ -3275,69 +3949,606 @@
                                                     }
                                                 },
                                                 "type": "vocabulary",
                                                 "ui": {
                                                     "detail": "vocabulary_item",
                                                     "edit": "vocabulary_item",
                                                     "marshmallow": {
+                                                        "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRContributorTypeVocabularyUISchema",
+                                                        "generate": false,
+                                                        "read": false,
+                                                        "unknown": "INCLUDE",
+                                                        "write": false
+                                                    }
+                                                },
+                                                "vocabulary-type": "contributor-types"
+                                            },
+                                            "familyName": {
+                                                "marshmallow": {
+                                                    "read": false,
+                                                    "write": false
+                                                },
+                                                "type": "keyword",
+                                                "ui": {
+                                                    "marshmallow": {
+                                                        "read": false,
+                                                        "write": false
+                                                    }
+                                                }
+                                            },
+                                            "fullName": {
+                                                "label.cs": "Jm\u00e9no autora",
+                                                "label.en": "Author name",
+                                                "marshmallow": {
+                                                    "read": false,
+                                                    "write": false
+                                                },
+                                                "required": true,
+                                                "sample": {
+                                                    "faker": "name"
+                                                },
+                                                "type": "keyword",
+                                                "ui": {
+                                                    "marshmallow": {
+                                                        "read": false,
+                                                        "write": false
+                                                    }
+                                                }
+                                            },
+                                            "givenName": {
+                                                "marshmallow": {
+                                                    "read": false,
+                                                    "write": false
+                                                },
+                                                "type": "keyword",
+                                                "ui": {
+                                                    "marshmallow": {
+                                                        "read": false,
+                                                        "write": false
+                                                    }
+                                                }
+                                            },
+                                            "nameType": {
+                                                "enum": [
+                                                    "Organizational"
+                                                ],
+                                                "label.cs": "Typ",
+                                                "label.en": "Type",
+                                                "marshmallow": {
+                                                    "read": false,
+                                                    "write": false
+                                                },
+                                                "sample": [
+                                                    "Organizational"
+                                                ],
+                                                "type": "keyword",
+                                                "ui": {
+                                                    "marshmallow": {
+                                                        "read": false,
+                                                        "write": false
+                                                    }
+                                                }
+                                            }
+                                        },
+                                        "schemas": {
+                                            "Organizational": {
+                                                "marshmallow": {
+                                                    "base-classes": [
+                                                        "nr_metadata.common.services.records.schema_datatypes.NROrganizationSchema"
+                                                    ],
+                                                    "class": "nr_metadata.common.services.records.schema_datatypes.NRRelatedItemContributorOrganizationSchema",
+                                                    "generate": true
+                                                },
+                                                "properties": {
+                                                    "authorityIdentifiers": {
+                                                        "items": {
+                                                            "marshmallow": {
+                                                                "class": "nr_metadata.schema.identifiers.NROrganizationIdentifierSchema",
+                                                                "generate": false
+                                                            },
+                                                            "properties": {
+                                                                "identifier": {
+                                                                    "i18n.key": "identifier",
+                                                                    "label.cs": "Identifik\u00e1tor",
+                                                                    "label.en": "Identifier",
+                                                                    "marshmallow": {
+                                                                        "read": false,
+                                                                        "write": false
+                                                                    },
+                                                                    "required": true,
+                                                                    "sample": {
+                                                                        "faker": "isbn13"
+                                                                    },
+                                                                    "type": "keyword",
+                                                                    "ui": {
+                                                                        "marshmallow": {
+                                                                            "read": false,
+                                                                            "write": false
+                                                                        }
+                                                                    }
+                                                                },
+                                                                "scheme": {
+                                                                    "enum": [
+                                                                        "ISNI",
+                                                                        "ROR",
+                                                                        "ICO",
+                                                                        "DOI"
+                                                                    ],
+                                                                    "hint.cs": "Doporu\u010dujeme zadat alespo\u0148 jeden z typ\u016f identifik\u00e1tor\u016f.\nPokud pot\u0159ebujete roz\u0161\u00ed\u0159it nab\u00eddku typ\u016f identifik\u00e1tor\u016f, kontaktujte n\u00e1s na support@narodni-repozitar.cz.\n",
+                                                                    "hint.en": "We recommend providing at least one of the identifier types.\nIf you need to expand the range of identifier types, contact us at support@narodni-repozitar.cz.\n",
+                                                                    "i18n.key": "identifier_type",
+                                                                    "label.cs": "Typ identifik\u00e1toru",
+                                                                    "label.en": "Identifier type",
+                                                                    "marshmallow": {
+                                                                        "read": false,
+                                                                        "write": false
+                                                                    },
+                                                                    "required": true,
+                                                                    "type": "keyword",
+                                                                    "ui": {
+                                                                        "marshmallow": {
+                                                                            "read": false,
+                                                                            "write": false
+                                                                        }
+                                                                    }
+                                                                }
+                                                            },
+                                                            "type": "object",
+                                                            "ui": {
+                                                                "detail": "nr_organization_identifier",
+                                                                "marshmallow": {
+                                                                    "class": "nr_metadata.ui_schema.identifiers.NROrganizationIdentifierUISchema",
+                                                                    "generate": false
+                                                                }
+                                                            }
+                                                        },
+                                                        "type": "array"
+                                                    },
+                                                    "contributorType": {
+                                                        "facets": {
+                                                            "args": [
+                                                                "vocabulary='contributor-types'"
+                                                            ]
+                                                        },
+                                                        "imports": [
+                                                            {
+                                                                "import": "invenio_vocabularies.records.api.Vocabulary"
+                                                            }
+                                                        ],
+                                                        "keys": [
+                                                            "id",
+                                                            "title"
+                                                        ],
+                                                        "label.cs": "Typ p\u0159isp\u011bvatele",
+                                                        "label.en": "Contributor's type",
+                                                        "marshmallow": {
+                                                            "class": "nr_metadata.common.services.records.schema_datatypes.NRContributorTypeVocabularySchema",
+                                                            "generate": false,
+                                                            "read": false,
+                                                            "unknown": "INCLUDE",
+                                                            "write": false
+                                                        },
+                                                        "model": "vocabularies",
+                                                        "pid-field": "Vocabulary.pid.with_type_ctx(\"contributor-types\")",
+                                                        "properties": {},
+                                                        "type": "vocabulary",
+                                                        "ui": {
+                                                            "detail": "vocabulary_item",
+                                                            "edit": "vocabulary_item",
+                                                            "marshmallow": {
+                                                                "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRContributorTypeVocabularyUISchema",
+                                                                "generate": false,
+                                                                "read": false,
+                                                                "unknown": "INCLUDE",
+                                                                "write": false
+                                                            }
+                                                        },
+                                                        "vocabulary-type": "contributor-types"
+                                                    },
+                                                    "fullName": {
+                                                        "label.cs": "Jm\u00e9no autora",
+                                                        "label.en": "Author name",
+                                                        "marshmallow": {
+                                                            "read": false,
+                                                            "write": false
+                                                        },
+                                                        "required": true,
+                                                        "sample": {
+                                                            "faker": "name"
+                                                        },
+                                                        "type": "keyword",
+                                                        "ui": {
+                                                            "marshmallow": {
+                                                                "read": false,
+                                                                "write": false
+                                                            }
+                                                        }
+                                                    },
+                                                    "nameType": {
+                                                        "enum": [
+                                                            "Organizational"
+                                                        ],
+                                                        "label.cs": "Typ",
+                                                        "label.en": "Type",
+                                                        "marshmallow": {
+                                                            "read": false,
+                                                            "write": false
+                                                        },
+                                                        "sample": [
+                                                            "Organizational"
+                                                        ],
+                                                        "type": "keyword",
+                                                        "ui": {
+                                                            "marshmallow": {
+                                                                "read": false,
+                                                                "write": false
+                                                            }
+                                                        }
+                                                    }
+                                                },
+                                                "type": "object",
+                                                "ui": {
+                                                    "detail": "nr_contributor_organization",
+                                                    "marshmallow": {
                                                         "base-classes": [
-                                                            "nr_metadata.common.services.records.ui_schema_datatypes.NRAuthorityRoleVocabularyUISchema"
+                                                            "nr_metadata.common.services.records.ui_schema_datatypes.NROrganizationUISchema"
                                                         ],
-                                                        "class": "nr_metadata.documents.services.records.ui_schema.RoleUISchema",
-                                                        "generate": false,
+                                                        "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRRelatedItemContributorOrganizationUISchema",
+                                                        "generate": true
+                                                    }
+                                                }
+                                            },
+                                            "Personal": {
+                                                "marshmallow": {
+                                                    "base-classes": [
+                                                        "nr_metadata.common.services.records.schema_datatypes.NRPersonSchema"
+                                                    ],
+                                                    "class": "nr_metadata.common.services.records.schema_datatypes.NRRelatedItemContributorPersonSchema",
+                                                    "generate": true
+                                                },
+                                                "properties": {
+                                                    "affiliations": {
+                                                        "items": {
+                                                            "facets": {
+                                                                "args": [
+                                                                    "vocabulary='institutions'"
+                                                                ]
+                                                            },
+                                                            "hint.cs": "Uve\u010fte instituci/instituce, pod jej\u00ed\u017e z\u00e1\u0161titou jste se na tvorb\u011b objektu pod\u00edleli.",
+                                                            "imports": [
+                                                                {
+                                                                    "import": "invenio_vocabularies.records.api.Vocabulary"
+                                                                }
+                                                            ],
+                                                            "keys": [
+                                                                "id",
+                                                                "title",
+                                                                {
+                                                                    "key": "props.ror",
+                                                                    "model": {
+                                                                        "type": "keyword"
+                                                                    },
+                                                                    "target": "ror"
+                                                                },
+                                                                {
+                                                                    "key": "hierarchy",
+                                                                    "model": {
+                                                                        "marshmallow": {
+                                                                            "class": "oarepo_vocabularies.services.schema.HierarchySchema",
+                                                                            "generate": false,
+                                                                            "imports": [
+                                                                                {
+                                                                                    "import": "oarepo_vocabularies.services.schema.HierarchySchema"
+                                                                                }
+                                                                            ]
+                                                                        },
+                                                                        "properties": {
+                                                                            "ancestors": {
+                                                                                "items": {
+                                                                                    "type": "keyword"
+                                                                                },
+                                                                                "type": "array"
+                                                                            },
+                                                                            "ancestors_or_self": {
+                                                                                "items": {
+                                                                                    "type": "keyword"
+                                                                                },
+                                                                                "type": "array"
+                                                                            },
+                                                                            "level": {
+                                                                                "type": "integer"
+                                                                            },
+                                                                            "parent": {
+                                                                                "type": "keyword"
+                                                                            },
+                                                                            "title": {
+                                                                                "items": {
+                                                                                    "additionalProperties": {
+                                                                                        "type": "string"
+                                                                                    },
+                                                                                    "mapping": {
+                                                                                        "dynamic": true
+                                                                                    },
+                                                                                    "marshmallow": {
+                                                                                        "class": "nr_metadata.data.services.records.schema.TitleItemSchema",
+                                                                                        "field": "i18n_strings",
+                                                                                        "generate": false
+                                                                                    },
+                                                                                    "propertyNames": {
+                                                                                        "pattern": "^[a-z]{2}$"
+                                                                                    },
+                                                                                    "type": "object",
+                                                                                    "ui": {
+                                                                                        "marshmallow": {
+                                                                                            "class": "nr_metadata.data.services.records.ui_schema.TitleItemUISchema",
+                                                                                            "field": "i18n_strings",
+                                                                                            "generate": false
+                                                                                        }
+                                                                                    }
+                                                                                },
+                                                                                "type": "array"
+                                                                            }
+                                                                        },
+                                                                        "type": "object",
+                                                                        "ui": {
+                                                                            "marshmallow": {
+                                                                                "class": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema",
+                                                                                "generate": false,
+                                                                                "imports": [
+                                                                                    {
+                                                                                        "import": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema"
+                                                                                    }
+                                                                                ]
+                                                                            }
+                                                                        }
+                                                                    },
+                                                                    "target": "hierarchy"
+                                                                }
+                                                            ],
+                                                            "label.cs": "Afiliace",
+                                                            "label.en": "Affiliation",
+                                                            "marshmallow": {
+                                                                "class": "nr_metadata.common.services.records.schema_datatypes.NRAffiliationVocabularySchema",
+                                                                "generate": false,
+                                                                "read": false,
+                                                                "unknown": "INCLUDE",
+                                                                "write": false
+                                                            },
+                                                            "model": "vocabularies",
+                                                            "pid-field": "Vocabulary.pid.with_type_ctx(\"institutions\")",
+                                                            "properties": {},
+                                                            "sample": {
+                                                                "faker": "company"
+                                                            },
+                                                            "type": "taxonomy",
+                                                            "ui": {
+                                                                "detail": "taxonomy_item",
+                                                                "edit": "taxonomy_item",
+                                                                "marshmallow": {
+                                                                    "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRAffiliationVocabularyUISchema",
+                                                                    "generate": false,
+                                                                    "read": false,
+                                                                    "unknown": "INCLUDE",
+                                                                    "write": false
+                                                                }
+                                                            },
+                                                            "vocabulary-type": "institutions"
+                                                        },
+                                                        "type": "array"
+                                                    },
+                                                    "authorityIdentifiers": {
+                                                        "items": {
+                                                            "marshmallow": {
+                                                                "class": "nr_metadata.schema.identifiers.NRPersonIdentifierSchema",
+                                                                "generate": false
+                                                            },
+                                                            "properties": {
+                                                                "identifier": {
+                                                                    "i18n.key": "identifier",
+                                                                    "label.cs": "Identifik\u00e1tor",
+                                                                    "label.en": "Identifier",
+                                                                    "marshmallow": {
+                                                                        "read": false,
+                                                                        "write": false
+                                                                    },
+                                                                    "required": true,
+                                                                    "sample": {
+                                                                        "faker": "isbn13"
+                                                                    },
+                                                                    "type": "keyword",
+                                                                    "ui": {
+                                                                        "marshmallow": {
+                                                                            "read": false,
+                                                                            "write": false
+                                                                        }
+                                                                    }
+                                                                },
+                                                                "scheme": {
+                                                                    "enum": [
+                                                                        "orcid",
+                                                                        "scopusID",
+                                                                        "researcherID",
+                                                                        "czenasAutID",
+                                                                        "vedidk",
+                                                                        "institutionalID",
+                                                                        "ISNI"
+                                                                    ],
+                                                                    "hint.cs": "Doporu\u010dujeme zadat alespo\u0148 jeden z typ\u016f identifik\u00e1tor\u016f.\nPokud pot\u0159ebujete roz\u0161\u00ed\u0159it nab\u00eddku typ\u016f identifik\u00e1tor\u016f, kontaktujte n\u00e1s na support@narodni-repozitar.cz.\n",
+                                                                    "hint.en": "We recommend providing at least one of the identifier types.\nIf you need to expand the range of identifier types, contact us at support@narodni-repozitar.cz.\n",
+                                                                    "i18n.key": "identifier_type",
+                                                                    "label.cs": "Typ identifik\u00e1toru",
+                                                                    "label.en": "Identifier type",
+                                                                    "marshmallow": {
+                                                                        "read": false,
+                                                                        "write": false
+                                                                    },
+                                                                    "required": true,
+                                                                    "type": "keyword",
+                                                                    "ui": {
+                                                                        "marshmallow": {
+                                                                            "read": false,
+                                                                            "write": false
+                                                                        }
+                                                                    }
+                                                                }
+                                                            },
+                                                            "type": "object",
+                                                            "ui": {
+                                                                "detail": "nr_person_identifier",
+                                                                "marshmallow": {
+                                                                    "class": "nr_metadata.ui_schema.identifiers.NRPersonIdentifierUISchema",
+                                                                    "generate": false
+                                                                }
+                                                            }
+                                                        },
+                                                        "type": "array"
+                                                    },
+                                                    "contributorType": {
+                                                        "facets": {
+                                                            "args": [
+                                                                "vocabulary='contributor-types'"
+                                                            ]
+                                                        },
                                                         "imports": [
                                                             {
-                                                                "alias": "nr_metadata.common.services.records.ui_schema_datatypes",
-                                                                "import": "nr_metadata.common.services.records.ui_schema_datatypes"
+                                                                "import": "invenio_vocabularies.records.api.Vocabulary"
                                                             }
                                                         ],
-                                                        "read": false,
-                                                        "unknown": "INCLUDE",
-                                                        "write": false
+                                                        "keys": [
+                                                            "id",
+                                                            "title"
+                                                        ],
+                                                        "label.cs": "Typ p\u0159isp\u011bvatele",
+                                                        "label.en": "Contributor's type",
+                                                        "marshmallow": {
+                                                            "class": "nr_metadata.common.services.records.schema_datatypes.NRContributorTypeVocabularySchema",
+                                                            "generate": false,
+                                                            "read": false,
+                                                            "unknown": "INCLUDE",
+                                                            "write": false
+                                                        },
+                                                        "model": "vocabularies",
+                                                        "pid-field": "Vocabulary.pid.with_type_ctx(\"contributor-types\")",
+                                                        "properties": {},
+                                                        "type": "vocabulary",
+                                                        "ui": {
+                                                            "detail": "vocabulary_item",
+                                                            "edit": "vocabulary_item",
+                                                            "marshmallow": {
+                                                                "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRContributorTypeVocabularyUISchema",
+                                                                "generate": false,
+                                                                "read": false,
+                                                                "unknown": "INCLUDE",
+                                                                "write": false
+                                                            }
+                                                        },
+                                                        "vocabulary-type": "contributor-types"
+                                                    },
+                                                    "familyName": {
+                                                        "marshmallow": {
+                                                            "read": false,
+                                                            "write": false
+                                                        },
+                                                        "type": "keyword",
+                                                        "ui": {
+                                                            "marshmallow": {
+                                                                "read": false,
+                                                                "write": false
+                                                            }
+                                                        }
+                                                    },
+                                                    "fullName": {
+                                                        "label.cs": "Jm\u00e9no autora",
+                                                        "label.en": "Author name",
+                                                        "marshmallow": {
+                                                            "read": false,
+                                                            "write": false
+                                                        },
+                                                        "required": true,
+                                                        "sample": {
+                                                            "faker": "name"
+                                                        },
+                                                        "type": "keyword",
+                                                        "ui": {
+                                                            "marshmallow": {
+                                                                "read": false,
+                                                                "write": false
+                                                            }
+                                                        }
+                                                    },
+                                                    "givenName": {
+                                                        "marshmallow": {
+                                                            "read": false,
+                                                            "write": false
+                                                        },
+                                                        "type": "keyword",
+                                                        "ui": {
+                                                            "marshmallow": {
+                                                                "read": false,
+                                                                "write": false
+                                                            }
+                                                        }
+                                                    },
+                                                    "nameType": {
+                                                        "enum": [
+                                                            "Personal"
+                                                        ],
+                                                        "label.cs": "Typ",
+                                                        "label.en": "Type",
+                                                        "marshmallow": {
+                                                            "read": false,
+                                                            "write": false
+                                                        },
+                                                        "type": "keyword",
+                                                        "ui": {
+                                                            "marshmallow": {
+                                                                "read": false,
+                                                                "write": false
+                                                            }
+                                                        }
                                                     }
                                                 },
-                                                "vocabulary-type": "contributor-roles"
+                                                "type": "object",
+                                                "ui": {
+                                                    "detail": "nr_contributor_person",
+                                                    "marshmallow": {
+                                                        "base-classes": [
+                                                            "nr_metadata.common.services.records.ui_schema_datatypes.NRPersonUISchema"
+                                                        ],
+                                                        "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRRelatedItemContributorPersonUISchema",
+                                                        "generate": true
+                                                    }
+                                                }
                                             }
                                         },
-                                        "type": "object",
+                                        "type": "polymorphic",
                                         "ui": {
                                             "detail": "contributor",
                                             "marshmallow": {
-                                                "base-classes": [
-                                                    "nr_metadata.common.services.records.ui_schema_datatypes.NRRelatedItemContributorUISchema"
-                                                ],
-                                                "class": "nr_metadata.documents.services.records.ui_schema.ItemContributorsItemUISchema",
+                                                "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRRelatedItemContributorUISchema",
                                                 "generate": true,
-                                                "imports": [
-                                                    {
-                                                        "alias": "nr_metadata.common.services.records.ui_schema_datatypes",
-                                                        "import": "nr_metadata.common.services.records.ui_schema_datatypes"
-                                                    }
-                                                ]
+                                                "read": false,
+                                                "write": false
                                             }
                                         }
                                     },
                                     "label.cs": "P\u0159isp\u011bvatel\u00e9",
                                     "label.en": "Contributors",
                                     "type": "array"
                                 },
                                 "itemCreators": {
                                     "items": {
+                                        "discriminator": "nameType",
+                                        "hint.cs": "Jako tv\u016frce je mo\u017en\u00e9 ozna\u010dit osobu nebo instituci.",
+                                        "hint.en": "It is possible to designate a person or an institution as the creator/contributor.",
                                         "marshmallow": {
-                                            "base-classes": [
-                                                "nr_metadata.common.services.records.schema_datatypes.NRRelatedItemCreatorSchema"
-                                            ],
-                                            "class": "nr_metadata.documents.services.records.schema.ItemCreatorsItemSchema",
+                                            "class": "nr_metadata.common.services.records.schema_datatypes.NRRelatedItemCreatorSchema",
                                             "generate": true,
-                                            "imports": [
-                                                {
-                                                    "alias": "nr_metadata.common.services.records.schema_datatypes",
-                                                    "import": "nr_metadata.common.services.records.schema_datatypes"
-                                                }
-                                            ]
+                                            "read": false,
+                                            "write": false
                                         },
                                         "properties": {
                                             "affiliations": {
                                                 "items": {
                                                     "facets": {
                                                         "args": [
                                                             "vocabulary='institutions'"
@@ -3349,14 +4560,21 @@
                                                             "import": "invenio_vocabularies.records.api.Vocabulary"
                                                         }
                                                     ],
                                                     "keys": [
                                                         "id",
                                                         "title",
                                                         {
+                                                            "key": "props.ror",
+                                                            "model": {
+                                                                "type": "keyword"
+                                                            },
+                                                            "target": "ror"
+                                                        },
+                                                        {
                                                             "key": "hierarchy",
                                                             "model": {
                                                                 "marshmallow": {
                                                                     "class": "oarepo_vocabularies.services.schema.HierarchySchema",
                                                                     "generate": false,
                                                                     "imports": [
                                                                         {
@@ -3388,25 +4606,25 @@
                                                                             "additionalProperties": {
                                                                                 "type": "string"
                                                                             },
                                                                             "mapping": {
                                                                                 "dynamic": true
                                                                             },
                                                                             "marshmallow": {
-                                                                                "class": "nr_metadata.documents.services.records.schema.TitleItemSchema",
+                                                                                "class": "nr_metadata.data.services.records.schema.TitleItemSchema",
                                                                                 "field": "i18n_strings",
                                                                                 "generate": false
                                                                             },
                                                                             "propertyNames": {
                                                                                 "pattern": "^[a-z]{2}$"
                                                                             },
                                                                             "type": "object",
                                                                             "ui": {
                                                                                 "marshmallow": {
-                                                                                    "class": "nr_metadata.documents.services.records.ui_schema.TitleItemUISchema",
+                                                                                    "class": "nr_metadata.data.services.records.ui_schema.TitleItemUISchema",
                                                                                     "field": "i18n_strings",
                                                                                     "generate": false
                                                                                 }
                                                                             }
                                                                         },
                                                                         "type": "array"
                                                                     }
@@ -3426,25 +4644,16 @@
                                                             },
                                                             "target": "hierarchy"
                                                         }
                                                     ],
                                                     "label.cs": "Afiliace",
                                                     "label.en": "Affiliation",
                                                     "marshmallow": {
-                                                        "base-classes": [
-                                                            "nr_metadata.common.services.records.schema_datatypes.NRAffiliationVocabularySchema"
-                                                        ],
-                                                        "class": "nr_metadata.documents.services.records.schema.AffiliationsItemSchema",
+                                                        "class": "nr_metadata.common.services.records.schema_datatypes.NRAffiliationVocabularySchema",
                                                         "generate": false,
-                                                        "imports": [
-                                                            {
-                                                                "alias": "nr_metadata.common.services.records.schema_datatypes",
-                                                                "import": "nr_metadata.common.services.records.schema_datatypes"
-                                                            }
-                                                        ],
                                                         "read": false,
                                                         "unknown": "INCLUDE",
                                                         "write": false
                                                     },
                                                     "model": "vocabularies",
                                                     "pid-field": "Vocabulary.pid.with_type_ctx(\"institutions\")",
                                                     "properties": {
@@ -3498,25 +4707,25 @@
                                                                         "additionalProperties": {
                                                                             "type": "string"
                                                                         },
                                                                         "mapping": {
                                                                             "dynamic": true
                                                                         },
                                                                         "marshmallow": {
-                                                                            "class": "nr_metadata.documents.services.records.schema.TitleItemSchema",
+                                                                            "class": "nr_metadata.data.services.records.schema.TitleItemSchema",
                                                                             "field": "i18n_strings",
                                                                             "generate": false
                                                                         },
                                                                         "propertyNames": {
                                                                             "pattern": "^[a-z]{2}$"
                                                                         },
                                                                         "type": "object",
                                                                         "ui": {
                                                                             "marshmallow": {
-                                                                                "class": "nr_metadata.documents.services.records.ui_schema.TitleItemUISchema",
+                                                                                "class": "nr_metadata.data.services.records.ui_schema.TitleItemUISchema",
                                                                                 "field": "i18n_strings",
                                                                                 "generate": false
                                                                             }
                                                                         }
                                                                     },
                                                                     "type": "array"
                                                                 }
@@ -3555,14 +4764,17 @@
                                                                 "marshmallow": {
                                                                     "field-class": "marshmallow.fields.String",
                                                                     "imports": [],
                                                                     "validators": []
                                                                 }
                                                             }
                                                         },
+                                                        "ror": {
+                                                            "type": "keyword"
+                                                        },
                                                         "title": {
                                                             "additionalProperties": {
                                                                 "type": "string"
                                                             },
                                                             "mapping": {
                                                                 "dynamic": true,
                                                                 "properties": {
@@ -3595,52 +4807,30 @@
                                                         "faker": "company"
                                                     },
                                                     "type": "taxonomy",
                                                     "ui": {
                                                         "detail": "taxonomy_item",
                                                         "edit": "taxonomy_item",
                                                         "marshmallow": {
-                                                            "base-classes": [
-                                                                "nr_metadata.common.services.records.ui_schema_datatypes.NRAffiliationVocabularyUISchema"
-                                                            ],
-                                                            "class": "nr_metadata.documents.services.records.ui_schema.AffiliationsItemUISchema",
+                                                            "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRAffiliationVocabularyUISchema",
                                                             "generate": false,
-                                                            "imports": [
-                                                                {
-                                                                    "alias": "nr_metadata.common.services.records.ui_schema_datatypes",
-                                                                    "import": "nr_metadata.common.services.records.ui_schema_datatypes"
-                                                                }
-                                                            ],
                                                             "read": false,
                                                             "unknown": "INCLUDE",
                                                             "write": false
                                                         }
                                                     },
                                                     "vocabulary-type": "institutions"
                                                 },
-                                                "label.cs": "Afiliace",
-                                                "label.en": "Affiliation",
                                                 "type": "array"
                                             },
                                             "authorityIdentifiers": {
                                                 "items": {
                                                     "marshmallow": {
-                                                        "base-classes": [
-                                                            "nr_metadata.schema.identifiers.NRAuthorityIdentifierSchema"
-                                                        ],
-                                                        "class": "nr_metadata.documents.services.records.schema.AuthorityIdentifiersItemSchema",
-                                                        "generate": false,
-                                                        "imports": [
-                                                            {
-                                                                "alias": "nr_metadata.schema.identifiers",
-                                                                "import": "nr_metadata.schema.identifiers"
-                                                            }
-                                                        ],
-                                                        "read": false,
-                                                        "write": false
+                                                        "class": "nr_metadata.schema.identifiers.NROrganizationIdentifierSchema",
+                                                        "generate": false
                                                     },
                                                     "properties": {
                                                         "identifier": {
                                                             "i18n.key": "identifier",
                                                             "label.cs": "Identifik\u00e1tor",
                                                             "label.en": "Identifier",
                                                             "marshmallow": {
@@ -3657,20 +4847,14 @@
                                                                     "read": false,
                                                                     "write": false
                                                                 }
                                                             }
                                                         },
                                                         "scheme": {
                                                             "enum": [
-                                                                "orcid",
-                                                                "scopusID",
-                                                                "researcherID",
-                                                                "czenasAutID",
-                                                                "vedidk",
-                                                                "institutionalID",
                                                                 "ISNI",
                                                                 "ROR",
                                                                 "ICO",
                                                                 "DOI"
                                                             ],
                                                             "hint.cs": "Doporu\u010dujeme zadat alespo\u0148 jeden z typ\u016f identifik\u00e1tor\u016f.\nPokud pot\u0159ebujete roz\u0161\u00ed\u0159it nab\u00eddku typ\u016f identifik\u00e1tor\u016f, kontaktujte n\u00e1s na support@narodni-repozitar.cz.\n",
                                                             "hint.en": "We recommend providing at least one of the identifier types.\nIf you need to expand the range of identifier types, contact us at support@narodni-repozitar.cz.\n",
@@ -3689,34 +4873,36 @@
                                                                     "write": false
                                                                 }
                                                             }
                                                         }
                                                     },
                                                     "type": "object",
                                                     "ui": {
-                                                        "detail": "nr_authority_identifier",
+                                                        "detail": "nr_organization_identifier",
                                                         "marshmallow": {
-                                                            "base-classes": [
-                                                                "nr_metadata.ui_schema.identifiers.NRAuthorityIdentifierUISchema"
-                                                            ],
-                                                            "class": "nr_metadata.documents.services.records.ui_schema.AuthorityIdentifiersItemUISchema",
-                                                            "generate": false,
-                                                            "imports": [
-                                                                {
-                                                                    "alias": "nr_metadata.ui_schema.identifiers",
-                                                                    "import": "nr_metadata.ui_schema.identifiers"
-                                                                }
-                                                            ],
-                                                            "read": false,
-                                                            "write": false
+                                                            "class": "nr_metadata.ui_schema.identifiers.NROrganizationIdentifierUISchema",
+                                                            "generate": false
                                                         }
                                                     }
                                                 },
                                                 "type": "array"
                                             },
+                                            "familyName": {
+                                                "marshmallow": {
+                                                    "read": false,
+                                                    "write": false
+                                                },
+                                                "type": "keyword",
+                                                "ui": {
+                                                    "marshmallow": {
+                                                        "read": false,
+                                                        "write": false
+                                                    }
+                                                }
+                                            },
                                             "fullName": {
                                                 "label.cs": "Jm\u00e9no autora",
                                                 "label.en": "Author name",
                                                 "marshmallow": {
                                                     "read": false,
                                                     "write": false
                                                 },
@@ -3728,55 +4914,454 @@
                                                 "ui": {
                                                     "marshmallow": {
                                                         "read": false,
                                                         "write": false
                                                     }
                                                 }
                                             },
+                                            "givenName": {
+                                                "marshmallow": {
+                                                    "read": false,
+                                                    "write": false
+                                                },
+                                                "type": "keyword",
+                                                "ui": {
+                                                    "marshmallow": {
+                                                        "read": false,
+                                                        "write": false
+                                                    }
+                                                }
+                                            },
                                             "nameType": {
                                                 "enum": [
-                                                    "Organizational",
-                                                    "Personal"
+                                                    "Organizational"
                                                 ],
-                                                "hint.cs": "Jako tv\u016frce je mo\u017en\u00e9 ozna\u010dit osobu nebo instituci.",
-                                                "hint.en": "It is possible to designate a person or an institution as the creator/contributor.",
                                                 "label.cs": "Typ",
                                                 "label.en": "Type",
                                                 "marshmallow": {
                                                     "read": false,
                                                     "write": false
                                                 },
                                                 "sample": [
-                                                    "Organizational",
-                                                    "Personal"
+                                                    "Organizational"
                                                 ],
                                                 "type": "keyword",
                                                 "ui": {
                                                     "marshmallow": {
                                                         "read": false,
                                                         "write": false
                                                     }
                                                 }
                                             }
                                         },
-                                        "type": "object",
+                                        "schemas": {
+                                            "Organizational": {
+                                                "marshmallow": {
+                                                    "class": "nr_metadata.common.services.records.schema_datatypes.NROrganizationSchema",
+                                                    "generate": false
+                                                },
+                                                "properties": {
+                                                    "authorityIdentifiers": {
+                                                        "items": {
+                                                            "marshmallow": {
+                                                                "class": "nr_metadata.schema.identifiers.NROrganizationIdentifierSchema",
+                                                                "generate": false
+                                                            },
+                                                            "properties": {
+                                                                "identifier": {
+                                                                    "i18n.key": "identifier",
+                                                                    "label.cs": "Identifik\u00e1tor",
+                                                                    "label.en": "Identifier",
+                                                                    "marshmallow": {
+                                                                        "read": false,
+                                                                        "write": false
+                                                                    },
+                                                                    "required": true,
+                                                                    "sample": {
+                                                                        "faker": "isbn13"
+                                                                    },
+                                                                    "type": "keyword",
+                                                                    "ui": {
+                                                                        "marshmallow": {
+                                                                            "read": false,
+                                                                            "write": false
+                                                                        }
+                                                                    }
+                                                                },
+                                                                "scheme": {
+                                                                    "enum": [
+                                                                        "ISNI",
+                                                                        "ROR",
+                                                                        "ICO",
+                                                                        "DOI"
+                                                                    ],
+                                                                    "hint.cs": "Doporu\u010dujeme zadat alespo\u0148 jeden z typ\u016f identifik\u00e1tor\u016f.\nPokud pot\u0159ebujete roz\u0161\u00ed\u0159it nab\u00eddku typ\u016f identifik\u00e1tor\u016f, kontaktujte n\u00e1s na support@narodni-repozitar.cz.\n",
+                                                                    "hint.en": "We recommend providing at least one of the identifier types.\nIf you need to expand the range of identifier types, contact us at support@narodni-repozitar.cz.\n",
+                                                                    "i18n.key": "identifier_type",
+                                                                    "label.cs": "Typ identifik\u00e1toru",
+                                                                    "label.en": "Identifier type",
+                                                                    "marshmallow": {
+                                                                        "read": false,
+                                                                        "write": false
+                                                                    },
+                                                                    "required": true,
+                                                                    "type": "keyword",
+                                                                    "ui": {
+                                                                        "marshmallow": {
+                                                                            "read": false,
+                                                                            "write": false
+                                                                        }
+                                                                    }
+                                                                }
+                                                            },
+                                                            "type": "object",
+                                                            "ui": {
+                                                                "detail": "nr_organization_identifier",
+                                                                "marshmallow": {
+                                                                    "class": "nr_metadata.ui_schema.identifiers.NROrganizationIdentifierUISchema",
+                                                                    "generate": false
+                                                                }
+                                                            }
+                                                        },
+                                                        "type": "array"
+                                                    },
+                                                    "fullName": {
+                                                        "label.cs": "Jm\u00e9no autora",
+                                                        "label.en": "Author name",
+                                                        "marshmallow": {
+                                                            "read": false,
+                                                            "write": false
+                                                        },
+                                                        "required": true,
+                                                        "sample": {
+                                                            "faker": "name"
+                                                        },
+                                                        "type": "keyword",
+                                                        "ui": {
+                                                            "marshmallow": {
+                                                                "read": false,
+                                                                "write": false
+                                                            }
+                                                        }
+                                                    },
+                                                    "nameType": {
+                                                        "enum": [
+                                                            "Organizational"
+                                                        ],
+                                                        "label.cs": "Typ",
+                                                        "label.en": "Type",
+                                                        "marshmallow": {
+                                                            "read": false,
+                                                            "write": false
+                                                        },
+                                                        "sample": [
+                                                            "Organizational"
+                                                        ],
+                                                        "type": "keyword",
+                                                        "ui": {
+                                                            "marshmallow": {
+                                                                "read": false,
+                                                                "write": false
+                                                            }
+                                                        }
+                                                    }
+                                                },
+                                                "type": "object",
+                                                "ui": {
+                                                    "detail": "nr_organization",
+                                                    "marshmallow": {
+                                                        "class": "nr_metadata.common.services.records.ui_schema_datatypes.NROrganizationUISchema",
+                                                        "generate": false
+                                                    }
+                                                }
+                                            },
+                                            "Personal": {
+                                                "marshmallow": {
+                                                    "class": "nr_metadata.common.services.records.schema_datatypes.NRPersonSchema",
+                                                    "generate": false
+                                                },
+                                                "properties": {
+                                                    "affiliations": {
+                                                        "items": {
+                                                            "facets": {
+                                                                "args": [
+                                                                    "vocabulary='institutions'"
+                                                                ]
+                                                            },
+                                                            "hint.cs": "Uve\u010fte instituci/instituce, pod jej\u00ed\u017e z\u00e1\u0161titou jste se na tvorb\u011b objektu pod\u00edleli.",
+                                                            "imports": [
+                                                                {
+                                                                    "import": "invenio_vocabularies.records.api.Vocabulary"
+                                                                }
+                                                            ],
+                                                            "keys": [
+                                                                "id",
+                                                                "title",
+                                                                {
+                                                                    "key": "props.ror",
+                                                                    "model": {
+                                                                        "type": "keyword"
+                                                                    },
+                                                                    "target": "ror"
+                                                                },
+                                                                {
+                                                                    "key": "hierarchy",
+                                                                    "model": {
+                                                                        "marshmallow": {
+                                                                            "class": "oarepo_vocabularies.services.schema.HierarchySchema",
+                                                                            "generate": false,
+                                                                            "imports": [
+                                                                                {
+                                                                                    "import": "oarepo_vocabularies.services.schema.HierarchySchema"
+                                                                                }
+                                                                            ]
+                                                                        },
+                                                                        "properties": {
+                                                                            "ancestors": {
+                                                                                "items": {
+                                                                                    "type": "keyword"
+                                                                                },
+                                                                                "type": "array"
+                                                                            },
+                                                                            "ancestors_or_self": {
+                                                                                "items": {
+                                                                                    "type": "keyword"
+                                                                                },
+                                                                                "type": "array"
+                                                                            },
+                                                                            "level": {
+                                                                                "type": "integer"
+                                                                            },
+                                                                            "parent": {
+                                                                                "type": "keyword"
+                                                                            },
+                                                                            "title": {
+                                                                                "items": {
+                                                                                    "additionalProperties": {
+                                                                                        "type": "string"
+                                                                                    },
+                                                                                    "mapping": {
+                                                                                        "dynamic": true
+                                                                                    },
+                                                                                    "marshmallow": {
+                                                                                        "class": "nr_metadata.data.services.records.schema.TitleItemSchema",
+                                                                                        "field": "i18n_strings",
+                                                                                        "generate": false
+                                                                                    },
+                                                                                    "propertyNames": {
+                                                                                        "pattern": "^[a-z]{2}$"
+                                                                                    },
+                                                                                    "type": "object",
+                                                                                    "ui": {
+                                                                                        "marshmallow": {
+                                                                                            "class": "nr_metadata.data.services.records.ui_schema.TitleItemUISchema",
+                                                                                            "field": "i18n_strings",
+                                                                                            "generate": false
+                                                                                        }
+                                                                                    }
+                                                                                },
+                                                                                "type": "array"
+                                                                            }
+                                                                        },
+                                                                        "type": "object",
+                                                                        "ui": {
+                                                                            "marshmallow": {
+                                                                                "class": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema",
+                                                                                "generate": false,
+                                                                                "imports": [
+                                                                                    {
+                                                                                        "import": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema"
+                                                                                    }
+                                                                                ]
+                                                                            }
+                                                                        }
+                                                                    },
+                                                                    "target": "hierarchy"
+                                                                }
+                                                            ],
+                                                            "label.cs": "Afiliace",
+                                                            "label.en": "Affiliation",
+                                                            "marshmallow": {
+                                                                "class": "nr_metadata.common.services.records.schema_datatypes.NRAffiliationVocabularySchema",
+                                                                "generate": false,
+                                                                "read": false,
+                                                                "unknown": "INCLUDE",
+                                                                "write": false
+                                                            },
+                                                            "model": "vocabularies",
+                                                            "pid-field": "Vocabulary.pid.with_type_ctx(\"institutions\")",
+                                                            "properties": {},
+                                                            "sample": {
+                                                                "faker": "company"
+                                                            },
+                                                            "type": "taxonomy",
+                                                            "ui": {
+                                                                "detail": "taxonomy_item",
+                                                                "edit": "taxonomy_item",
+                                                                "marshmallow": {
+                                                                    "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRAffiliationVocabularyUISchema",
+                                                                    "generate": false,
+                                                                    "read": false,
+                                                                    "unknown": "INCLUDE",
+                                                                    "write": false
+                                                                }
+                                                            },
+                                                            "vocabulary-type": "institutions"
+                                                        },
+                                                        "type": "array"
+                                                    },
+                                                    "authorityIdentifiers": {
+                                                        "items": {
+                                                            "marshmallow": {
+                                                                "class": "nr_metadata.schema.identifiers.NRPersonIdentifierSchema",
+                                                                "generate": false
+                                                            },
+                                                            "properties": {
+                                                                "identifier": {
+                                                                    "i18n.key": "identifier",
+                                                                    "label.cs": "Identifik\u00e1tor",
+                                                                    "label.en": "Identifier",
+                                                                    "marshmallow": {
+                                                                        "read": false,
+                                                                        "write": false
+                                                                    },
+                                                                    "required": true,
+                                                                    "sample": {
+                                                                        "faker": "isbn13"
+                                                                    },
+                                                                    "type": "keyword",
+                                                                    "ui": {
+                                                                        "marshmallow": {
+                                                                            "read": false,
+                                                                            "write": false
+                                                                        }
+                                                                    }
+                                                                },
+                                                                "scheme": {
+                                                                    "enum": [
+                                                                        "orcid",
+                                                                        "scopusID",
+                                                                        "researcherID",
+                                                                        "czenasAutID",
+                                                                        "vedidk",
+                                                                        "institutionalID",
+                                                                        "ISNI"
+                                                                    ],
+                                                                    "hint.cs": "Doporu\u010dujeme zadat alespo\u0148 jeden z typ\u016f identifik\u00e1tor\u016f.\nPokud pot\u0159ebujete roz\u0161\u00ed\u0159it nab\u00eddku typ\u016f identifik\u00e1tor\u016f, kontaktujte n\u00e1s na support@narodni-repozitar.cz.\n",
+                                                                    "hint.en": "We recommend providing at least one of the identifier types.\nIf you need to expand the range of identifier types, contact us at support@narodni-repozitar.cz.\n",
+                                                                    "i18n.key": "identifier_type",
+                                                                    "label.cs": "Typ identifik\u00e1toru",
+                                                                    "label.en": "Identifier type",
+                                                                    "marshmallow": {
+                                                                        "read": false,
+                                                                        "write": false
+                                                                    },
+                                                                    "required": true,
+                                                                    "type": "keyword",
+                                                                    "ui": {
+                                                                        "marshmallow": {
+                                                                            "read": false,
+                                                                            "write": false
+                                                                        }
+                                                                    }
+                                                                }
+                                                            },
+                                                            "type": "object",
+                                                            "ui": {
+                                                                "detail": "nr_person_identifier",
+                                                                "marshmallow": {
+                                                                    "class": "nr_metadata.ui_schema.identifiers.NRPersonIdentifierUISchema",
+                                                                    "generate": false
+                                                                }
+                                                            }
+                                                        },
+                                                        "type": "array"
+                                                    },
+                                                    "familyName": {
+                                                        "marshmallow": {
+                                                            "read": false,
+                                                            "write": false
+                                                        },
+                                                        "type": "keyword",
+                                                        "ui": {
+                                                            "marshmallow": {
+                                                                "read": false,
+                                                                "write": false
+                                                            }
+                                                        }
+                                                    },
+                                                    "fullName": {
+                                                        "label.cs": "Jm\u00e9no autora",
+                                                        "label.en": "Author name",
+                                                        "marshmallow": {
+                                                            "read": false,
+                                                            "write": false
+                                                        },
+                                                        "required": true,
+                                                        "sample": {
+                                                            "faker": "name"
+                                                        },
+                                                        "type": "keyword",
+                                                        "ui": {
+                                                            "marshmallow": {
+                                                                "read": false,
+                                                                "write": false
+                                                            }
+                                                        }
+                                                    },
+                                                    "givenName": {
+                                                        "marshmallow": {
+                                                            "read": false,
+                                                            "write": false
+                                                        },
+                                                        "type": "keyword",
+                                                        "ui": {
+                                                            "marshmallow": {
+                                                                "read": false,
+                                                                "write": false
+                                                            }
+                                                        }
+                                                    },
+                                                    "nameType": {
+                                                        "enum": [
+                                                            "Personal"
+                                                        ],
+                                                        "label.cs": "Typ",
+                                                        "label.en": "Type",
+                                                        "marshmallow": {
+                                                            "read": false,
+                                                            "write": false
+                                                        },
+                                                        "type": "keyword",
+                                                        "ui": {
+                                                            "marshmallow": {
+                                                                "read": false,
+                                                                "write": false
+                                                            }
+                                                        }
+                                                    }
+                                                },
+                                                "type": "object",
+                                                "ui": {
+                                                    "detail": "nr_person",
+                                                    "marshmallow": {
+                                                        "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRPersonUISchema",
+                                                        "generate": false
+                                                    }
+                                                }
+                                            }
+                                        },
+                                        "type": "polymorphic",
                                         "ui": {
                                             "detail": "creator",
                                             "marshmallow": {
-                                                "base-classes": [
-                                                    "nr_metadata.common.services.records.ui_schema_datatypes.NRRelatedItemCreatorUISchema"
-                                                ],
-                                                "class": "nr_metadata.documents.services.records.ui_schema.ItemCreatorsItemUISchema",
+                                                "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRRelatedItemCreatorUISchema",
                                                 "generate": true,
-                                                "imports": [
-                                                    {
-                                                        "alias": "nr_metadata.common.services.records.ui_schema_datatypes",
-                                                        "import": "nr_metadata.common.services.records.ui_schema_datatypes"
-                                                    }
-                                                ]
+                                                "read": false,
+                                                "write": false
                                             }
                                         }
                                     },
                                     "label.cs": "Auto\u0159i",
                                     "label.en": "Authors",
                                     "type": "array"
                                 },
@@ -3809,27 +5394,16 @@
                                             "write": false
                                         }
                                     }
                                 },
                                 "itemPIDs": {
                                     "items": {
                                         "marshmallow": {
-                                            "base-classes": [
-                                                "nr_metadata.schema.identifiers.NRObjectIdentifierSchema"
-                                            ],
-                                            "class": "nr_metadata.documents.services.records.schema.ObjectIdentifiersItemSchema",
-                                            "generate": false,
-                                            "imports": [
-                                                {
-                                                    "alias": "nr_metadata.schema.identifiers",
-                                                    "import": "nr_metadata.schema.identifiers"
-                                                }
-                                            ],
-                                            "read": false,
-                                            "write": false
+                                            "class": "nr_metadata.schema.identifiers.NRObjectIdentifierSchema",
+                                            "generate": false
                                         },
                                         "properties": {
                                             "identifier": {
                                                 "label.cs": "Identifik\u00e1tor objektu",
                                                 "label.en": "Object identifier",
                                                 "marshmallow": {
                                                     "read": false,
@@ -3849,15 +5423,16 @@
                                             },
                                             "scheme": {
                                                 "enum": [
                                                     "DOI",
                                                     "Handle",
                                                     "ISBN",
                                                     "ISSN",
-                                                    "RIV"
+                                                    "RIV",
+                                                    "IGSN"
                                                 ],
                                                 "label.cs": "Typ identifik\u00e1toru",
                                                 "label.en": "Identifier type",
                                                 "marshmallow": {
                                                     "read": false,
                                                     "write": false
                                                 },
@@ -3871,27 +5446,16 @@
                                                 }
                                             }
                                         },
                                         "type": "object",
                                         "ui": {
                                             "detail": "nr_object_pid",
                                             "marshmallow": {
-                                                "base-classes": [
-                                                    "nr_metadata.ui_schema.identifiers.NRObjectIdentifierUISchema"
-                                                ],
-                                                "class": "nr_metadata.documents.services.records.ui_schema.ObjectIdentifiersItemUISchema",
-                                                "generate": false,
-                                                "imports": [
-                                                    {
-                                                        "alias": "nr_metadata.ui_schema.identifiers",
-                                                        "import": "nr_metadata.ui_schema.identifiers"
-                                                    }
-                                                ],
-                                                "read": false,
-                                                "write": false
+                                                "class": "nr_metadata.ui_schema.identifiers.NRObjectIdentifierUISchema",
+                                                "generate": false
                                             }
                                         }
                                     },
                                     "type": "array"
                                 },
                                 "itemPublisher": {
                                     "label.cs": "Vydavatel",
@@ -3923,25 +5487,16 @@
                                     "keys": [
                                         "id",
                                         "title"
                                     ],
                                     "label.cs": "Typ vazby",
                                     "label.en": "Relation type",
                                     "marshmallow": {
-                                        "base-classes": [
-                                            "nr_metadata.common.services.records.schema_datatypes.NRItemRelationTypeVocabularySchema"
-                                        ],
-                                        "class": "nr_metadata.documents.services.records.schema.ItemRelationTypeSchema",
+                                        "class": "nr_metadata.common.services.records.schema_datatypes.NRItemRelationTypeVocabularySchema",
                                         "generate": true,
-                                        "imports": [
-                                            {
-                                                "alias": "nr_metadata.common.services.records.schema_datatypes",
-                                                "import": "nr_metadata.common.services.records.schema_datatypes"
-                                            }
-                                        ],
                                         "read": false,
                                         "unknown": "INCLUDE",
                                         "write": false
                                     },
                                     "model": "vocabularies",
                                     "pid-field": "Vocabulary.pid.with_type_ctx(\"item-relation-types\")",
                                     "properties": {
@@ -4019,25 +5574,16 @@
                                         }
                                     },
                                     "type": "vocabulary",
                                     "ui": {
                                         "detail": "vocabulary_item",
                                         "edit": "vocabulary_item",
                                         "marshmallow": {
-                                            "base-classes": [
-                                                "nr_metadata.common.services.records.ui_schema_datatypes.NRItemRelationTypeVocabularyUISchema"
-                                            ],
-                                            "class": "nr_metadata.documents.services.records.ui_schema.ItemRelationTypeUISchema",
+                                            "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRItemRelationTypeVocabularyUISchema",
                                             "generate": true,
-                                            "imports": [
-                                                {
-                                                    "alias": "nr_metadata.common.services.records.ui_schema_datatypes",
-                                                    "import": "nr_metadata.common.services.records.ui_schema_datatypes"
-                                                }
-                                            ],
                                             "read": false,
                                             "unknown": "INCLUDE",
                                             "write": false
                                         }
                                     },
                                     "vocabulary-type": "item-relation-types"
                                 },
@@ -4055,25 +5601,16 @@
                                     "keys": [
                                         "id",
                                         "title"
                                     ],
                                     "label.cs": "Typ zdroje",
                                     "label.en": "Resource type",
                                     "marshmallow": {
-                                        "base-classes": [
-                                            "nr_metadata.common.services.records.schema_datatypes.NRResourceTypeVocabularySchema"
-                                        ],
-                                        "class": "nr_metadata.documents.services.records.schema.ItemResourceTypeSchema",
+                                        "class": "nr_metadata.common.services.records.schema_datatypes.NRResourceTypeVocabularySchema",
                                         "generate": true,
-                                        "imports": [
-                                            {
-                                                "alias": "nr_metadata.common.services.records.schema_datatypes",
-                                                "import": "nr_metadata.common.services.records.schema_datatypes"
-                                            }
-                                        ],
                                         "read": false,
                                         "unknown": "INCLUDE",
                                         "write": false
                                     },
                                     "model": "vocabularies",
                                     "pid-field": "Vocabulary.pid.with_type_ctx(\"resource-types\")",
                                     "properties": {
@@ -4156,25 +5693,16 @@
                                         "Dataset"
                                     ],
                                     "type": "vocabulary",
                                     "ui": {
                                         "detail": "vocabulary_item",
                                         "edit": "vocabulary_item",
                                         "marshmallow": {
-                                            "base-classes": [
-                                                "nr_metadata.common.services.records.ui_schema_datatypes.NRResourceTypeVocabularyUISchema"
-                                            ],
-                                            "class": "nr_metadata.documents.services.records.ui_schema.ItemResourceTypeUISchema",
+                                            "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRResourceTypeVocabularyUISchema",
                                             "generate": true,
-                                            "imports": [
-                                                {
-                                                    "alias": "nr_metadata.common.services.records.ui_schema_datatypes",
-                                                    "import": "nr_metadata.common.services.records.ui_schema_datatypes"
-                                                }
-                                            ],
                                             "read": false,
                                             "unknown": "INCLUDE",
                                             "write": false
                                         }
                                     },
                                     "vocabulary-type": "resource-types"
                                 },
@@ -4259,27 +5787,16 @@
                                     }
                                 }
                             },
                             "type": "object",
                             "ui": {
                                 "detail": "related_item",
                                 "marshmallow": {
-                                    "base-classes": [
-                                        "nr_metadata.common.services.records.ui_schema_datatypes.NRRelatedItemUISchema"
-                                    ],
-                                    "class": "nr_metadata.documents.services.records.ui_schema.RelatedItemsItemUISchema",
-                                    "generate": true,
-                                    "imports": [
-                                        {
-                                            "alias": "nr_metadata.common.services.records.ui_schema_datatypes",
-                                            "import": "nr_metadata.common.services.records.ui_schema_datatypes"
-                                        }
-                                    ],
-                                    "read": false,
-                                    "write": false
+                                    "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRRelatedItemUISchema",
+                                    "generate": false
                                 }
                             }
                         },
                         "label.cs": "Vazba na/z dal\u0161\u00edch zdroj\u016f:",
                         "label.en": "Link to/from other resources:",
                         "type": "array"
                     },
@@ -4297,25 +5814,16 @@
                         "keys": [
                             "id",
                             "title"
                         ],
                         "label.cs": "Typ zdroje",
                         "label.en": "Resource type",
                         "marshmallow": {
-                            "base-classes": [
-                                "nr_metadata.common.services.records.schema_datatypes.NRResourceTypeVocabularySchema"
-                            ],
-                            "class": "nr_metadata.documents.services.records.schema.ItemResourceTypeSchema",
+                            "class": "nr_metadata.common.services.records.schema_datatypes.NRResourceTypeVocabularySchema",
                             "generate": false,
-                            "imports": [
-                                {
-                                    "alias": "nr_metadata.common.services.records.schema_datatypes",
-                                    "import": "nr_metadata.common.services.records.schema_datatypes"
-                                }
-                            ],
                             "read": false,
                             "unknown": "INCLUDE",
                             "write": false
                         },
                         "model": "vocabularies",
                         "pid-field": "Vocabulary.pid.with_type_ctx(\"resource-types\")",
                         "properties": {
@@ -4399,67 +5907,49 @@
                             "Dataset"
                         ],
                         "type": "vocabulary",
                         "ui": {
                             "detail": "vocabulary_item",
                             "edit": "vocabulary_item",
                             "marshmallow": {
-                                "base-classes": [
-                                    "nr_metadata.common.services.records.ui_schema_datatypes.NRResourceTypeVocabularyUISchema"
-                                ],
-                                "class": "nr_metadata.documents.services.records.ui_schema.ItemResourceTypeUISchema",
+                                "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRResourceTypeVocabularyUISchema",
                                 "generate": false,
-                                "imports": [
-                                    {
-                                        "alias": "nr_metadata.common.services.records.ui_schema_datatypes",
-                                        "import": "nr_metadata.common.services.records.ui_schema_datatypes"
-                                    }
-                                ],
                                 "read": false,
                                 "unknown": "INCLUDE",
                                 "write": false
                             }
                         },
                         "vocabulary-type": "resource-types"
                     },
                     "rights": {
                         "facets": {
                             "args": [
-                                "vocabulary='licenses'"
+                                "vocabulary='rights'"
                             ]
                         },
                         "imports": [
                             {
                                 "import": "invenio_vocabularies.records.api.Vocabulary"
                             }
                         ],
                         "keys": [
                             "id",
                             "title"
                         ],
-                        "label.cs": "Licence",
-                        "label.en": "License",
+                        "label.cs": "Pr\u00e1va/Licence",
+                        "label.en": "Rights/Licenses",
                         "marshmallow": {
-                            "base-classes": [
-                                "nr_metadata.common.services.records.schema_datatypes.NRLicenseVocabularySchema"
-                            ],
-                            "class": "nr_metadata.documents.services.records.schema.RightsSchema",
+                            "class": "nr_metadata.common.services.records.schema_datatypes.NRRightsVocabularySchema",
                             "generate": true,
-                            "imports": [
-                                {
-                                    "alias": "nr_metadata.common.services.records.schema_datatypes",
-                                    "import": "nr_metadata.common.services.records.schema_datatypes"
-                                }
-                            ],
                             "read": false,
                             "unknown": "INCLUDE",
                             "write": false
                         },
                         "model": "vocabularies",
-                        "pid-field": "Vocabulary.pid.with_type_ctx(\"licenses\")",
+                        "pid-field": "Vocabulary.pid.with_type_ctx(\"rights\")",
                         "properties": {
                             "@v": {
                                 "facets": {
                                     "facet": false
                                 },
                                 "marshmallow": {
                                     "field-class": "marshmallow.fields.String",
@@ -4539,48 +6029,28 @@
                             "CC BY-NC-ND"
                         ],
                         "type": "vocabulary",
                         "ui": {
                             "detail": "vocabulary_item",
                             "edit": "vocabulary_item",
                             "marshmallow": {
-                                "base-classes": [
-                                    "nr_metadata.common.services.records.ui_schema_datatypes.NRLicenseVocabularyUISchema"
-                                ],
-                                "class": "nr_metadata.documents.services.records.ui_schema.RightsUISchema",
+                                "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRRightsVocabularyUISchema",
                                 "generate": true,
-                                "imports": [
-                                    {
-                                        "alias": "nr_metadata.common.services.records.ui_schema_datatypes",
-                                        "import": "nr_metadata.common.services.records.ui_schema_datatypes"
-                                    }
-                                ],
                                 "read": false,
                                 "unknown": "INCLUDE",
                                 "write": false
                             }
                         },
-                        "vocabulary-type": "licenses"
+                        "vocabulary-type": "rights"
                     },
                     "series": {
                         "items": {
                             "marshmallow": {
-                                "base-classes": [
-                                    "nr_metadata.common.services.records.schema_datatypes.NRSeriesSchema"
-                                ],
-                                "class": "nr_metadata.documents.services.records.schema.SeriesItemSchema",
-                                "generate": true,
-                                "imports": [
-                                    {
-                                        "alias": "nr_metadata.common.services.records.schema_datatypes",
-                                        "import": "nr_metadata.common.services.records.schema_datatypes"
-                                    }
-                                ],
-                                "read": false,
-                                "write": false
+                                "class": "nr_metadata.common.services.records.schema_datatypes.NRSeriesSchema",
+                                "generate": false
                             },
                             "properties": {
                                 "seriesTitle": {
                                     "label.cs": "N\u00e1zev edice",
                                     "label.en": "Series title",
                                     "marshmallow": {
                                         "read": false,
@@ -4622,31 +6092,20 @@
                                     }
                                 }
                             },
                             "type": "object",
                             "ui": {
                                 "detail": "series",
                                 "marshmallow": {
-                                    "base-classes": [
-                                        "nr_metadata.common.services.records.ui_schema_datatypes.NRSeriesUISchema"
-                                    ],
-                                    "class": "nr_metadata.documents.services.records.ui_schema.SeriesItemUISchema",
-                                    "generate": true,
-                                    "imports": [
-                                        {
-                                            "alias": "nr_metadata.common.services.records.ui_schema_datatypes",
-                                            "import": "nr_metadata.common.services.records.ui_schema_datatypes"
-                                        }
-                                    ],
-                                    "read": false,
-                                    "write": false
+                                    "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRSeriesUISchema",
+                                    "generate": false
                                 }
                             }
                         },
-                        "label.cs": "S\u00e9rie",
+                        "label.cs": "Edice",
                         "label.en": "Series",
                         "type": "array"
                     },
                     "subjectCategories": {
                         "items": {
                             "facets": {
                                 "args": [
@@ -4661,25 +6120,16 @@
                             "keys": [
                                 "id",
                                 "title"
                             ],
                             "label.cs": "Oborov\u00e9 t\u0159\u00edd\u011bn\u00ed",
                             "label.en": "Subject categories",
                             "marshmallow": {
-                                "base-classes": [
-                                    "nr_metadata.common.services.records.schema_datatypes.NRSubjectCategoryVocabularySchema"
-                                ],
-                                "class": "nr_metadata.documents.services.records.schema.SubjectCategoriesItemSchema",
+                                "class": "nr_metadata.common.services.records.schema_datatypes.NRSubjectCategoryVocabularySchema",
                                 "generate": true,
-                                "imports": [
-                                    {
-                                        "alias": "nr_metadata.common.services.records.schema_datatypes",
-                                        "import": "nr_metadata.common.services.records.schema_datatypes"
-                                    }
-                                ],
                                 "read": false,
                                 "unknown": "INCLUDE",
                                 "write": false
                             },
                             "model": "vocabularies",
                             "pid-field": "Vocabulary.pid.with_type_ctx(\"subject-categories\")",
                             "properties": {
@@ -4757,52 +6207,32 @@
                                 }
                             },
                             "type": "vocabulary",
                             "ui": {
                                 "detail": "vocabulary_item",
                                 "edit": "vocabulary_item",
                                 "marshmallow": {
-                                    "base-classes": [
-                                        "nr_metadata.common.services.records.ui_schema_datatypes.NRSubjectCategoryVocabularyUISchema"
-                                    ],
-                                    "class": "nr_metadata.documents.services.records.ui_schema.SubjectCategoriesItemUISchema",
+                                    "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRSubjectCategoryVocabularyUISchema",
                                     "generate": true,
-                                    "imports": [
-                                        {
-                                            "alias": "nr_metadata.common.services.records.ui_schema_datatypes",
-                                            "import": "nr_metadata.common.services.records.ui_schema_datatypes"
-                                        }
-                                    ],
                                     "read": false,
                                     "unknown": "INCLUDE",
                                     "write": false
                                 }
                             },
                             "vocabulary-type": "subject-categories"
                         },
                         "label.cs": "Oborov\u00e9 t\u0159\u00edd\u011bn\u00ed",
                         "label.en": "Subject categories",
                         "type": "array"
                     },
                     "subjects": {
                         "items": {
                             "marshmallow": {
-                                "base-classes": [
-                                    "nr_metadata.common.services.records.schema_datatypes.NRSubjectSchema"
-                                ],
-                                "class": "nr_metadata.documents.services.records.schema.SubjectsItemSchema",
-                                "generate": true,
-                                "imports": [
-                                    {
-                                        "alias": "nr_metadata.common.services.records.schema_datatypes",
-                                        "import": "nr_metadata.common.services.records.schema_datatypes"
-                                    }
-                                ],
-                                "read": false,
-                                "write": false
+                                "class": "nr_metadata.common.services.records.schema_datatypes.NRSubjectSchema",
+                                "generate": false
                             },
                             "properties": {
                                 "classificationCode": {
                                     "marshmallow": {
                                         "read": false,
                                         "write": false
                                     },
@@ -4902,27 +6332,16 @@
                                     }
                                 }
                             },
                             "type": "object",
                             "ui": {
                                 "detail": "subject",
                                 "marshmallow": {
-                                    "base-classes": [
-                                        "nr_metadata.common.services.records.ui_schema_datatypes.NRSubjectUISchema"
-                                    ],
-                                    "class": "nr_metadata.documents.services.records.ui_schema.SubjectsItemUISchema",
-                                    "generate": true,
-                                    "imports": [
-                                        {
-                                            "alias": "nr_metadata.common.services.records.ui_schema_datatypes",
-                                            "import": "nr_metadata.common.services.records.ui_schema_datatypes"
-                                        }
-                                    ],
-                                    "read": false,
-                                    "write": false
+                                    "class": "nr_metadata.common.services.records.ui_schema_datatypes.NRSubjectUISchema",
+                                    "generate": false
                                 }
                             }
                         },
                         "label.cs": "Kl\u00ed\u010dov\u00e1 slova",
                         "label.en": "Keywords",
                         "type": "array",
                         "ui": {
@@ -4930,27 +6349,16 @@
                                 "field-class": "nr_metadata.ui_schema.subjects.NRSubjectListField"
                             }
                         }
                     },
                     "systemIdentifiers": {
                         "items": {
                             "marshmallow": {
-                                "base-classes": [
-                                    "nr_metadata.schema.identifiers.NRSystemIdentifierSchema"
-                                ],
-                                "class": "nr_metadata.documents.services.records.schema.SystemIdentifiersItemSchema",
-                                "generate": true,
-                                "imports": [
-                                    {
-                                        "alias": "nr_metadata.schema.identifiers",
-                                        "import": "nr_metadata.schema.identifiers"
-                                    }
-                                ],
-                                "read": false,
-                                "write": false
+                                "class": "nr_metadata.schema.identifiers.NRSystemIdentifierSchema",
+                                "generate": false
                             },
                             "properties": {
                                 "identifier": {
                                     "label.cs": "Syst\u00e9mov\u00fd identifik\u00e1tor",
                                     "label.en": "System Identifier",
                                     "marshmallow": {
                                         "read": false,
@@ -4989,27 +6397,16 @@
                                     }
                                 }
                             },
                             "type": "object",
                             "ui": {
                                 "detail": "identifier",
                                 "marshmallow": {
-                                    "base-classes": [
-                                        "nr_metadata.ui_schema.identifiers.NRSystemIdentifierUISchema"
-                                    ],
-                                    "class": "nr_metadata.documents.services.records.ui_schema.SystemIdentifiersItemUISchema",
-                                    "generate": true,
-                                    "imports": [
-                                        {
-                                            "alias": "nr_metadata.ui_schema.identifiers",
-                                            "import": "nr_metadata.ui_schema.identifiers"
-                                        }
-                                    ],
-                                    "read": false,
-                                    "write": false
+                                    "class": "nr_metadata.ui_schema.identifiers.NRSystemIdentifierUISchema",
+                                    "generate": false
                                 }
                             }
                         },
                         "label.cs": "Syst\u00e9mov\u00e9 identifik\u00e1tory",
                         "label.en": "System identifiers",
                         "type": "array"
                     },
@@ -5056,305 +6453,14 @@
                             "marshmallow": {
                                 "field-class": "oarepo_runtime.services.schema.i18n_ui.MultilingualUIField",
                                 "read": false,
                                 "write": false
                             }
                         }
                     },
-                    "thesis": {
-                        "marshmallow": {
-                            "class": "nr_metadata.documents.services.records.schema.NRThesisSchema",
-                            "generate": true
-                        },
-                        "properties": {
-                            "dateDefended": {
-                                "label.cs": "Datum obhajoby",
-                                "label.en": "Date defended",
-                                "type": "date"
-                            },
-                            "defended": {
-                                "label.cs": "Obh\u00e1jeno?",
-                                "label.en": "Defended?",
-                                "type": "boolean"
-                            },
-                            "degreeGrantors": {
-                                "items": {
-                                    "facets": {
-                                        "args": [
-                                            "vocabulary='institutions'"
-                                        ]
-                                    },
-                                    "imports": [
-                                        {
-                                            "import": "invenio_vocabularies.records.api.Vocabulary"
-                                        }
-                                    ],
-                                    "keys": [
-                                        "id",
-                                        "title",
-                                        {
-                                            "key": "hierarchy",
-                                            "model": {
-                                                "marshmallow": {
-                                                    "class": "oarepo_vocabularies.services.schema.HierarchySchema",
-                                                    "generate": false,
-                                                    "imports": [
-                                                        {
-                                                            "import": "oarepo_vocabularies.services.schema.HierarchySchema"
-                                                        }
-                                                    ]
-                                                },
-                                                "properties": {
-                                                    "ancestors": {
-                                                        "items": {
-                                                            "type": "keyword"
-                                                        },
-                                                        "type": "array"
-                                                    },
-                                                    "ancestors_or_self": {
-                                                        "items": {
-                                                            "type": "keyword"
-                                                        },
-                                                        "type": "array"
-                                                    },
-                                                    "level": {
-                                                        "type": "integer"
-                                                    },
-                                                    "parent": {
-                                                        "type": "keyword"
-                                                    },
-                                                    "title": {
-                                                        "items": {
-                                                            "additionalProperties": {
-                                                                "type": "string"
-                                                            },
-                                                            "mapping": {
-                                                                "dynamic": true
-                                                            },
-                                                            "marshmallow": {
-                                                                "class": "nr_metadata.documents.services.records.schema.TitleItemSchema",
-                                                                "field": "i18n_strings",
-                                                                "generate": false
-                                                            },
-                                                            "propertyNames": {
-                                                                "pattern": "^[a-z]{2}$"
-                                                            },
-                                                            "type": "object",
-                                                            "ui": {
-                                                                "marshmallow": {
-                                                                    "class": "nr_metadata.documents.services.records.ui_schema.TitleItemUISchema",
-                                                                    "field": "i18n_strings",
-                                                                    "generate": false
-                                                                }
-                                                            }
-                                                        },
-                                                        "type": "array"
-                                                    }
-                                                },
-                                                "type": "object",
-                                                "ui": {
-                                                    "marshmallow": {
-                                                        "class": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema",
-                                                        "generate": false,
-                                                        "imports": [
-                                                            {
-                                                                "import": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema"
-                                                            }
-                                                        ]
-                                                    }
-                                                }
-                                            },
-                                            "target": "hierarchy"
-                                        }
-                                    ],
-                                    "marshmallow": {
-                                        "class": "nr_metadata.documents.services.records.schema.NRDegreeGrantorSchema",
-                                        "generate": true,
-                                        "unknown": "INCLUDE"
-                                    },
-                                    "model": "vocabularies",
-                                    "pid-field": "Vocabulary.pid.with_type_ctx(\"institutions\")",
-                                    "properties": {
-                                        "@v": {
-                                            "facets": {
-                                                "facet": false
-                                            },
-                                            "marshmallow": {
-                                                "field-class": "marshmallow.fields.String",
-                                                "field-name": "_version"
-                                            },
-                                            "type": "keyword",
-                                            "ui": {
-                                                "marshmallow": {
-                                                    "field-class": "marshmallow.fields.String",
-                                                    "field-name": "_version"
-                                                }
-                                            }
-                                        },
-                                        "hierarchy": {
-                                            "marshmallow": {
-                                                "class": "oarepo_vocabularies.services.schema.HierarchySchema",
-                                                "generate": false,
-                                                "imports": [
-                                                    {
-                                                        "import": "oarepo_vocabularies.services.schema.HierarchySchema"
-                                                    }
-                                                ]
-                                            },
-                                            "properties": {
-                                                "ancestors": {
-                                                    "items": {
-                                                        "type": "keyword"
-                                                    },
-                                                    "type": "array"
-                                                },
-                                                "ancestors_or_self": {
-                                                    "items": {
-                                                        "type": "keyword"
-                                                    },
-                                                    "type": "array"
-                                                },
-                                                "level": {
-                                                    "type": "integer"
-                                                },
-                                                "parent": {
-                                                    "type": "keyword"
-                                                },
-                                                "title": {
-                                                    "items": {
-                                                        "additionalProperties": {
-                                                            "type": "string"
-                                                        },
-                                                        "mapping": {
-                                                            "dynamic": true
-                                                        },
-                                                        "marshmallow": {
-                                                            "class": "nr_metadata.documents.services.records.schema.TitleItemSchema",
-                                                            "field": "i18n_strings",
-                                                            "generate": false
-                                                        },
-                                                        "propertyNames": {
-                                                            "pattern": "^[a-z]{2}$"
-                                                        },
-                                                        "type": "object",
-                                                        "ui": {
-                                                            "marshmallow": {
-                                                                "class": "nr_metadata.documents.services.records.ui_schema.TitleItemUISchema",
-                                                                "field": "i18n_strings",
-                                                                "generate": false
-                                                            }
-                                                        }
-                                                    },
-                                                    "type": "array"
-                                                }
-                                            },
-                                            "type": "object",
-                                            "ui": {
-                                                "marshmallow": {
-                                                    "class": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema",
-                                                    "generate": false,
-                                                    "imports": [
-                                                        {
-                                                            "import": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema"
-                                                        }
-                                                    ]
-                                                }
-                                            }
-                                        },
-                                        "id": {
-                                            "mapping": {
-                                                "fields": {
-                                                    "text": {
-                                                        "type": "search_as_you_type"
-                                                    }
-                                                }
-                                            },
-                                            "marshmallow": {
-                                                "field-class": "marshmallow.fields.String",
-                                                "imports": [],
-                                                "validators": []
-                                            },
-                                            "sample": {
-                                                "skip": true
-                                            },
-                                            "type": "keyword",
-                                            "ui": {
-                                                "marshmallow": {
-                                                    "field-class": "marshmallow.fields.String",
-                                                    "imports": [],
-                                                    "validators": []
-                                                }
-                                            }
-                                        },
-                                        "title": {
-                                            "additionalProperties": {
-                                                "type": "string"
-                                            },
-                                            "mapping": {
-                                                "dynamic": true,
-                                                "properties": {
-                                                    "en": {
-                                                        "copy_to": "title_sort",
-                                                        "type": "search_as_you_type"
-                                                    }
-                                                }
-                                            },
-                                            "marshmallow": {
-                                                "class": "invenio_vocabularies.services.records.schema.TitleSchema",
-                                                "field": "{{invenio_vocabularies.services.schema.i18n_strings}}",
-                                                "field-class": "marshmallow.fields.Nested",
-                                                "generate": false,
-                                                "validators": []
-                                            },
-                                            "propertyNames": {
-                                                "pattern": "^[a-z]{2}$"
-                                            },
-                                            "type": "object",
-                                            "ui": {
-                                                "marshmallow": {
-                                                    "field": "{{oarepo_vocabularies.services.ui_schema.VocabularyI18nStrUIField}}()",
-                                                    "generate": false
-                                                }
-                                            }
-                                        }
-                                    },
-                                    "type": "taxonomy",
-                                    "ui": {
-                                        "detail": "nr_degree_grantor",
-                                        "edit": "taxonomy_item",
-                                        "marshmallow": {
-                                            "class": "nr_metadata.documents.services.records.ui_schema.NRDegreeGrantorUISchema",
-                                            "generate": true,
-                                            "unknown": "INCLUDE"
-                                        }
-                                    },
-                                    "vocabulary-type": "institutions"
-                                },
-                                "label.cs": "Instituce / grantor",
-                                "label.en": "Degree grantor",
-                                "type": "array"
-                            },
-                            "studyFields": {
-                                "items": {
-                                    "type": "keyword"
-                                },
-                                "label.cs": "Oblasti studia",
-                                "label.en": "Study fields",
-                                "type": "array"
-                            }
-                        },
-                        "type": "object",
-                        "ui": {
-                            "detail": "thesis",
-                            "marshmallow": {
-                                "class": "nr_metadata.documents.services.records.ui_schema.NRThesisUISchema",
-                                "generate": true
-                            }
-                        }
-                    },
                     "title": {
                         "label.cs": "N\u00e1zev",
                         "label.en": "Title",
                         "marshmallow": {
                             "read": false,
                             "write": false
                         },
@@ -5392,314 +6498,18 @@
                 },
                 "type": "object",
                 "ui": {
                     "marshmallow": {
                         "base-classes": [
                             "nr_metadata.common.services.records.ui_schema_common.NRCommonMetadataUISchema"
                         ],
-                        "class": "nr_metadata.documents.services.records.ui_schema.NRDocumentMetadataUISchema",
+                        "class": "nr_metadata.data.services.records.ui_schema.NRDataMetadataUISchema",
                         "extra-code": "",
                         "generate": true,
-                        "imports": [
-                            {
-                                "alias": "nr_metadata.common.services.records.ui_schema_common",
-                                "import": "nr_metadata.common.services.records.ui_schema_common"
-                            }
-                        ],
-                        "module": "nr_metadata.documents.services.records.ui_schema"
-                    }
-                }
-            },
-            "syntheticFields": {
-                "marshmallow": {
-                    "class": "nr_metadata.documents.services.records.schema.NRDocumentSyntheticFieldsSchema",
-                    "generate": true
-                },
-                "properties": {
-                    "institutions": {
-                        "facets": {
-                            "args": [
-                                "vocabulary='institutions'"
-                            ]
-                        },
-                        "imports": [
-                            {
-                                "import": "invenio_vocabularies.records.api.Vocabulary"
-                            }
-                        ],
-                        "keys": [
-                            "id",
-                            "title",
-                            {
-                                "key": "hierarchy",
-                                "model": {
-                                    "marshmallow": {
-                                        "class": "oarepo_vocabularies.services.schema.HierarchySchema",
-                                        "generate": false,
-                                        "imports": [
-                                            {
-                                                "import": "oarepo_vocabularies.services.schema.HierarchySchema"
-                                            }
-                                        ]
-                                    },
-                                    "properties": {
-                                        "ancestors": {
-                                            "items": {
-                                                "type": "keyword"
-                                            },
-                                            "type": "array"
-                                        },
-                                        "ancestors_or_self": {
-                                            "items": {
-                                                "type": "keyword"
-                                            },
-                                            "type": "array"
-                                        },
-                                        "level": {
-                                            "type": "integer"
-                                        },
-                                        "parent": {
-                                            "type": "keyword"
-                                        },
-                                        "title": {
-                                            "items": {
-                                                "additionalProperties": {
-                                                    "type": "string"
-                                                },
-                                                "mapping": {
-                                                    "dynamic": true
-                                                },
-                                                "marshmallow": {
-                                                    "class": "nr_metadata.documents.services.records.schema.TitleItemSchema",
-                                                    "field": "i18n_strings",
-                                                    "generate": false
-                                                },
-                                                "propertyNames": {
-                                                    "pattern": "^[a-z]{2}$"
-                                                },
-                                                "type": "object",
-                                                "ui": {
-                                                    "marshmallow": {
-                                                        "class": "nr_metadata.documents.services.records.ui_schema.TitleItemUISchema",
-                                                        "field": "i18n_strings",
-                                                        "generate": false
-                                                    }
-                                                }
-                                            },
-                                            "type": "array"
-                                        }
-                                    },
-                                    "type": "object",
-                                    "ui": {
-                                        "marshmallow": {
-                                            "class": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema",
-                                            "generate": false,
-                                            "imports": [
-                                                {
-                                                    "import": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema"
-                                                }
-                                            ]
-                                        }
-                                    }
-                                },
-                                "target": "hierarchy"
-                            }
-                        ],
-                        "marshmallow": {
-                            "class": "nr_metadata.documents.services.records.schema.InstitutionsSchema",
-                            "generate": true,
-                            "read": false,
-                            "unknown": "INCLUDE",
-                            "write": false
-                        },
-                        "model": "vocabularies",
-                        "pid-field": "Vocabulary.pid.with_type_ctx(\"institutions\")",
-                        "properties": {
-                            "@v": {
-                                "facets": {
-                                    "facet": false
-                                },
-                                "marshmallow": {
-                                    "field-class": "marshmallow.fields.String",
-                                    "field-name": "_version"
-                                },
-                                "type": "keyword",
-                                "ui": {
-                                    "marshmallow": {
-                                        "field-class": "marshmallow.fields.String",
-                                        "field-name": "_version"
-                                    }
-                                }
-                            },
-                            "hierarchy": {
-                                "marshmallow": {
-                                    "class": "oarepo_vocabularies.services.schema.HierarchySchema",
-                                    "generate": false,
-                                    "imports": [
-                                        {
-                                            "import": "oarepo_vocabularies.services.schema.HierarchySchema"
-                                        }
-                                    ]
-                                },
-                                "properties": {
-                                    "ancestors": {
-                                        "items": {
-                                            "type": "keyword"
-                                        },
-                                        "type": "array"
-                                    },
-                                    "ancestors_or_self": {
-                                        "items": {
-                                            "type": "keyword"
-                                        },
-                                        "type": "array"
-                                    },
-                                    "level": {
-                                        "type": "integer"
-                                    },
-                                    "parent": {
-                                        "type": "keyword"
-                                    },
-                                    "title": {
-                                        "items": {
-                                            "additionalProperties": {
-                                                "type": "string"
-                                            },
-                                            "mapping": {
-                                                "dynamic": true
-                                            },
-                                            "marshmallow": {
-                                                "class": "nr_metadata.documents.services.records.schema.TitleItemSchema",
-                                                "field": "i18n_strings",
-                                                "generate": false
-                                            },
-                                            "propertyNames": {
-                                                "pattern": "^[a-z]{2}$"
-                                            },
-                                            "type": "object",
-                                            "ui": {
-                                                "marshmallow": {
-                                                    "class": "nr_metadata.documents.services.records.ui_schema.TitleItemUISchema",
-                                                    "field": "i18n_strings",
-                                                    "generate": false
-                                                }
-                                            }
-                                        },
-                                        "type": "array"
-                                    }
-                                },
-                                "type": "object",
-                                "ui": {
-                                    "marshmallow": {
-                                        "class": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema",
-                                        "generate": false,
-                                        "imports": [
-                                            {
-                                                "import": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema"
-                                            }
-                                        ]
-                                    }
-                                }
-                            },
-                            "id": {
-                                "mapping": {
-                                    "fields": {
-                                        "text": {
-                                            "type": "search_as_you_type"
-                                        }
-                                    }
-                                },
-                                "marshmallow": {
-                                    "field-class": "marshmallow.fields.String",
-                                    "imports": [],
-                                    "validators": []
-                                },
-                                "sample": {
-                                    "skip": true
-                                },
-                                "type": "keyword",
-                                "ui": {
-                                    "marshmallow": {
-                                        "field-class": "marshmallow.fields.String",
-                                        "imports": [],
-                                        "validators": []
-                                    }
-                                }
-                            },
-                            "title": {
-                                "additionalProperties": {
-                                    "type": "string"
-                                },
-                                "mapping": {
-                                    "dynamic": true,
-                                    "properties": {
-                                        "en": {
-                                            "copy_to": "title_sort",
-                                            "type": "search_as_you_type"
-                                        }
-                                    }
-                                },
-                                "marshmallow": {
-                                    "class": "invenio_vocabularies.services.records.schema.TitleSchema",
-                                    "field": "{{invenio_vocabularies.services.schema.i18n_strings}}",
-                                    "field-class": "marshmallow.fields.Nested",
-                                    "generate": false,
-                                    "validators": []
-                                },
-                                "propertyNames": {
-                                    "pattern": "^[a-z]{2}$"
-                                },
-                                "type": "object",
-                                "ui": {
-                                    "marshmallow": {
-                                        "field": "{{oarepo_vocabularies.services.ui_schema.VocabularyI18nStrUIField}}()",
-                                        "generate": false
-                                    }
-                                }
-                            }
-                        },
-                        "type": "taxonomy",
-                        "ui": {
-                            "detail": "taxonomy_item",
-                            "edit": "taxonomy_item",
-                            "marshmallow": {
-                                "class": "nr_metadata.documents.services.records.ui_schema.InstitutionsUISchema",
-                                "generate": true,
-                                "unknown": "INCLUDE"
-                            }
-                        },
-                        "vocabulary-type": "institutions"
-                    },
-                    "keywords_cs": {
-                        "marshmallow": {
-                            "read": false,
-                            "write": false
-                        },
-                        "type": "keyword"
-                    },
-                    "keywords_en": {
-                        "marshmallow": {
-                            "read": false,
-                            "write": false
-                        },
-                        "type": "keyword"
-                    },
-                    "person": {
-                        "marshmallow": {
-                            "read": false,
-                            "write": false
-                        },
-                        "type": "keyword"
-                    }
-                },
-                "type": "object",
-                "ui": {
-                    "marshmallow": {
-                        "class": "nr_metadata.documents.services.records.ui_schema.NRDocumentSyntheticFieldsUISchema",
-                        "generate": true
+                        "module": "nr_metadata.data.services.records.ui_schema"
                     }
                 }
             },
             "updated": {
                 "facets": {
                     "facet": false,
                     "searchable": true
@@ -5718,149 +6528,176 @@
                         "write": false
                     }
                 }
             }
         },
         "proxy": {
             "generate": true,
-            "module": "nr_metadata.documents.proxies"
+            "module": "nr_metadata.data.proxies"
         },
         "record": {
             "base-classes": [
                 "invenio_records_resources.records.api.Record{InvenioRecord}"
             ],
-            "class": "nr_metadata.documents.records.api.DocumentsRecord",
+            "class": "nr_metadata.data.records.api.DataRecord",
             "extra-code": "",
+            "fields": {},
             "generate": true,
             "imports": [],
-            "module": "nr_metadata.documents.records.api"
+            "module": "nr_metadata.data.records.api"
         },
         "record-dumper": {
             "base-classes": [
                 "oarepo_runtime.records.dumpers.SearchDumper"
             ],
-            "class": "nr_metadata.documents.records.dumpers.dumper.DocumentsDumper",
+            "class": "nr_metadata.data.records.dumpers.dumper.DataDumper",
             "extensions": [
-                "{{nr_metadata.documents.records.dumpers.multilingual.MultilingualSearchDumperExt}}()",
-                "{{nr_metadata.documents.records.dumpers.edtf.DocumentsEDTFIntervalDumperExt}}()"
+                "{{nr_metadata.data.records.dumpers.multilingual.MultilingualSearchDumperExt}}()",
+                "{{nr_metadata.data.records.dumpers.edtf.DataEDTFIntervalDumperExt}}()"
+            ],
+            "extra-code": "",
+            "generate": true,
+            "imports": [],
+            "module": "nr_metadata.data.records.dumpers.dumper"
+        },
+        "record-item": {
+            "base-classes": [
+                "oarepo_runtime.services.results.RecordItem"
+            ],
+            "class": "nr_metadata.data.services.records.results.DataRecordItem",
+            "components": [],
+            "extra-code": "",
+            "generate": true,
+            "imports": [],
+            "module": "nr_metadata.data.services.records.results"
+        },
+        "record-list": {
+            "base-classes": [
+                "oarepo_runtime.services.results.RecordList"
             ],
+            "class": "nr_metadata.data.services.records.results.DataRecordList",
+            "components": [],
             "extra-code": "",
             "generate": true,
             "imports": [],
-            "module": "nr_metadata.documents.records.dumpers.dumper"
+            "module": "nr_metadata.data.services.records.results"
         },
         "record-metadata": {
-            "alembic": "nr_metadata.documents.alembic",
-            "alias": "documents",
+            "alembic": "nr_metadata.data.alembic",
+            "alias": "data",
             "base-classes": [
                 "invenio_db.db{db.Model}",
                 "invenio_records.models.RecordMetadataBase"
             ],
-            "class": "nr_metadata.documents.records.models.DocumentsMetadata",
+            "class": "nr_metadata.data.records.models.DataMetadata",
             "extra-code": "",
             "generate": true,
             "imports": [],
-            "module": "nr_metadata.documents.records.models",
-            "table": "documents_metadata",
+            "module": "nr_metadata.data.records.models",
+            "table": "data_metadata",
             "use-versioning": true
         },
         "resource": {
+            "additional-args": [],
             "base-classes": [
                 "invenio_records_resources.resources.RecordResource"
             ],
-            "class": "nr_metadata.documents.resources.records.resource.DocumentsResource",
-            "config-key": "DOCUMENTS_RECORD_RESOURCE_CLASS",
+            "class": "nr_metadata.data.resources.records.resource.DataResource",
+            "config-key": "DATA_RECORD_RESOURCE_CLASS",
             "extra-code": "",
             "generate": true,
             "imports": [],
-            "module": "nr_metadata.documents.resources.records.resource",
+            "module": "nr_metadata.data.resources.records.resource",
             "proxy": "current_resource"
         },
         "resource-config": {
+            "additional-args": [],
             "base-classes": [
                 "invenio_records_resources.resources.RecordResourceConfig"
             ],
-            "base-html-url": "/nr-metadata-documents/",
-            "base-url": "/nr-metadata-documents/",
-            "class": "nr_metadata.documents.resources.records.config.DocumentsResourceConfig",
-            "config-key": "DOCUMENTS_RECORD_RESOURCE_CONFIG",
+            "base-html-url": "/nr-metadata-data/",
+            "base-url": "/nr-metadata-data/",
+            "class": "nr_metadata.data.resources.records.config.DataResourceConfig",
+            "config-key": "DATA_RECORD_RESOURCE_CONFIG",
             "extra-code": "",
             "generate": true,
             "imports": [],
-            "module": "nr_metadata.documents.resources.records.config"
+            "module": "nr_metadata.data.resources.records.config"
         },
         "sample": {
             "file": "data/sample_data.yaml"
         },
         "saved-model": {
-            "alias": "documents",
-            "file": "nr_metadata/documents/models/records.json",
-            "module": "nr_metadata.documents.models"
+            "alias": "data",
+            "file": "nr_metadata/data/models/records.json",
+            "module": "nr_metadata.data.models"
         },
         "search-options": {
             "base-classes": [
                 "invenio_records_resources.services.SearchOptions{InvenioSearchOptions}"
             ],
-            "class": "nr_metadata.documents.services.records.search.DocumentsSearchOptions",
+            "class": "nr_metadata.data.services.records.search.DataSearchOptions",
             "extra-code": "",
+            "fields": {},
             "generate": true,
             "imports": [],
-            "module": "nr_metadata.documents.services.records.search",
+            "module": "nr_metadata.data.services.records.search",
             "sort-options-field": "sort_options"
         },
         "searchable": true,
         "service": {
+            "additional-args": [],
             "base-classes": [
                 "invenio_records_resources.services.RecordService{InvenioRecordService}"
             ],
-            "class": "nr_metadata.documents.services.records.service.DocumentsService",
-            "config-key": "DOCUMENTS_RECORD_SERVICE_CLASS",
+            "class": "nr_metadata.data.services.records.service.DataService",
+            "config-key": "DATA_RECORD_SERVICE_CLASS",
             "extra-code": "",
             "generate": true,
             "imports": [],
-            "module": "nr_metadata.documents.services.records.service",
+            "module": "nr_metadata.data.services.records.service",
             "proxy": "current_service"
         },
         "service-config": {
+            "additional-args": [],
             "base-classes": [
                 "oarepo_runtime.services.config.service.PermissionsPresetsConfigMixin",
                 "invenio_records_resources.services.RecordServiceConfig{InvenioRecordServiceConfig}"
             ],
-            "class": "nr_metadata.documents.services.records.config.DocumentsServiceConfig",
+            "class": "nr_metadata.data.services.records.config.DataServiceConfig",
             "components": [
                 "{{invenio_records_resources.services.records.components.DataComponent}}"
             ],
-            "config-key": "DOCUMENTS_RECORD_SERVICE_CONFIG",
+            "config-key": "DATA_RECORD_SERVICE_CONFIG",
             "extra-code": "",
             "generate": true,
-            "module": "nr_metadata.documents.services.records.config",
-            "result-list-class": "oarepo_runtime.services.results.RecordList",
-            "service-id": "documents"
+            "module": "nr_metadata.data.services.records.config",
+            "service-id": "data"
         },
         "sortable": [],
         "tests": {
             "extra-code": "",
             "extra-fixtures": [],
             "module": "tests"
         },
         "translations": {
-            "alias": "documents",
-            "module": "nr_metadata.documents.translations"
+            "alias": "data",
+            "module": "nr_metadata.data.translations"
         },
         "type": "model",
         "ui": {
-            "alias": "documents",
-            "file": "nr_metadata/documents/models/ui.json",
+            "alias": "data",
+            "file": "nr_metadata/data/models/ui.json",
             "marshmallow": {
                 "base-classes": [
                     "oarepo_runtime.services.schema.ui.InvenioUISchema"
                 ],
-                "class": "nr_metadata.documents.services.records.ui_schema.NRDocumentRecordUISchema",
+                "class": "nr_metadata.data.services.records.ui_schema.NRDataRecordUISchema",
                 "extra-code": "",
                 "generate": true,
                 "imports": [],
-                "module": "nr_metadata.documents.services.records.ui_schema"
+                "module": "nr_metadata.data.services.records.ui_schema"
             },
-            "module": "nr_metadata.documents.models"
+            "module": "nr_metadata.data.models"
         }
     }
 }
```

### Comparing `nr-metadata-2.0.8/nr_metadata/documents/records/api.py` & `nr-metadata-2.0.9/nr_metadata/data/records/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,55 +2,58 @@
 from invenio_records.systemfields import ConstantField
 from invenio_records_resources.records.api import Record as InvenioRecord
 from invenio_records_resources.records.systemfields import IndexField
 from invenio_records_resources.records.systemfields.pid import PIDField, PIDFieldContext
 from invenio_vocabularies.records.api import Vocabulary
 from oarepo_runtime.records.relations import PIDRelation, RelationsField
 
-from nr_metadata.documents.records.dumpers.dumper import DocumentsDumper
-from nr_metadata.documents.records.models import DocumentsMetadata
+from nr_metadata.data.records.dumpers.dumper import DataDumper
+from nr_metadata.data.records.models import DataMetadata
 
 
-class DocumentsIdProvider(RecordIdProviderV2):
-    pid_type = "dcmnts"
+class DataIdProvider(RecordIdProviderV2):
+    pid_type = "data"
 
 
-class DocumentsRecord(InvenioRecord):
+class DataRecord(InvenioRecord):
 
-    model_cls = DocumentsMetadata
+    model_cls = DataMetadata
 
-    schema = ConstantField("$schema", "local://documents-1.0.0.json")
+    schema = ConstantField("$schema", "local://data-1.0.0.json")
 
-    index = IndexField("documents-documents-1.0.0")
+    index = IndexField("data-data-1.0.0")
 
-    pid = PIDField(
-        provider=DocumentsIdProvider, context_cls=PIDFieldContext, create=True
-    )
+    pid = PIDField(provider=DataIdProvider, context_cls=PIDFieldContext, create=True)
 
-    dumper = DocumentsDumper()
+    dumper = DataDumper()
 
     relations = RelationsField(
         accessRights=PIDRelation(
             "metadata.accessRights",
             keys=["id", "title"],
             pid_field=Vocabulary.pid.with_type_ctx("access-rights"),
         ),
         affiliations=PIDRelation(
             "metadata.contributors.affiliations",
-            keys=["id", "title", "hierarchy"],
+            keys=["id", "title", {"key": "props.ror", "target": "ror"}, "hierarchy"],
             pid_field=Vocabulary.pid.with_type_ctx("institutions"),
         ),
-        role=PIDRelation(
-            "metadata.contributors.role",
+        contributorType=PIDRelation(
+            "metadata.contributors.contributorType",
+            keys=["id", "title"],
+            pid_field=Vocabulary.pid.with_type_ctx("contributor-types"),
+        ),
+        Organizational_contributorType=PIDRelation(
+            "metadata.contributors.contributorType",
             keys=["id", "title"],
-            pid_field=Vocabulary.pid.with_type_ctx("contributor-roles"),
+            pid_field=Vocabulary.pid.with_type_ctx("contributor-types"),
         ),
-        creators_affiliations=PIDRelation(
+        Personal_affiliations=PIDRelation(
             "metadata.creators.affiliations",
-            keys=["id", "title", "hierarchy"],
+            keys=["id", "title", {"key": "props.ror", "target": "ror"}, "hierarchy"],
             pid_field=Vocabulary.pid.with_type_ctx("institutions"),
         ),
         country=PIDRelation(
             "metadata.events.eventLocation.country",
             keys=["id", "title"],
             pid_field=Vocabulary.pid.with_type_ctx("countries"),
         ),
@@ -60,27 +63,37 @@
             pid_field=Vocabulary.pid.with_type_ctx("funders"),
         ),
         languages=PIDRelation(
             "metadata.languages",
             keys=["id", "title"],
             pid_field=Vocabulary.pid.with_type_ctx("languages"),
         ),
-        itemContributors_affiliations=PIDRelation(
+        publishers=PIDRelation(
+            "metadata.publishers",
+            keys=["id", "title", {"key": "props.ror", "target": "ror"}, "hierarchy"],
+            pid_field=Vocabulary.pid.with_type_ctx("institutions"),
+        ),
+        itemContributors_Personal_affiliations=PIDRelation(
             "metadata.relatedItems.itemContributors.affiliations",
-            keys=["id", "title", "hierarchy"],
+            keys=["id", "title", {"key": "props.ror", "target": "ror"}, "hierarchy"],
             pid_field=Vocabulary.pid.with_type_ctx("institutions"),
         ),
-        itemContributors_role=PIDRelation(
-            "metadata.relatedItems.itemContributors.role",
+        Personal_contributorType=PIDRelation(
+            "metadata.relatedItems.itemContributors.contributorType",
             keys=["id", "title"],
-            pid_field=Vocabulary.pid.with_type_ctx("contributor-roles"),
+            pid_field=Vocabulary.pid.with_type_ctx("contributor-types"),
         ),
-        itemCreators_affiliations=PIDRelation(
+        itemContributors_Organizational_contributorType=PIDRelation(
+            "metadata.relatedItems.itemContributors.contributorType",
+            keys=["id", "title"],
+            pid_field=Vocabulary.pid.with_type_ctx("contributor-types"),
+        ),
+        itemCreators_Personal_affiliations=PIDRelation(
             "metadata.relatedItems.itemCreators.affiliations",
-            keys=["id", "title", "hierarchy"],
+            keys=["id", "title", {"key": "props.ror", "target": "ror"}, "hierarchy"],
             pid_field=Vocabulary.pid.with_type_ctx("institutions"),
         ),
         itemRelationType=PIDRelation(
             "metadata.relatedItems.itemRelationType",
             keys=["id", "title"],
             pid_field=Vocabulary.pid.with_type_ctx("item-relation-types"),
         ),
@@ -93,25 +106,15 @@
             "metadata.resourceType",
             keys=["id", "title"],
             pid_field=Vocabulary.pid.with_type_ctx("resource-types"),
         ),
         rights=PIDRelation(
             "metadata.rights",
             keys=["id", "title"],
-            pid_field=Vocabulary.pid.with_type_ctx("licenses"),
+            pid_field=Vocabulary.pid.with_type_ctx("rights"),
         ),
         subjectCategories=PIDRelation(
             "metadata.subjectCategories",
             keys=["id", "title"],
             pid_field=Vocabulary.pid.with_type_ctx("subject-categories"),
         ),
-        degreeGrantors=PIDRelation(
-            "metadata.thesis.degreeGrantors",
-            keys=["id", "title", "hierarchy"],
-            pid_field=Vocabulary.pid.with_type_ctx("institutions"),
-        ),
-        institutions=PIDRelation(
-            "syntheticFields.institutions",
-            keys=["id", "title", "hierarchy"],
-            pid_field=Vocabulary.pid.with_type_ctx("institutions"),
-        ),
     )
```

### Comparing `nr-metadata-2.0.8/nr_metadata/documents/records/dumpers/multilingual.py` & `nr-metadata-2.0.9/nr_metadata/data/records/dumpers/multilingual.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-2.0.8/nr_metadata/documents/records/jsonschemas/documents-1.0.0.json` & `nr-metadata-2.0.9/nr_metadata/documents/records/jsonschemas/documents-1.0.0.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99534230679749%*

 * *Differences: {"'properties'": "{'metadata': {'properties': {'contributors': {'items': {'properties': "*

 * *                 "{'affiliations': {'items': {'properties': {'ror': OrderedDict([('type', "*

 * *                 "'string')])}}}, 'contributorType': OrderedDict([('type', 'object'), "*

 * *                 "('properties', OrderedDict([('id', OrderedDict([('type', 'string')])), ('title', "*

 * *                 "OrderedDict([('type', 'object')])), ('@v', OrderedDict([('type', "*

 * *                 "'string')]))]))]), 'familyName': Order […]*

```diff
@@ -72,17 +72,14 @@
                                 "type": "string"
                             }
                         },
                         "type": "object"
                     },
                     "type": "array"
                 },
-                "collection": {
-                    "type": "string"
-                },
                 "contributors": {
                     "items": {
                         "properties": {
                             "affiliations": {
                                 "items": {
                                     "properties": {
                                         "@v": {
@@ -116,14 +113,17 @@
                                                 }
                                             },
                                             "type": "object"
                                         },
                                         "id": {
                                             "type": "string"
                                         },
+                                        "ror": {
+                                            "type": "string"
+                                        },
                                         "title": {
                                             "type": "object"
                                         }
                                     },
                                     "type": "object"
                                 },
                                 "type": "array"
@@ -138,33 +138,39 @@
                                             "type": "string"
                                         }
                                     },
                                     "type": "object"
                                 },
                                 "type": "array"
                             },
-                            "fullName": {
-                                "type": "string"
-                            },
-                            "nameType": {
-                                "type": "string"
-                            },
-                            "role": {
+                            "contributorType": {
                                 "properties": {
                                     "@v": {
                                         "type": "string"
                                     },
                                     "id": {
                                         "type": "string"
                                     },
                                     "title": {
                                         "type": "object"
                                     }
                                 },
                                 "type": "object"
+                            },
+                            "familyName": {
+                                "type": "string"
+                            },
+                            "fullName": {
+                                "type": "string"
+                            },
+                            "givenName": {
+                                "type": "string"
+                            },
+                            "nameType": {
+                                "type": "string"
                             }
                         },
                         "type": "object"
                     },
                     "type": "array"
                 },
                 "creators": {
@@ -204,14 +210,17 @@
                                                 }
                                             },
                                             "type": "object"
                                         },
                                         "id": {
                                             "type": "string"
                                         },
+                                        "ror": {
+                                            "type": "string"
+                                        },
                                         "title": {
                                             "type": "object"
                                         }
                                     },
                                     "type": "object"
                                 },
                                 "type": "array"
@@ -226,27 +235,33 @@
                                             "type": "string"
                                         }
                                     },
                                     "type": "object"
                                 },
                                 "type": "array"
                             },
+                            "familyName": {
+                                "type": "string"
+                            },
                             "fullName": {
                                 "type": "string"
                             },
+                            "givenName": {
+                                "type": "string"
+                            },
                             "nameType": {
                                 "type": "string"
                             }
                         },
                         "type": "object"
                     },
                     "type": "array"
                 },
                 "dateAvailable": {
-                    "format": "date-time",
+                    "format": "date",
                     "type": "string"
                 },
                 "dateIssued": {
                     "format": "date-time",
                     "type": "string"
                 },
                 "dateModified": {
@@ -460,14 +475,17 @@
                                                             }
                                                         },
                                                         "type": "object"
                                                     },
                                                     "id": {
                                                         "type": "string"
                                                     },
+                                                    "ror": {
+                                                        "type": "string"
+                                                    },
                                                     "title": {
                                                         "type": "object"
                                                     }
                                                 },
                                                 "type": "object"
                                             },
                                             "type": "array"
@@ -482,33 +500,39 @@
                                                         "type": "string"
                                                     }
                                                 },
                                                 "type": "object"
                                             },
                                             "type": "array"
                                         },
-                                        "fullName": {
-                                            "type": "string"
-                                        },
-                                        "nameType": {
-                                            "type": "string"
-                                        },
-                                        "role": {
+                                        "contributorType": {
                                             "properties": {
                                                 "@v": {
                                                     "type": "string"
                                                 },
                                                 "id": {
                                                     "type": "string"
                                                 },
                                                 "title": {
                                                     "type": "object"
                                                 }
                                             },
                                             "type": "object"
+                                        },
+                                        "familyName": {
+                                            "type": "string"
+                                        },
+                                        "fullName": {
+                                            "type": "string"
+                                        },
+                                        "givenName": {
+                                            "type": "string"
+                                        },
+                                        "nameType": {
+                                            "type": "string"
                                         }
                                     },
                                     "type": "object"
                                 },
                                 "type": "array"
                             },
                             "itemCreators": {
@@ -548,14 +572,17 @@
                                                             }
                                                         },
                                                         "type": "object"
                                                     },
                                                     "id": {
                                                         "type": "string"
                                                     },
+                                                    "ror": {
+                                                        "type": "string"
+                                                    },
                                                     "title": {
                                                         "type": "object"
                                                     }
                                                 },
                                                 "type": "object"
                                             },
                                             "type": "array"
@@ -570,17 +597,23 @@
                                                         "type": "string"
                                                     }
                                                 },
                                                 "type": "object"
                                             },
                                             "type": "array"
                                         },
+                                        "familyName": {
+                                            "type": "string"
+                                        },
                                         "fullName": {
                                             "type": "string"
                                         },
+                                        "givenName": {
+                                            "type": "string"
+                                        },
                                         "nameType": {
                                             "type": "string"
                                         }
                                     },
                                     "type": "object"
                                 },
                                 "type": "array"
@@ -845,14 +878,18 @@
                     "type": "string"
                 }
             },
             "type": "object"
         },
         "syntheticFields": {
             "properties": {
+                "date": {
+                    "format": "date",
+                    "type": "string"
+                },
                 "institutions": {
                     "properties": {
                         "@v": {
                             "type": "string"
                         },
                         "hierarchy": {
                             "properties": {
@@ -888,21 +925,18 @@
                         },
                         "title": {
                             "type": "object"
                         }
                     },
                     "type": "object"
                 },
-                "keywords_cs": {
-                    "type": "string"
-                },
-                "keywords_en": {
+                "keywords": {
                     "type": "string"
                 },
-                "person": {
+                "people": {
                     "type": "string"
                 }
             },
             "type": "object"
         },
         "updated": {
             "format": "date-time",
```

### Comparing `nr-metadata-2.0.8/nr_metadata/documents/records/mappings/os-v2/documents/documents-1.0.0.json` & `nr-metadata-2.0.9/nr_metadata/data/records/mappings/os-v2/data/data-1.0.0.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9572909292040229%*

 * *Differences: {"'mappings'": "{'properties': {'metadata': {'properties': {'contributors': {'properties': "*

 * *               "{'affiliations': {'properties': {'ror': OrderedDict([('type', 'keyword'), "*

 * *               "('ignore_above', 1024)])}}, 'contributorType': OrderedDict([('type', 'object'), "*

 * *               "('properties', OrderedDict([('id', OrderedDict([('fields', OrderedDict([('text', "*

 * *               "OrderedDict([('type', 'search_as_you_type')]))])), ('type', 'keyword'), "*

 * *               "('ignore_above', 1024)]) […]*

```diff
@@ -159,18 +159,14 @@
                                     }
                                 },
                                 "type": "text"
                             }
                         },
                         "type": "object"
                     },
-                    "collection": {
-                        "ignore_above": 1024,
-                        "type": "keyword"
-                    },
                     "contributors": {
                         "properties": {
                             "affiliations": {
                                 "properties": {
                                     "@v": {
                                         "ignore_above": 1024,
                                         "type": "keyword"
@@ -204,14 +200,18 @@
                                             "text": {
                                                 "type": "search_as_you_type"
                                             }
                                         },
                                         "ignore_above": 1024,
                                         "type": "keyword"
                                     },
+                                    "ror": {
+                                        "ignore_above": 1024,
+                                        "type": "keyword"
+                                    },
                                     "title": {
                                         "dynamic": true,
                                         "properties": {
                                             "en": {
                                                 "copy_to": "title_sort",
                                                 "type": "search_as_you_type"
                                             }
@@ -230,23 +230,15 @@
                                     "scheme": {
                                         "ignore_above": 1024,
                                         "type": "keyword"
                                     }
                                 },
                                 "type": "object"
                             },
-                            "fullName": {
-                                "ignore_above": 1024,
-                                "type": "keyword"
-                            },
-                            "nameType": {
-                                "ignore_above": 1024,
-                                "type": "keyword"
-                            },
-                            "role": {
+                            "contributorType": {
                                 "properties": {
                                     "@v": {
                                         "ignore_above": 1024,
                                         "type": "keyword"
                                     },
                                     "id": {
                                         "fields": {
@@ -265,14 +257,30 @@
                                                 "type": "search_as_you_type"
                                             }
                                         },
                                         "type": "object"
                                     }
                                 },
                                 "type": "object"
+                            },
+                            "familyName": {
+                                "ignore_above": 1024,
+                                "type": "keyword"
+                            },
+                            "fullName": {
+                                "ignore_above": 1024,
+                                "type": "keyword"
+                            },
+                            "givenName": {
+                                "ignore_above": 1024,
+                                "type": "keyword"
+                            },
+                            "nameType": {
+                                "ignore_above": 1024,
+                                "type": "keyword"
                             }
                         },
                         "type": "object"
                     },
                     "creators": {
                         "properties": {
                             "affiliations": {
@@ -310,14 +318,18 @@
                                             "text": {
                                                 "type": "search_as_you_type"
                                             }
                                         },
                                         "ignore_above": 1024,
                                         "type": "keyword"
                                     },
+                                    "ror": {
+                                        "ignore_above": 1024,
+                                        "type": "keyword"
+                                    },
                                     "title": {
                                         "dynamic": true,
                                         "properties": {
                                             "en": {
                                                 "copy_to": "title_sort",
                                                 "type": "search_as_you_type"
                                             }
@@ -336,37 +348,68 @@
                                     "scheme": {
                                         "ignore_above": 1024,
                                         "type": "keyword"
                                     }
                                 },
                                 "type": "object"
                             },
+                            "familyName": {
+                                "ignore_above": 1024,
+                                "type": "keyword"
+                            },
                             "fullName": {
                                 "ignore_above": 1024,
                                 "type": "keyword"
                             },
+                            "givenName": {
+                                "ignore_above": 1024,
+                                "type": "keyword"
+                            },
                             "nameType": {
                                 "ignore_above": 1024,
                                 "type": "keyword"
                             }
                         },
                         "type": "object"
                     },
                     "dateAvailable": {
-                        "format": "strict_date_time||strict_date_time_no_millis||strict_date||yyyy-MM||yyyy",
+                        "format": "basic_date||strict_date",
                         "type": "date"
                     },
+                    "dateCollected": {
+                        "format": "strict_date_time||strict_date_time_no_millis||strict_date||yyyy-MM||yyyy",
+                        "index": false,
+                        "type": "date_range"
+                    },
+                    "dateCreated": {
+                        "format": "strict_date_time||strict_date_time_no_millis||strict_date||yyyy-MM||yyyy",
+                        "index": false,
+                        "type": "date_range"
+                    },
                     "dateIssued": {
                         "format": "strict_date_time||strict_date_time_no_millis||strict_date||yyyy-MM||yyyy",
                         "type": "date"
                     },
-                    "dateModified": {
-                        "format": "strict_date_time||strict_date_time_no_millis||strict_date||yyyy-MM||yyyy",
+                    "dateValidTo": {
+                        "format": "basic_date||strict_date",
                         "type": "date"
                     },
+                    "dateWithdrawn": {
+                        "properties": {
+                            "dateInformation": {
+                                "ignore_above": 1024,
+                                "type": "keyword"
+                            },
+                            "type": {
+                                "format": "basic_date||strict_date",
+                                "type": "date"
+                            }
+                        },
+                        "type": "object"
+                    },
                     "events": {
                         "properties": {
                             "eventDate": {
                                 "format": "strict_date_time||strict_date_time_no_millis||strict_date||yyyy-MM||yyyy",
                                 "index": false,
                                 "type": "date_range"
                             },
@@ -412,26 +455,14 @@
                             },
                             "eventNameOriginal": {
                                 "type": "text"
                             }
                         },
                         "type": "object"
                     },
-                    "externalLocation": {
-                        "properties": {
-                            "externalLocationNote": {
-                                "type": "text"
-                            },
-                            "externalLocationURL": {
-                                "ignore_above": 1024,
-                                "type": "keyword"
-                            }
-                        },
-                        "type": "object"
-                    },
                     "fundingReferences": {
                         "properties": {
                             "funder": {
                                 "properties": {
                                     "@v": {
                                         "ignore_above": 1024,
                                         "type": "keyword"
@@ -573,15 +604,68 @@
                         "type": "object"
                     },
                     "originalRecord": {
                         "ignore_above": 1024,
                         "type": "keyword"
                     },
                     "publishers": {
-                        "type": "text"
+                        "properties": {
+                            "@v": {
+                                "ignore_above": 1024,
+                                "type": "keyword"
+                            },
+                            "hierarchy": {
+                                "properties": {
+                                    "ancestors": {
+                                        "ignore_above": 1024,
+                                        "type": "keyword"
+                                    },
+                                    "ancestors_or_self": {
+                                        "ignore_above": 1024,
+                                        "type": "keyword"
+                                    },
+                                    "level": {
+                                        "type": "integer"
+                                    },
+                                    "parent": {
+                                        "ignore_above": 1024,
+                                        "type": "keyword"
+                                    },
+                                    "title": {
+                                        "dynamic": true,
+                                        "type": "object"
+                                    }
+                                },
+                                "type": "object"
+                            },
+                            "id": {
+                                "fields": {
+                                    "text": {
+                                        "type": "search_as_you_type"
+                                    }
+                                },
+                                "ignore_above": 1024,
+                                "type": "keyword"
+                            },
+                            "ror": {
+                                "ignore_above": 1024,
+                                "type": "keyword"
+                            },
+                            "title": {
+                                "dynamic": true,
+                                "properties": {
+                                    "en": {
+                                        "copy_to": "title_sort",
+                                        "type": "search_as_you_type"
+                                    }
+                                },
+                                "type": "object"
+                            }
+                        },
+                        "type": "object"
                     },
                     "relatedItems": {
                         "properties": {
                             "itemContributors": {
                                 "properties": {
                                     "affiliations": {
                                         "properties": {
@@ -618,14 +702,18 @@
                                                     "text": {
                                                         "type": "search_as_you_type"
                                                     }
                                                 },
                                                 "ignore_above": 1024,
                                                 "type": "keyword"
                                             },
+                                            "ror": {
+                                                "ignore_above": 1024,
+                                                "type": "keyword"
+                                            },
                                             "title": {
                                                 "dynamic": true,
                                                 "properties": {
                                                     "en": {
                                                         "copy_to": "title_sort",
                                                         "type": "search_as_you_type"
                                                     }
@@ -644,23 +732,15 @@
                                             "scheme": {
                                                 "ignore_above": 1024,
                                                 "type": "keyword"
                                             }
                                         },
                                         "type": "object"
                                     },
-                                    "fullName": {
-                                        "ignore_above": 1024,
-                                        "type": "keyword"
-                                    },
-                                    "nameType": {
-                                        "ignore_above": 1024,
-                                        "type": "keyword"
-                                    },
-                                    "role": {
+                                    "contributorType": {
                                         "properties": {
                                             "@v": {
                                                 "ignore_above": 1024,
                                                 "type": "keyword"
                                             },
                                             "id": {
                                                 "fields": {
@@ -679,14 +759,30 @@
                                                         "type": "search_as_you_type"
                                                     }
                                                 },
                                                 "type": "object"
                                             }
                                         },
                                         "type": "object"
+                                    },
+                                    "familyName": {
+                                        "ignore_above": 1024,
+                                        "type": "keyword"
+                                    },
+                                    "fullName": {
+                                        "ignore_above": 1024,
+                                        "type": "keyword"
+                                    },
+                                    "givenName": {
+                                        "ignore_above": 1024,
+                                        "type": "keyword"
+                                    },
+                                    "nameType": {
+                                        "ignore_above": 1024,
+                                        "type": "keyword"
                                     }
                                 },
                                 "type": "object"
                             },
                             "itemCreators": {
                                 "properties": {
                                     "affiliations": {
@@ -724,14 +820,18 @@
                                                     "text": {
                                                         "type": "search_as_you_type"
                                                     }
                                                 },
                                                 "ignore_above": 1024,
                                                 "type": "keyword"
                                             },
+                                            "ror": {
+                                                "ignore_above": 1024,
+                                                "type": "keyword"
+                                            },
                                             "title": {
                                                 "dynamic": true,
                                                 "properties": {
                                                     "en": {
                                                         "copy_to": "title_sort",
                                                         "type": "search_as_you_type"
                                                     }
@@ -750,18 +850,26 @@
                                             "scheme": {
                                                 "ignore_above": 1024,
                                                 "type": "keyword"
                                             }
                                         },
                                         "type": "object"
                                     },
+                                    "familyName": {
+                                        "ignore_above": 1024,
+                                        "type": "keyword"
+                                    },
                                     "fullName": {
                                         "ignore_above": 1024,
                                         "type": "keyword"
                                     },
+                                    "givenName": {
+                                        "ignore_above": 1024,
+                                        "type": "keyword"
+                                    },
                                     "nameType": {
                                         "ignore_above": 1024,
                                         "type": "keyword"
                                     }
                                 },
                                 "type": "object"
                             },
@@ -1064,82 +1172,14 @@
                             "keyword": {
                                 "ignore_above": 256,
                                 "type": "keyword"
                             }
                         },
                         "type": "text"
                     },
-                    "thesis": {
-                        "properties": {
-                            "dateDefended": {
-                                "format": "basic_date||strict_date",
-                                "type": "date"
-                            },
-                            "defended": {
-                                "type": "boolean"
-                            },
-                            "degreeGrantors": {
-                                "properties": {
-                                    "@v": {
-                                        "ignore_above": 1024,
-                                        "type": "keyword"
-                                    },
-                                    "hierarchy": {
-                                        "properties": {
-                                            "ancestors": {
-                                                "ignore_above": 1024,
-                                                "type": "keyword"
-                                            },
-                                            "ancestors_or_self": {
-                                                "ignore_above": 1024,
-                                                "type": "keyword"
-                                            },
-                                            "level": {
-                                                "type": "integer"
-                                            },
-                                            "parent": {
-                                                "ignore_above": 1024,
-                                                "type": "keyword"
-                                            },
-                                            "title": {
-                                                "dynamic": true,
-                                                "type": "object"
-                                            }
-                                        },
-                                        "type": "object"
-                                    },
-                                    "id": {
-                                        "fields": {
-                                            "text": {
-                                                "type": "search_as_you_type"
-                                            }
-                                        },
-                                        "ignore_above": 1024,
-                                        "type": "keyword"
-                                    },
-                                    "title": {
-                                        "dynamic": true,
-                                        "properties": {
-                                            "en": {
-                                                "copy_to": "title_sort",
-                                                "type": "search_as_you_type"
-                                            }
-                                        },
-                                        "type": "object"
-                                    }
-                                },
-                                "type": "object"
-                            },
-                            "studyFields": {
-                                "ignore_above": 1024,
-                                "type": "keyword"
-                            }
-                        },
-                        "type": "object"
-                    },
                     "title": {
                         "fields": {
                             "keyword": {
                                 "ignore_above": 256,
                                 "type": "keyword"
                             }
                         },
@@ -1148,83 +1188,14 @@
                     "version": {
                         "ignore_above": 1024,
                         "type": "keyword"
                     }
                 },
                 "type": "object"
             },
-            "syntheticFields": {
-                "properties": {
-                    "institutions": {
-                        "properties": {
-                            "@v": {
-                                "ignore_above": 1024,
-                                "type": "keyword"
-                            },
-                            "hierarchy": {
-                                "properties": {
-                                    "ancestors": {
-                                        "ignore_above": 1024,
-                                        "type": "keyword"
-                                    },
-                                    "ancestors_or_self": {
-                                        "ignore_above": 1024,
-                                        "type": "keyword"
-                                    },
-                                    "level": {
-                                        "type": "integer"
-                                    },
-                                    "parent": {
-                                        "ignore_above": 1024,
-                                        "type": "keyword"
-                                    },
-                                    "title": {
-                                        "dynamic": true,
-                                        "type": "object"
-                                    }
-                                },
-                                "type": "object"
-                            },
-                            "id": {
-                                "fields": {
-                                    "text": {
-                                        "type": "search_as_you_type"
-                                    }
-                                },
-                                "ignore_above": 1024,
-                                "type": "keyword"
-                            },
-                            "title": {
-                                "dynamic": true,
-                                "properties": {
-                                    "en": {
-                                        "copy_to": "title_sort",
-                                        "type": "search_as_you_type"
-                                    }
-                                },
-                                "type": "object"
-                            }
-                        },
-                        "type": "object"
-                    },
-                    "keywords_cs": {
-                        "ignore_above": 1024,
-                        "type": "keyword"
-                    },
-                    "keywords_en": {
-                        "ignore_above": 1024,
-                        "type": "keyword"
-                    },
-                    "person": {
-                        "ignore_above": 1024,
-                        "type": "keyword"
-                    }
-                },
-                "type": "object"
-            },
             "updated": {
                 "format": "strict_date_time||strict_date_time_no_millis||basic_date_time||basic_date_time_no_millis||basic_date||strict_date||strict_date_hour_minute_second||strict_date_hour_minute_second_fraction",
                 "type": "date"
             }
         }
     }
 }
```

### Comparing `nr-metadata-2.0.8/nr_metadata/documents/resources/records/config.py` & `nr-metadata-2.0.9/nr_metadata/documents/resources/records/config.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-2.0.8/nr_metadata/documents/resources/records/ui.py` & `nr-metadata-2.0.9/nr_metadata/datacite/resources/records/ui.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+from flask import g
 from flask_resources import BaseListSchema
 from flask_resources.serializers import JSONSerializer
 from oarepo_runtime.resources import LocalizedUIJSONSerializer
 
-from nr_metadata.documents.services.records.ui_schema import NRDocumentRecordUISchema
+from nr_metadata.datacite.services.records.ui_schema import DataCiteRecordUISchema
 
 
-class DocumentsUIJSONSerializer(LocalizedUIJSONSerializer):
+class DataciteUIJSONSerializer(LocalizedUIJSONSerializer):
     """UI JSON serializer."""
 
     def __init__(self):
         """Initialise Serializer."""
         super().__init__(
             format_serializer_cls=JSONSerializer,
-            object_schema_cls=NRDocumentRecordUISchema,
+            object_schema_cls=DataCiteRecordUISchema,
             list_schema_cls=BaseListSchema,
-            schema_context={"object_key": "ui"},
+            schema_context={"object_key": "ui", "identity": g.identity},
         )
```

### Comparing `nr-metadata-2.0.8/nr_metadata/documents/services/records/config.py` & `nr-metadata-2.0.9/nr_metadata/documents/services/records/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 from invenio_records_resources.services import RecordLink
 from invenio_records_resources.services import (
     RecordServiceConfig as InvenioRecordServiceConfig,
 )
 from invenio_records_resources.services import pagination_links
 from invenio_records_resources.services.records.components import DataComponent
 from oarepo_runtime.services.config.service import PermissionsPresetsConfigMixin
-from oarepo_runtime.services.results import RecordList
 
 from nr_metadata.documents.records.api import DocumentsRecord
 from nr_metadata.documents.services.records.permissions import DocumentsPermissionPolicy
+from nr_metadata.documents.services.records.results import (
+    DocumentsRecordItem,
+    DocumentsRecordList,
+)
 from nr_metadata.documents.services.records.schema import NRDocumentRecordSchema
 from nr_metadata.documents.services.records.search import DocumentsSearchOptions
 
 
 class DocumentsServiceConfig(PermissionsPresetsConfigMixin, InvenioRecordServiceConfig):
     """DocumentsRecord service config."""
 
-    result_list_cls = RecordList
+    result_item_cls = DocumentsRecordItem
+
+    result_list_cls = DocumentsRecordList
 
     PERMISSIONS_PRESETS = ["everyone"]
 
     url_prefix = "/nr-metadata-documents/"
 
     base_permission_policy_cls = DocumentsPermissionPolicy
```

### Comparing `nr-metadata-2.0.8/nr_metadata/documents/services/records/facets.py` & `nr-metadata-2.0.9/nr_metadata/documents/services/records/facets.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,18 +65,14 @@
 )
 
 metadata_additionalTitles_titleType = TermsFacet(
     field="metadata.additionalTitles.titleType",
     label=_("metadata/additionalTitles/titleType.label"),
 )
 
-metadata_collection = TermsFacet(
-    field="metadata.collection", label=_("metadata/collection.label")
-)
-
 metadata_contributors_affiliations = HierarchyVocabularyFacet(
     field="metadata.contributors.affiliations",
     label=_("metadata/contributors/affiliations.label"),
     vocabulary="institutions",
 )
 
 metadata_contributors_authorityIdentifiers_identifier = TermsFacet(
@@ -85,30 +81,40 @@
 )
 
 metadata_contributors_authorityIdentifiers_scheme = TermsFacet(
     field="metadata.contributors.authorityIdentifiers.scheme",
     label=_("metadata/contributors/authorityIdentifiers/scheme.label"),
 )
 
+metadata_contributors_contributorType = VocabularyFacet(
+    field="metadata.contributors.contributorType",
+    label=_("metadata/contributors/contributorType.label"),
+    vocabulary="contributor-types",
+)
+
+metadata_contributors_familyName = TermsFacet(
+    field="metadata.contributors.familyName",
+    label=_("metadata/contributors/familyName.label"),
+)
+
 metadata_contributors_fullName = TermsFacet(
     field="metadata.contributors.fullName",
     label=_("metadata/contributors/fullName.label"),
 )
 
+metadata_contributors_givenName = TermsFacet(
+    field="metadata.contributors.givenName",
+    label=_("metadata/contributors/givenName.label"),
+)
+
 metadata_contributors_nameType = TermsFacet(
     field="metadata.contributors.nameType",
     label=_("metadata/contributors/nameType.label"),
 )
 
-metadata_contributors_role = VocabularyFacet(
-    field="metadata.contributors.role",
-    label=_("metadata/contributors/role.label"),
-    vocabulary="contributor-roles",
-)
-
 metadata_creators_affiliations = HierarchyVocabularyFacet(
     field="metadata.creators.affiliations",
     label=_("metadata/creators/affiliations.label"),
     vocabulary="institutions",
 )
 
 metadata_creators_authorityIdentifiers_identifier = TermsFacet(
@@ -117,18 +123,26 @@
 )
 
 metadata_creators_authorityIdentifiers_scheme = TermsFacet(
     field="metadata.creators.authorityIdentifiers.scheme",
     label=_("metadata/creators/authorityIdentifiers/scheme.label"),
 )
 
+metadata_creators_familyName = TermsFacet(
+    field="metadata.creators.familyName", label=_("metadata/creators/familyName.label")
+)
+
 metadata_creators_fullName = TermsFacet(
     field="metadata.creators.fullName", label=_("metadata/creators/fullName.label")
 )
 
+metadata_creators_givenName = TermsFacet(
+    field="metadata.creators.givenName", label=_("metadata/creators/givenName.label")
+)
+
 metadata_creators_nameType = TermsFacet(
     field="metadata.creators.nameType", label=_("metadata/creators/nameType.label")
 )
 
 metadata_dateAvailable = DateTimeFacet(
     field="metadata.dateAvailable", label=_("metadata/dateAvailable.label")
 )
@@ -232,30 +246,40 @@
 )
 
 metadata_relatedItems_itemContributors_authorityIdentifiers_scheme = TermsFacet(
     field="metadata.relatedItems.itemContributors.authorityIdentifiers.scheme",
     label=_("metadata/relatedItems/itemContributors/authorityIdentifiers/scheme.label"),
 )
 
+metadata_relatedItems_itemContributors_contributorType = VocabularyFacet(
+    field="metadata.relatedItems.itemContributors.contributorType",
+    label=_("metadata/relatedItems/itemContributors/contributorType.label"),
+    vocabulary="contributor-types",
+)
+
+metadata_relatedItems_itemContributors_familyName = TermsFacet(
+    field="metadata.relatedItems.itemContributors.familyName",
+    label=_("metadata/relatedItems/itemContributors/familyName.label"),
+)
+
 metadata_relatedItems_itemContributors_fullName = TermsFacet(
     field="metadata.relatedItems.itemContributors.fullName",
     label=_("metadata/relatedItems/itemContributors/fullName.label"),
 )
 
+metadata_relatedItems_itemContributors_givenName = TermsFacet(
+    field="metadata.relatedItems.itemContributors.givenName",
+    label=_("metadata/relatedItems/itemContributors/givenName.label"),
+)
+
 metadata_relatedItems_itemContributors_nameType = TermsFacet(
     field="metadata.relatedItems.itemContributors.nameType",
     label=_("metadata/relatedItems/itemContributors/nameType.label"),
 )
 
-metadata_relatedItems_itemContributors_role = VocabularyFacet(
-    field="metadata.relatedItems.itemContributors.role",
-    label=_("metadata/relatedItems/itemContributors/role.label"),
-    vocabulary="contributor-roles",
-)
-
 metadata_relatedItems_itemCreators_affiliations = HierarchyVocabularyFacet(
     field="metadata.relatedItems.itemCreators.affiliations",
     label=_("metadata/relatedItems/itemCreators/affiliations.label"),
     vocabulary="institutions",
 )
 
 metadata_relatedItems_itemCreators_authorityIdentifiers_identifier = TermsFacet(
@@ -264,19 +288,29 @@
 )
 
 metadata_relatedItems_itemCreators_authorityIdentifiers_scheme = TermsFacet(
     field="metadata.relatedItems.itemCreators.authorityIdentifiers.scheme",
     label=_("metadata/relatedItems/itemCreators/authorityIdentifiers/scheme.label"),
 )
 
+metadata_relatedItems_itemCreators_familyName = TermsFacet(
+    field="metadata.relatedItems.itemCreators.familyName",
+    label=_("metadata/relatedItems/itemCreators/familyName.label"),
+)
+
 metadata_relatedItems_itemCreators_fullName = TermsFacet(
     field="metadata.relatedItems.itemCreators.fullName",
     label=_("metadata/relatedItems/itemCreators/fullName.label"),
 )
 
+metadata_relatedItems_itemCreators_givenName = TermsFacet(
+    field="metadata.relatedItems.itemCreators.givenName",
+    label=_("metadata/relatedItems/itemCreators/givenName.label"),
+)
+
 metadata_relatedItems_itemCreators_nameType = TermsFacet(
     field="metadata.relatedItems.itemCreators.nameType",
     label=_("metadata/relatedItems/itemCreators/nameType.label"),
 )
 
 metadata_relatedItems_itemEndPage = TermsFacet(
     field="metadata.relatedItems.itemEndPage",
@@ -338,15 +372,15 @@
 metadata_resourceType = VocabularyFacet(
     field="metadata.resourceType",
     label=_("metadata/resourceType.label"),
     vocabulary="resource-types",
 )
 
 metadata_rights = VocabularyFacet(
-    field="metadata.rights", label=_("metadata/rights.label"), vocabulary="licenses"
+    field="metadata.rights", label=_("metadata/rights.label"), vocabulary="rights"
 )
 
 metadata_series_seriesTitle = TermsFacet(
     field="metadata.series.seriesTitle", label=_("metadata/series/seriesTitle.label")
 )
 
 metadata_series_seriesVolume = TermsFacet(
@@ -435,24 +469,24 @@
     field="metadata.thesis.studyFields", label=_("metadata/thesis/studyFields.label")
 )
 
 metadata_version = TermsFacet(
     field="metadata.version", label=_("metadata/version.label")
 )
 
+syntheticFields_date = DateTimeFacet(
+    field="syntheticFields.date", label=_("syntheticFields/date.label")
+)
+
 syntheticFields_institutions = HierarchyVocabularyFacet(
     field="syntheticFields.institutions",
     label=_("syntheticFields/institutions.label"),
     vocabulary="institutions",
 )
 
-syntheticFields_keywords_cs = TermsFacet(
-    field="syntheticFields.keywords_cs", label=_("syntheticFields/keywords_cs.label")
-)
-
-syntheticFields_keywords_en = TermsFacet(
-    field="syntheticFields.keywords_en", label=_("syntheticFields/keywords_en.label")
+syntheticFields_keywords = TermsFacet(
+    field="syntheticFields.keywords", label=_("syntheticFields/keywords.label")
 )
 
-syntheticFields_person = TermsFacet(
-    field="syntheticFields.person", label=_("syntheticFields/person.label")
+syntheticFields_people = TermsFacet(
+    field="syntheticFields.people", label=_("syntheticFields/people.label")
 )
```

### Comparing `nr-metadata-2.0.8/nr_metadata/documents/services/records/search.py` & `nr-metadata-2.0.9/nr_metadata/common/services/records/search.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,187 +1,98 @@
 from invenio_records_resources.services import SearchOptions as InvenioSearchOptions
 
 from . import facets
 
 
-class DocumentsSearchOptions(InvenioSearchOptions):
-    """DocumentsRecord search options."""
+class CommonSearchOptions(InvenioSearchOptions):
+    """CommonRecord search options."""
 
-    facet_groups = {
-        "default": {
-            "metadata_abstract_cs": facets.metadata_abstract_cs,
-            "metadata_abstract_en": facets.metadata_abstract_en,
-            "metadata_accessibility_cs": facets.metadata_accessibility_cs,
-            "metadata_accessibility_en": facets.metadata_accessibility_en,
-            "metadata_additionalTitles_title_cs": (
-                facets.metadata_additionalTitles_title_cs
-            ),
-            "metadata_additionalTitles_title_en": (
-                facets.metadata_additionalTitles_title_en
-            ),
-            "metadata_methods_cs": facets.metadata_methods_cs,
-            "metadata_methods_en": facets.metadata_methods_en,
-            "metadata_subjects_subject_cs": facets.metadata_subjects_subject_cs,
-            "metadata_subjects_subject_en": facets.metadata_subjects_subject_en,
-            "metadata_technicalInfo_cs": facets.metadata_technicalInfo_cs,
-            "metadata_technicalInfo_en": facets.metadata_technicalInfo_en,
-            **getattr(InvenioSearchOptions, "facet_groups", {}).get("default", {}),
-        },
-    }
+    facet_groups = {}
 
     facets = {
         "metadata_abstract_cs": facets.metadata_abstract_cs,
         "metadata_abstract_en": facets.metadata_abstract_en,
         "metadata_abstract_lang": facets.metadata_abstract_lang,
         "metadata_accessRights": facets.metadata_accessRights,
         "metadata_accessibility_cs": facets.metadata_accessibility_cs,
         "metadata_accessibility_en": facets.metadata_accessibility_en,
         "metadata_accessibility_lang": facets.metadata_accessibility_lang,
         "metadata_additionalTitles_title_cs": facets.metadata_additionalTitles_title_cs,
         "metadata_additionalTitles_title_en": facets.metadata_additionalTitles_title_en,
-        "metadata_additionalTitles_title_lang": (
-            facets.metadata_additionalTitles_title_lang
-        ),
-        "metadata_additionalTitles_titleType": (
-            facets.metadata_additionalTitles_titleType
-        ),
-        "metadata_collection": facets.metadata_collection,
+        "metadata_additionalTitles_title_lang": facets.metadata_additionalTitles_title_lang,
+        "metadata_additionalTitles_titleType": facets.metadata_additionalTitles_titleType,
         "metadata_contributors_affiliations": facets.metadata_contributors_affiliations,
-        "metadata_contributors_authorityIdentifiers_identifier": (
-            facets.metadata_contributors_authorityIdentifiers_identifier
-        ),
-        "metadata_contributors_authorityIdentifiers_scheme": (
-            facets.metadata_contributors_authorityIdentifiers_scheme
-        ),
+        "metadata_contributors_authorityIdentifiers_identifier": facets.metadata_contributors_authorityIdentifiers_identifier,
+        "metadata_contributors_authorityIdentifiers_scheme": facets.metadata_contributors_authorityIdentifiers_scheme,
+        "metadata_contributors_contributorType": facets.metadata_contributors_contributorType,
+        "metadata_contributors_familyName": facets.metadata_contributors_familyName,
         "metadata_contributors_fullName": facets.metadata_contributors_fullName,
+        "metadata_contributors_givenName": facets.metadata_contributors_givenName,
         "metadata_contributors_nameType": facets.metadata_contributors_nameType,
-        "metadata_contributors_role": facets.metadata_contributors_role,
         "metadata_creators_affiliations": facets.metadata_creators_affiliations,
-        "metadata_creators_authorityIdentifiers_identifier": (
-            facets.metadata_creators_authorityIdentifiers_identifier
-        ),
-        "metadata_creators_authorityIdentifiers_scheme": (
-            facets.metadata_creators_authorityIdentifiers_scheme
-        ),
+        "metadata_creators_authorityIdentifiers_identifier": facets.metadata_creators_authorityIdentifiers_identifier,
+        "metadata_creators_authorityIdentifiers_scheme": facets.metadata_creators_authorityIdentifiers_scheme,
+        "metadata_creators_familyName": facets.metadata_creators_familyName,
         "metadata_creators_fullName": facets.metadata_creators_fullName,
+        "metadata_creators_givenName": facets.metadata_creators_givenName,
         "metadata_creators_nameType": facets.metadata_creators_nameType,
         "metadata_dateAvailable": facets.metadata_dateAvailable,
         "metadata_dateIssued": facets.metadata_dateIssued,
-        "metadata_dateModified": facets.metadata_dateModified,
-        "metadata_events_eventLocation_country": (
-            facets.metadata_events_eventLocation_country
-        ),
-        "metadata_events_eventLocation_place": (
-            facets.metadata_events_eventLocation_place
-        ),
-        "metadata_externalLocation_externalLocationURL": (
-            facets.metadata_externalLocation_externalLocationURL
-        ),
+        "metadata_events_eventLocation_country": facets.metadata_events_eventLocation_country,
+        "metadata_events_eventLocation_place": facets.metadata_events_eventLocation_place,
         "metadata_fundingReferences_funder": facets.metadata_fundingReferences_funder,
-        "metadata_fundingReferences_projectID": (
-            facets.metadata_fundingReferences_projectID
-        ),
-        "metadata_geoLocations_geoLocationPlace": (
-            facets.metadata_geoLocations_geoLocationPlace
-        ),
-        "metadata_geoLocations_geoLocationPoint_pointLatitude": (
-            facets.metadata_geoLocations_geoLocationPoint_pointLatitude
-        ),
-        "metadata_geoLocations_geoLocationPoint_pointLongitude": (
-            facets.metadata_geoLocations_geoLocationPoint_pointLongitude
-        ),
+        "metadata_fundingReferences_projectID": facets.metadata_fundingReferences_projectID,
+        "metadata_geoLocations_geoLocationPlace": facets.metadata_geoLocations_geoLocationPlace,
+        "metadata_geoLocations_geoLocationPoint_pointLatitude": facets.metadata_geoLocations_geoLocationPoint_pointLatitude,
+        "metadata_geoLocations_geoLocationPoint_pointLongitude": facets.metadata_geoLocations_geoLocationPoint_pointLongitude,
         "metadata_languages": facets.metadata_languages,
         "metadata_methods_cs": facets.metadata_methods_cs,
         "metadata_methods_en": facets.metadata_methods_en,
         "metadata_methods_lang": facets.metadata_methods_lang,
-        "metadata_objectIdentifiers_identifier": (
-            facets.metadata_objectIdentifiers_identifier
-        ),
+        "metadata_objectIdentifiers_identifier": facets.metadata_objectIdentifiers_identifier,
         "metadata_objectIdentifiers_scheme": facets.metadata_objectIdentifiers_scheme,
         "metadata_originalRecord": facets.metadata_originalRecord,
-        "metadata_relatedItems_itemContributors_affiliations": (
-            facets.metadata_relatedItems_itemContributors_affiliations
-        ),
-        "metadata_relatedItems_itemContributors_authorityIdentifiers_identifier": (
-            facets.metadata_relatedItems_itemContributors_authorityIdentifiers_identifier
-        ),
-        "metadata_relatedItems_itemContributors_authorityIdentifiers_scheme": (
-            facets.metadata_relatedItems_itemContributors_authorityIdentifiers_scheme
-        ),
-        "metadata_relatedItems_itemContributors_fullName": (
-            facets.metadata_relatedItems_itemContributors_fullName
-        ),
-        "metadata_relatedItems_itemContributors_nameType": (
-            facets.metadata_relatedItems_itemContributors_nameType
-        ),
-        "metadata_relatedItems_itemContributors_role": (
-            facets.metadata_relatedItems_itemContributors_role
-        ),
-        "metadata_relatedItems_itemCreators_affiliations": (
-            facets.metadata_relatedItems_itemCreators_affiliations
-        ),
-        "metadata_relatedItems_itemCreators_authorityIdentifiers_identifier": (
-            facets.metadata_relatedItems_itemCreators_authorityIdentifiers_identifier
-        ),
-        "metadata_relatedItems_itemCreators_authorityIdentifiers_scheme": (
-            facets.metadata_relatedItems_itemCreators_authorityIdentifiers_scheme
-        ),
-        "metadata_relatedItems_itemCreators_fullName": (
-            facets.metadata_relatedItems_itemCreators_fullName
-        ),
-        "metadata_relatedItems_itemCreators_nameType": (
-            facets.metadata_relatedItems_itemCreators_nameType
-        ),
+        "metadata_relatedItems_itemContributors_affiliations": facets.metadata_relatedItems_itemContributors_affiliations,
+        "metadata_relatedItems_itemContributors_authorityIdentifiers_identifier": facets.metadata_relatedItems_itemContributors_authorityIdentifiers_identifier,
+        "metadata_relatedItems_itemContributors_authorityIdentifiers_scheme": facets.metadata_relatedItems_itemContributors_authorityIdentifiers_scheme,
+        "metadata_relatedItems_itemContributors_contributorType": facets.metadata_relatedItems_itemContributors_contributorType,
+        "metadata_relatedItems_itemContributors_familyName": facets.metadata_relatedItems_itemContributors_familyName,
+        "metadata_relatedItems_itemContributors_fullName": facets.metadata_relatedItems_itemContributors_fullName,
+        "metadata_relatedItems_itemContributors_givenName": facets.metadata_relatedItems_itemContributors_givenName,
+        "metadata_relatedItems_itemContributors_nameType": facets.metadata_relatedItems_itemContributors_nameType,
+        "metadata_relatedItems_itemCreators_affiliations": facets.metadata_relatedItems_itemCreators_affiliations,
+        "metadata_relatedItems_itemCreators_authorityIdentifiers_identifier": facets.metadata_relatedItems_itemCreators_authorityIdentifiers_identifier,
+        "metadata_relatedItems_itemCreators_authorityIdentifiers_scheme": facets.metadata_relatedItems_itemCreators_authorityIdentifiers_scheme,
+        "metadata_relatedItems_itemCreators_familyName": facets.metadata_relatedItems_itemCreators_familyName,
+        "metadata_relatedItems_itemCreators_fullName": facets.metadata_relatedItems_itemCreators_fullName,
+        "metadata_relatedItems_itemCreators_givenName": facets.metadata_relatedItems_itemCreators_givenName,
+        "metadata_relatedItems_itemCreators_nameType": facets.metadata_relatedItems_itemCreators_nameType,
         "metadata_relatedItems_itemEndPage": facets.metadata_relatedItems_itemEndPage,
         "metadata_relatedItems_itemIssue": facets.metadata_relatedItems_itemIssue,
-        "metadata_relatedItems_itemPIDs_identifier": (
-            facets.metadata_relatedItems_itemPIDs_identifier
-        ),
-        "metadata_relatedItems_itemPIDs_scheme": (
-            facets.metadata_relatedItems_itemPIDs_scheme
-        ),
-        "metadata_relatedItems_itemPublisher": (
-            facets.metadata_relatedItems_itemPublisher
-        ),
-        "metadata_relatedItems_itemRelationType": (
-            facets.metadata_relatedItems_itemRelationType
-        ),
-        "metadata_relatedItems_itemResourceType": (
-            facets.metadata_relatedItems_itemResourceType
-        ),
-        "metadata_relatedItems_itemStartPage": (
-            facets.metadata_relatedItems_itemStartPage
-        ),
+        "metadata_relatedItems_itemPIDs_identifier": facets.metadata_relatedItems_itemPIDs_identifier,
+        "metadata_relatedItems_itemPIDs_scheme": facets.metadata_relatedItems_itemPIDs_scheme,
+        "metadata_relatedItems_itemPublisher": facets.metadata_relatedItems_itemPublisher,
+        "metadata_relatedItems_itemRelationType": facets.metadata_relatedItems_itemRelationType,
+        "metadata_relatedItems_itemResourceType": facets.metadata_relatedItems_itemResourceType,
+        "metadata_relatedItems_itemStartPage": facets.metadata_relatedItems_itemStartPage,
         "metadata_relatedItems_itemURL": facets.metadata_relatedItems_itemURL,
         "metadata_relatedItems_itemVolume": facets.metadata_relatedItems_itemVolume,
         "metadata_relatedItems_itemYear": facets.metadata_relatedItems_itemYear,
         "metadata_resourceType": facets.metadata_resourceType,
         "metadata_rights": facets.metadata_rights,
         "metadata_series_seriesTitle": facets.metadata_series_seriesTitle,
         "metadata_series_seriesVolume": facets.metadata_series_seriesVolume,
         "metadata_subjectCategories": facets.metadata_subjectCategories,
-        "metadata_subjects_classificationCode": (
-            facets.metadata_subjects_classificationCode
-        ),
+        "metadata_subjects_classificationCode": facets.metadata_subjects_classificationCode,
         "metadata_subjects_subject_cs": facets.metadata_subjects_subject_cs,
         "metadata_subjects_subject_en": facets.metadata_subjects_subject_en,
         "metadata_subjects_subject_lang": facets.metadata_subjects_subject_lang,
         "metadata_subjects_subjectScheme": facets.metadata_subjects_subjectScheme,
         "metadata_subjects_valueURI": facets.metadata_subjects_valueURI,
-        "metadata_systemIdentifiers_identifier": (
-            facets.metadata_systemIdentifiers_identifier
-        ),
+        "metadata_systemIdentifiers_identifier": facets.metadata_systemIdentifiers_identifier,
         "metadata_systemIdentifiers_scheme": facets.metadata_systemIdentifiers_scheme,
         "metadata_technicalInfo_cs": facets.metadata_technicalInfo_cs,
         "metadata_technicalInfo_en": facets.metadata_technicalInfo_en,
         "metadata_technicalInfo_lang": facets.metadata_technicalInfo_lang,
-        "metadata_thesis_dateDefended": facets.metadata_thesis_dateDefended,
-        "metadata_thesis_defended": facets.metadata_thesis_defended,
-        "metadata_thesis_degreeGrantors": facets.metadata_thesis_degreeGrantors,
-        "metadata_thesis_studyFields": facets.metadata_thesis_studyFields,
         "metadata_version": facets.metadata_version,
-        "syntheticFields_institutions": facets.syntheticFields_institutions,
-        "syntheticFields_keywords_cs": facets.syntheticFields_keywords_cs,
-        "syntheticFields_keywords_en": facets.syntheticFields_keywords_en,
-        "syntheticFields_person": facets.syntheticFields_person,
         **getattr(InvenioSearchOptions, "facets", {}),
     }
```

### Comparing `nr-metadata-2.0.8/nr_metadata/documents/views/records/api.py` & `nr-metadata-2.0.9/nr_metadata/documents/views/records/api.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-2.0.8/nr_metadata/documents/views/records/app.py` & `nr-metadata-2.0.9/nr_metadata/documents/views/records/app.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-2.0.8/nr_metadata/schema/identifiers.py` & `nr-metadata-2.0.9/nr_metadata/schema/identifiers.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,7 +67,42 @@
         required=True,
         validate=[
             validate.OneOf(
                 ["nusl", "nuslOAI", "originalRecordOAI", "catalogueSysNo", "nrOAI"]
             )
         ],
     )
+
+class NROrganizationIdentifierSchema(NRIdentifierSchema):
+    scheme = ma.fields.String(
+        required=True,
+        validate=[
+            validate.OneOf(
+                [
+
+                    "ISNI",
+                    "ROR",
+                    "ICO",
+                    "DOI",  # normalized
+                ]
+            )
+        ],
+    )
+
+class NRPersonIdentifierSchema(NRIdentifierSchema):
+    scheme = ma.fields.String(
+        required=True,
+        validate=[
+            validate.OneOf(
+                [
+                    "orcid",  # normalized
+                    "scopusID",
+                    "researcherID",
+                    "czenasAutID",
+                    "vedidk",
+                    "institutionalID",
+                    "ISNI",
+
+                ]
+            )
+        ],
+    )
```

### Comparing `nr-metadata-2.0.8/nr_metadata/services/records/facets/dumper.py` & `nr-metadata-2.0.9/nr_metadata/services/records/facets/dumper.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-2.0.8/nr_metadata/ui_schema/subjects.py` & `nr-metadata-2.0.9/nr_metadata/ui_schema/subjects.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-2.0.8/nr_metadata.egg-info/PKG-INFO` & `nr-metadata-2.0.9/nr_metadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nr-metadata
-Version: 2.0.8
+Version: 2.0.9
 Summary: "Generated metadata files for the Czech National Repository"
 Home-page: https://github.com/Narodni-repozitar/ne-metadata
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio Czech NR
 Platform: any
```

### Comparing `nr-metadata-2.0.8/setup.cfg` & `nr-metadata-2.0.9/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -40,14 +40,16 @@
 [options.package_data]
 * = *.json, *.rst, *.md, *.json5, *.jinja2, *.po, *.mo, *.pot
 
 [options.entry_points]
 oarepo.models = 
 	common = nr_metadata.common.models:records.json
 	documents = nr_metadata.documents.models:records.json
+	data = nr_metadata.data.models:records.json
+	datacite = nr_metadata.datacite.models:records.json
 
 [build_sphinx]
 source-dir = docs/
 build-dir = docs/_build
 all_files = 1
 
 [bdist_wheel]
```

