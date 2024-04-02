# Comparing `tmp/nc_py_api-0.8.0.tar.gz` & `tmp/nc_py_api-0.9.0.tar.gz`

## Comparing `nc_py_api-0.8.0.tar` & `nc_py_api-0.9.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
--rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/CHANGELOG.md
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/__init__.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/_deffered_error.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/_exceptions.py
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/_misc.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/_preferences.py
--rw-r--r--   0        0        0     7091 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/_preferences_ex.py
--rw-r--r--   0        0        0    19761 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/_session.py
--rw-r--r--   0        0        0    51033 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/_talk_api.py
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/_theming.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/_version.py
--rw-r--r--   0        0        0     9574 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/activity.py
--rw-r--r--   0        0        0     9774 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/apps.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/calendar.py
--rw-r--r--   0        0        0    22328 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/nextcloud.py
--rw-r--r--   0        0        0    15106 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/notes.py
--rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/notifications.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/options.py
--rw-r--r--   0        0        0    29368 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/talk.py
--rw-r--r--   0        0        0    16526 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/talk_bot.py
--rw-r--r--   0        0        0    13288 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/user_status.py
--rw-r--r--   0        0        0    15488 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/users.py
--rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/users_groups.py
--rw-r--r--   0        0        0     7582 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/weather_status.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/ex_app/__init__.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/ex_app/defs.py
--rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/ex_app/integration_fastapi.py
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/ex_app/misc.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/ex_app/persist_transformers_cache.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/ex_app/uvicorn_fastapi.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/ex_app/providers/__init__.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/ex_app/providers/providers.py
--rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/ex_app/providers/speech_to_text.py
--rw-r--r--   0        0        0     5325 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/ex_app/providers/text_processing.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/ex_app/ui/__init__.py
--rw-r--r--   0        0        0     7412 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/ex_app/ui/files_actions.py
--rw-r--r--   0        0        0    12457 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/ex_app/ui/resources.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/ex_app/ui/top_menu.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/ex_app/ui/ui.py
--rw-r--r--   0        0        0    11798 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/files/__init__.py
--rw-r--r--   0        0        0    12226 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/files/_files.py
--rw-r--r--   0        0        0    44904 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/files/files.py
--rw-r--r--   0        0        0    14395 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/nc_py_api/files/sharing.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/.gitignore
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/AUTHORS
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0     5916 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/README.md
--rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     8778 2020-02-02 00:00:00.000000 nc_py_api-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     9791 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/__init__.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/_deffered_error.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/_exceptions.py
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/_misc.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/_preferences.py
+-rw-r--r--   0        0        0     7091 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/_preferences_ex.py
+-rw-r--r--   0        0        0    19761 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/_session.py
+-rw-r--r--   0        0        0    51033 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/_talk_api.py
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/_theming.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/_version.py
+-rw-r--r--   0        0        0     9574 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/activity.py
+-rw-r--r--   0        0        0     9774 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/apps.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/calendar.py
+-rw-r--r--   0        0        0    22328 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/nextcloud.py
+-rw-r--r--   0        0        0    15106 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/notes.py
+-rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/notifications.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/options.py
+-rw-r--r--   0        0        0    29368 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/talk.py
+-rw-r--r--   0        0        0    16562 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/talk_bot.py
+-rw-r--r--   0        0        0    13288 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/user_status.py
+-rw-r--r--   0        0        0    15488 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/users.py
+-rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/users_groups.py
+-rw-r--r--   0        0        0     7582 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/weather_status.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/ex_app/__init__.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/ex_app/defs.py
+-rw-r--r--   0        0        0     8737 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/ex_app/integration_fastapi.py
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/ex_app/misc.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/ex_app/persist_transformers_cache.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/ex_app/uvicorn_fastapi.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/ex_app/providers/__init__.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/ex_app/providers/providers.py
+-rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/ex_app/providers/speech_to_text.py
+-rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/ex_app/providers/text_processing.py
+-rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/ex_app/providers/translations.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/ex_app/ui/__init__.py
+-rw-r--r--   0        0        0     7412 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/ex_app/ui/files_actions.py
+-rw-r--r--   0        0        0    12457 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/ex_app/ui/resources.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/ex_app/ui/top_menu.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/ex_app/ui/ui.py
+-rw-r--r--   0        0        0    12564 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/files/__init__.py
+-rw-r--r--   0        0        0    12226 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/files/_files.py
+-rw-r--r--   0        0        0    44904 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/files/files.py
+-rw-r--r--   0        0        0    14395 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/nc_py_api/files/sharing.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/.gitignore
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/AUTHORS
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/README.md
+-rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     8791 2020-02-02 00:00:00.000000 nc_py_api-0.9.0/PKG-INFO
```

### Comparing `nc_py_api-0.8.0/CHANGELOG.md` & `nc_py_api-0.9.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [0.9.0 - 2024-01-25]
+
+### Added
+
+- class `Share`: added missing `file_source_id`, `can_edit`, `can_delete` properties. #206
+- NextcloudApp: `AppAPIAuthMiddleware` for easy cover all endpoints. #205
+- NextcloudApp: API for registering `MachineTranslation` providers(*avalaible from Nextcloud 29*). #207
+
+### Changed
+
+- **large amount of incompatible changes** for `AppAPI 2.0`, see PR for description. #212
+- class `Share`.raw_data marked as deprecated and changed to `_raw_data`. #206
+- `ex_app.talk_bot_app`/`ex_app.atalk_bot_app` renamed to `ex_app.talk_bot_msg`/`ex_app.atalk_bot_msg`.
+
 ## [0.8.0 - 2024-01-12]
 
 ### Added
 
 - `download_log` method to download `nextcloud.log`. #199
 - NextcloudApp: API for registering `Speech to Text` providers(*avalaible from Nextcloud 29*). #196
 - NextcloudApp: API for registering `Text Processing` providers(*avalaible from Nextcloud 29*). #198
```

### Comparing `nc_py_api-0.8.0/nc_py_api/_exceptions.py` & `nc_py_api-0.9.0/nc_py_api/_exceptions.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/nc_py_api/_misc.py` & `nc_py_api-0.9.0/nc_py_api/_misc.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/nc_py_api/_preferences.py` & `nc_py_api-0.9.0/nc_py_api/_preferences.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/nc_py_api/_preferences_ex.py` & `nc_py_api-0.9.0/nc_py_api/_preferences_ex.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/nc_py_api/_session.py` & `nc_py_api-0.9.0/nc_py_api/_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from abc import ABC, abstractmethod
 from base64 import b64encode
 from dataclasses import dataclass
 from enum import IntEnum
 from json import loads
 from os import environ
 
-from fastapi import Request as FastAPIRequest
 from httpx import AsyncClient, Client, Headers, Limits, ReadTimeout, Request, Response
+from starlette.requests import HTTPConnection
 
 from . import options
 from ._exceptions import (
     NextcloudException,
     NextcloudExceptionNotFound,
     NextcloudExceptionNotModified,
     check_error,
@@ -455,15 +455,15 @@
     adapter: AsyncClient | Client
     adapter_dav: AsyncClient | Client
 
     def __init__(self, **kwargs):
         self.cfg = AppConfig(**kwargs)
         super().__init__(**kwargs)
 
-    def sign_check(self, request: FastAPIRequest) -> None:
+    def sign_check(self, request: HTTPConnection) -> None:
         headers = {
             "AA-VERSION": request.headers.get("AA-VERSION", ""),
             "EX-APP-ID": request.headers.get("EX-APP-ID", ""),
             "EX-APP-VERSION": request.headers.get("EX-APP-VERSION", ""),
             "AUTHORIZATION-APP-API": request.headers.get("AUTHORIZATION-APP-API", ""),
         }
```

### Comparing `nc_py_api-0.8.0/nc_py_api/_talk_api.py` & `nc_py_api-0.9.0/nc_py_api/_talk_api.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/nc_py_api/_theming.py` & `nc_py_api-0.9.0/nc_py_api/_theming.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/nc_py_api/activity.py` & `nc_py_api-0.9.0/nc_py_api/activity.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/nc_py_api/apps.py` & `nc_py_api-0.9.0/nc_py_api/apps.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/nc_py_api/calendar.py` & `nc_py_api-0.9.0/nc_py_api/calendar.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/nc_py_api/nextcloud.py` & `nc_py_api-0.9.0/nc_py_api/nextcloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Nextcloud class providing access to all API endpoints."""
 
 import typing
 from abc import ABC
 
-from fastapi import Request as FastAPIRequest
 from httpx import Headers
+from starlette.requests import HTTPConnection
 
 from ._exceptions import NextcloudExceptionNotFound
 from ._misc import check_capabilities, require_capabilities
 from ._preferences import AsyncPreferencesAPI, PreferencesAPI
 from ._preferences_ex import (
     AppConfigExAPI,
     AsyncAppConfigExAPI,
@@ -391,15 +391,15 @@
         }
         try:
             self._session.ocs("DELETE", f"{self._session.ae_url}/talk_bot", json=params)
         except NextcloudExceptionNotFound:
             return False
         return True
 
-    def request_sign_check(self, request: FastAPIRequest) -> bool:
+    def request_sign_check(self, request: HTTPConnection) -> bool:
         """Verifies the signature and validity of an incoming request from the Nextcloud.
 
         :param request: The `Starlette request <https://www.starlette.io/requests/>`_
 
         .. note:: In most cases ``nc: Annotated[NextcloudApp, Depends(nc_app)]`` should be used.
         """
         try:
@@ -531,15 +531,15 @@
         }
         try:
             await self._session.ocs("DELETE", f"{self._session.ae_url}/talk_bot", json=params)
         except NextcloudExceptionNotFound:
             return False
         return True
 
-    def request_sign_check(self, request: FastAPIRequest) -> bool:
+    def request_sign_check(self, request: HTTPConnection) -> bool:
         """Verifies the signature and validity of an incoming request from the Nextcloud.
 
         :param request: The `Starlette request <https://www.starlette.io/requests/>`_
 
         .. note:: In most cases ``nc: Annotated[NextcloudApp, Depends(nc_app)]`` should be used.
         """
         try:
```

### Comparing `nc_py_api-0.8.0/nc_py_api/notes.py` & `nc_py_api-0.9.0/nc_py_api/notes.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/nc_py_api/notifications.py` & `nc_py_api-0.9.0/nc_py_api/notifications.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/nc_py_api/options.py` & `nc_py_api-0.9.0/nc_py_api/options.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/nc_py_api/talk.py` & `nc_py_api-0.9.0/nc_py_api/talk.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/nc_py_api/talk_bot.py` & `nc_py_api-0.9.0/nc_py_api/talk_bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     def __init__(self, callback_url: str, display_name: str, description: str = ""):
         """Class implementing Nextcloud Talk Bot functionality.
 
         :param callback_url: FastAPI endpoint which will be assigned to bot.
         :param display_name: The display name of the bot that is shown as author when it posts a message or reaction.
         :param description: Description of the bot helping moderators to decide if they want to enable this bot.
         """
-        self.callback_url = callback_url
+        self.callback_url = callback_url.lstrip("/")
         self.display_name = display_name
         self.description = description
 
     def enabled_handler(self, enabled: bool, nc: NextcloudApp) -> None:
         """Handles the app ``on``/``off`` event in the context of the bot.
 
         :param enabled: Value that was passed to ``/enabled`` handler.
@@ -207,15 +207,15 @@
     def __init__(self, callback_url: str, display_name: str, description: str = ""):
         """Class implementing Nextcloud Talk Bot functionality.
 
         :param callback_url: FastAPI endpoint which will be assigned to bot.
         :param display_name: The display name of the bot that is shown as author when it posts a message or reaction.
         :param description: Description of the bot helping moderators to decide if they want to enable this bot.
         """
-        self.callback_url = callback_url
+        self.callback_url = callback_url.lstrip("/")
         self.display_name = display_name
         self.description = description
 
     async def enabled_handler(self, enabled: bool, nc: AsyncNextcloudApp) -> None:
         """Handles the app ``on``/``off`` event in the context of the bot.
 
         :param enabled: Value that was passed to ``/enabled`` handler.
@@ -314,15 +314,15 @@
                 cookies={"XDEBUG_SESSION": options.XDEBUG_SESSION} if options.XDEBUG_SESSION else {},
                 timeout=nc_app_cfg.options.timeout,
             )
 
 
 def __get_bot_secret(callback_url: str) -> str:
     sha_1 = hashlib.sha1(usedforsecurity=False)
-    string_to_hash = os.environ["APP_ID"] + "_" + callback_url
+    string_to_hash = os.environ["APP_ID"] + "_" + callback_url.lstrip("/")
     sha_1.update(string_to_hash.encode("UTF-8"))
     return sha_1.hexdigest()
 
 
 def get_bot_secret(callback_url: str) -> bytes | None:
     """Returns the bot's secret from an environment variable or from the application's configuration on the server."""
     secret_key = __get_bot_secret(callback_url)
```

### Comparing `nc_py_api-0.8.0/nc_py_api/user_status.py` & `nc_py_api-0.9.0/nc_py_api/user_status.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/nc_py_api/users.py` & `nc_py_api-0.9.0/nc_py_api/users.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/nc_py_api/users_groups.py` & `nc_py_api-0.9.0/nc_py_api/users_groups.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/nc_py_api/weather_status.py` & `nc_py_api-0.9.0/nc_py_api/weather_status.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/nc_py_api/ex_app/defs.py` & `nc_py_api-0.9.0/nc_py_api/ex_app/defs.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/nc_py_api/ex_app/integration_fastapi.py` & `nc_py_api-0.9.0/nc_py_api/ex_app/integration_fastapi.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,77 +1,64 @@
 """FastAPI directly related stuff."""
 
 import asyncio
-import hashlib
-import hmac
 import json
 import os
 import typing
 
 from fastapi import (
     BackgroundTasks,
     Depends,
     FastAPI,
     HTTPException,
-    Request,
     responses,
     staticfiles,
     status,
 )
+from starlette.requests import HTTPConnection, Request
+from starlette.types import ASGIApp, Receive, Scope, Send
 
 from .._misc import get_username_secret_from_headers
 from ..nextcloud import AsyncNextcloudApp, NextcloudApp
-from ..talk_bot import TalkBotMessage, aget_bot_secret, get_bot_secret
+from ..talk_bot import TalkBotMessage
 from .misc import persistent_storage
 
 
-def nc_app(request: Request) -> NextcloudApp:
+def nc_app(request: HTTPConnection) -> NextcloudApp:
     """Authentication handler for requests from Nextcloud to the application."""
     user = get_username_secret_from_headers(
         {"AUTHORIZATION-APP-API": request.headers.get("AUTHORIZATION-APP-API", "")}
     )[0]
     request_id = request.headers.get("AA-REQUEST-ID", None)
     nextcloud_app = NextcloudApp(user=user, headers={"AA-REQUEST-ID": request_id} if request_id else {})
     if not nextcloud_app.request_sign_check(request):
         raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED)
     return nextcloud_app
 
 
-def anc_app(request: Request) -> AsyncNextcloudApp:
+def anc_app(request: HTTPConnection) -> AsyncNextcloudApp:
     """Async Authentication handler for requests from Nextcloud to the application."""
     user = get_username_secret_from_headers(
         {"AUTHORIZATION-APP-API": request.headers.get("AUTHORIZATION-APP-API", "")}
     )[0]
     request_id = request.headers.get("AA-REQUEST-ID", None)
     nextcloud_app = AsyncNextcloudApp(user=user, headers={"AA-REQUEST-ID": request_id} if request_id else {})
     if not nextcloud_app.request_sign_check(request):
         raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED)
     return nextcloud_app
 
 
-def __talk_bot_app(secret: bytes | None, request: Request, body: bytes) -> TalkBotMessage:
-    if not secret:
-        raise HTTPException(status_code=status.HTTP_500_INTERNAL_SERVER_ERROR)
-    hmac_sign = hmac.new(
-        secret, request.headers.get("X-NEXTCLOUD-TALK-RANDOM", "").encode("UTF-8"), digestmod=hashlib.sha256
-    )
-    hmac_sign.update(body)
-    if request.headers["X-NEXTCLOUD-TALK-SIGNATURE"] != hmac_sign.hexdigest():
-        raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED)
-    return TalkBotMessage(json.loads(body))
-
-
-def talk_bot_app(request: Request) -> TalkBotMessage:
+def talk_bot_msg(request: Request) -> TalkBotMessage:
     """Authentication handler for bot requests from Nextcloud Talk to the application."""
-    return __talk_bot_app(get_bot_secret(request.url.components.path), request, asyncio.run(request.body()))
+    return TalkBotMessage(json.loads(asyncio.run(request.body())))
 
 
-async def atalk_bot_app(request: Request) -> TalkBotMessage:
+async def atalk_bot_msg(request: Request) -> TalkBotMessage:
     """Async Authentication handler for bot requests from Nextcloud Talk to the application."""
-    return __talk_bot_app(await aget_bot_secret(request.url.components.path), request, await request.body())
+    return TalkBotMessage(json.loads(await request.body()))
 
 
 def set_handlers(
     fast_api_app: FastAPI,
     enabled_handler: typing.Callable[[bool, AsyncNextcloudApp | NextcloudApp], typing.Awaitable[str] | str],
     heartbeat_handler: typing.Callable[[], typing.Awaitable[str] | str] | None = None,
     init_handler: typing.Callable[[AsyncNextcloudApp | NextcloudApp], typing.Awaitable[None] | None] | None = None,
@@ -190,7 +177,44 @@
                 return super().display(msg, pos)
 
         for model in models:
             workers = models[model].pop("max_workers", 2)
             cache = models[model].pop("cache_dir", persistent_storage())
             snapshot_download(model, tqdm_class=TqdmProgress, **models[model], max_workers=workers, cache_dir=cache)
     nc.set_init_status(100)
+
+
+class AppAPIAuthMiddleware:
+    """Pure ASGI AppAPIAuth Middleware."""
+
+    _disable_for: list[str]
+
+    def __init__(
+        self,
+        app: ASGIApp,
+        disable_for: list[str] | None = None,
+    ) -> None:
+        self.app = app
+        disable_for = [] if disable_for is None else [i.lstrip("/") for i in disable_for]
+        self._disable_for = [i for i in disable_for if i != "heartbeat"] + ["heartbeat"]
+
+    async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
+        """Method that will be called by Starlette for each event."""
+        if scope["type"] != "http":
+            await self.app(scope, receive, send)
+            return
+
+        conn = HTTPConnection(scope)
+        url_path = conn.url.path.lstrip("/")
+        if url_path not in self._disable_for:
+            try:
+                anc_app(conn)
+            except HTTPException as exc:
+                response = self._on_error(exc.status_code, exc.detail)
+                await response(scope, receive, send)
+                return
+
+        await self.app(scope, receive, send)
+
+    @staticmethod
+    def _on_error(status_code: int = 400, content: str = "") -> responses.PlainTextResponse:
+        return responses.PlainTextResponse(content, status_code=status_code)
```

### Comparing `nc_py_api-0.8.0/nc_py_api/ex_app/misc.py` & `nc_py_api-0.9.0/nc_py_api/ex_app/misc.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/nc_py_api/ex_app/uvicorn_fastapi.py` & `nc_py_api-0.9.0/nc_py_api/ex_app/uvicorn_fastapi.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/nc_py_api/ex_app/providers/speech_to_text.py` & `nc_py_api-0.9.0/nc_py_api/ex_app/providers/speech_to_text.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import contextlib
 import dataclasses
 
 from ..._exceptions import NextcloudException, NextcloudExceptionNotFound
 from ..._misc import require_capabilities
 from ..._session import AsyncNcSessionApp, NcSessionApp
 
+_EP_SUFFIX: str = "ai_provider/speech_to_text"
+
 
 @dataclasses.dataclass
 class SpeechToTextProvider:
     """Speech2Text provider description."""
 
     def __init__(self, raw_data: dict):
         self._raw_data = raw_data
@@ -31,100 +33,96 @@
         return self._raw_data["action_handler"]
 
     def __repr__(self):
         return f"<{self.__class__.__name__} name={self.name}, handler={self.action_handler}>"
 
 
 class _SpeechToTextProviderAPI:
-    """API for registering Speech2Text providers."""
-
-    _ep_suffix: str = "ai_provider/speech_to_text"
+    """API for Speech2Text providers."""
 
     def __init__(self, session: NcSessionApp):
         self._session = session
 
     def register(self, name: str, display_name: str, callback_url: str) -> None:
         """Registers or edit the SpeechToText provider."""
         require_capabilities("app_api", self._session.capabilities)
         params = {
             "name": name,
             "displayName": display_name,
             "actionHandler": callback_url,
         }
-        self._session.ocs("POST", f"{self._session.ae_url}/{self._ep_suffix}", json=params)
+        self._session.ocs("POST", f"{self._session.ae_url}/{_EP_SUFFIX}", json=params)
 
     def unregister(self, name: str, not_fail=True) -> None:
         """Removes SpeechToText provider."""
         require_capabilities("app_api", self._session.capabilities)
         try:
-            self._session.ocs("DELETE", f"{self._session.ae_url}/{self._ep_suffix}", params={"name": name})
+            self._session.ocs("DELETE", f"{self._session.ae_url}/{_EP_SUFFIX}", params={"name": name})
         except NextcloudExceptionNotFound as e:
             if not not_fail:
                 raise e from None
 
     def get_entry(self, name: str) -> SpeechToTextProvider | None:
         """Get information of the SpeechToText."""
         require_capabilities("app_api", self._session.capabilities)
         try:
             return SpeechToTextProvider(
-                self._session.ocs("GET", f"{self._session.ae_url}/{self._ep_suffix}", params={"name": name})
+                self._session.ocs("GET", f"{self._session.ae_url}/{_EP_SUFFIX}", params={"name": name})
             )
         except NextcloudExceptionNotFound:
             return None
 
     def report_result(self, task_id: int, result: str = "", error: str = "") -> None:
         """Report results of speech to text task to Nextcloud."""
         require_capabilities("app_api", self._session.capabilities)
         with contextlib.suppress(NextcloudException):
             self._session.ocs(
                 "PUT",
-                f"{self._session.ae_url}/{self._ep_suffix}",
+                f"{self._session.ae_url}/{_EP_SUFFIX}",
                 json={"taskId": task_id, "result": result, "error": error},
             )
 
 
 class _AsyncSpeechToTextProviderAPI:
-    """API for registering Speech2Text providers."""
-
-    _ep_suffix: str = "ai_provider/speech_to_text"
+    """API for Speech2Text providers."""
 
     def __init__(self, session: AsyncNcSessionApp):
         self._session = session
 
     async def register(self, name: str, display_name: str, callback_url: str) -> None:
         """Registers or edit the SpeechToText provider."""
         require_capabilities("app_api", await self._session.capabilities)
         params = {
             "name": name,
             "displayName": display_name,
             "actionHandler": callback_url,
         }
-        await self._session.ocs("POST", f"{self._session.ae_url}/{self._ep_suffix}", json=params)
+        await self._session.ocs("POST", f"{self._session.ae_url}/{_EP_SUFFIX}", json=params)
 
     async def unregister(self, name: str, not_fail=True) -> None:
         """Removes SpeechToText provider."""
         require_capabilities("app_api", await self._session.capabilities)
         try:
-            await self._session.ocs("DELETE", f"{self._session.ae_url}/{self._ep_suffix}", params={"name": name})
+            await self._session.ocs("DELETE", f"{self._session.ae_url}/{_EP_SUFFIX}", params={"name": name})
         except NextcloudExceptionNotFound as e:
             if not not_fail:
                 raise e from None
 
     async def get_entry(self, name: str) -> SpeechToTextProvider | None:
         """Get information of the SpeechToText."""
         require_capabilities("app_api", await self._session.capabilities)
         try:
             return SpeechToTextProvider(
-                await self._session.ocs("GET", f"{self._session.ae_url}/{self._ep_suffix}", params={"name": name})
+                await self._session.ocs("GET", f"{self._session.ae_url}/{_EP_SUFFIX}", params={"name": name})
             )
         except NextcloudExceptionNotFound:
             return None
 
     async def report_result(self, task_id: int, result: str = "", error: str = "") -> None:
         """Report results of speech to text task to Nextcloud."""
         require_capabilities("app_api", await self._session.capabilities)
         with contextlib.suppress(NextcloudException):
             await self._session.ocs(
                 "PUT",
-                f"{self._session.ae_url}/{self._ep_suffix}",
+                f"{self._session.ae_url}/{_EP_SUFFIX}",
                 json={"taskId": task_id, "result": result, "error": error},
             )
```

### Comparing `nc_py_api-0.8.0/nc_py_api/ex_app/providers/text_processing.py` & `nc_py_api-0.9.0/nc_py_api/ex_app/providers/text_processing.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import contextlib
 import dataclasses
 
 from ..._exceptions import NextcloudException, NextcloudExceptionNotFound
 from ..._misc import require_capabilities
 from ..._session import AsyncNcSessionApp, NcSessionApp
 
+_EP_SUFFIX: str = "ai_provider/text_processing"
+
 
 @dataclasses.dataclass
 class TextProcessingProvider:
     """TextProcessing provider description."""
 
     def __init__(self, raw_data: dict):
         self._raw_data = raw_data
@@ -36,102 +38,98 @@
         return self._raw_data["task_type"]
 
     def __repr__(self):
         return f"<{self.__class__.__name__} name={self.name}, type={self.task_type}, handler={self.action_handler}>"
 
 
 class _TextProcessingProviderAPI:
-    """API for registering TextProcessing providers."""
-
-    _ep_suffix: str = "ai_provider/text_processing"
+    """API for TextProcessing providers."""
 
     def __init__(self, session: NcSessionApp):
         self._session = session
 
     def register(self, name: str, display_name: str, callback_url: str, task_type: str) -> None:
         """Registers or edit the TextProcessing provider."""
         require_capabilities("app_api", self._session.capabilities)
         params = {
             "name": name,
             "displayName": display_name,
             "actionHandler": callback_url,
             "taskType": task_type,
         }
-        self._session.ocs("POST", f"{self._session.ae_url}/{self._ep_suffix}", json=params)
+        self._session.ocs("POST", f"{self._session.ae_url}/{_EP_SUFFIX}", json=params)
 
     def unregister(self, name: str, not_fail=True) -> None:
         """Removes TextProcessing provider."""
         require_capabilities("app_api", self._session.capabilities)
         try:
-            self._session.ocs("DELETE", f"{self._session.ae_url}/{self._ep_suffix}", params={"name": name})
+            self._session.ocs("DELETE", f"{self._session.ae_url}/{_EP_SUFFIX}", params={"name": name})
         except NextcloudExceptionNotFound as e:
             if not not_fail:
                 raise e from None
 
     def get_entry(self, name: str) -> TextProcessingProvider | None:
         """Get information of the TextProcessing."""
         require_capabilities("app_api", self._session.capabilities)
         try:
             return TextProcessingProvider(
-                self._session.ocs("GET", f"{self._session.ae_url}/{self._ep_suffix}", params={"name": name})
+                self._session.ocs("GET", f"{self._session.ae_url}/{_EP_SUFFIX}", params={"name": name})
             )
         except NextcloudExceptionNotFound:
             return None
 
     def report_result(self, task_id: int, result: str = "", error: str = "") -> None:
         """Report results of the text processing to Nextcloud."""
         require_capabilities("app_api", self._session.capabilities)
         with contextlib.suppress(NextcloudException):
             self._session.ocs(
                 "PUT",
-                f"{self._session.ae_url}/{self._ep_suffix}",
+                f"{self._session.ae_url}/{_EP_SUFFIX}",
                 json={"taskId": task_id, "result": result, "error": error},
             )
 
 
 class _AsyncTextProcessingProviderAPI:
-    """API for registering TextProcessing providers."""
-
-    _ep_suffix: str = "ai_provider/text_processing"
+    """API for TextProcessing providers."""
 
     def __init__(self, session: AsyncNcSessionApp):
         self._session = session
 
     async def register(self, name: str, display_name: str, callback_url: str, task_type: str) -> None:
         """Registers or edit the TextProcessing provider."""
         require_capabilities("app_api", await self._session.capabilities)
         params = {
             "name": name,
             "displayName": display_name,
             "actionHandler": callback_url,
             "taskType": task_type,
         }
-        await self._session.ocs("POST", f"{self._session.ae_url}/{self._ep_suffix}", json=params)
+        await self._session.ocs("POST", f"{self._session.ae_url}/{_EP_SUFFIX}", json=params)
 
     async def unregister(self, name: str, not_fail=True) -> None:
         """Removes TextProcessing provider."""
         require_capabilities("app_api", await self._session.capabilities)
         try:
-            await self._session.ocs("DELETE", f"{self._session.ae_url}/{self._ep_suffix}", params={"name": name})
+            await self._session.ocs("DELETE", f"{self._session.ae_url}/{_EP_SUFFIX}", params={"name": name})
         except NextcloudExceptionNotFound as e:
             if not not_fail:
                 raise e from None
 
     async def get_entry(self, name: str) -> TextProcessingProvider | None:
         """Get information of the TextProcessing."""
         require_capabilities("app_api", await self._session.capabilities)
         try:
             return TextProcessingProvider(
-                await self._session.ocs("GET", f"{self._session.ae_url}/{self._ep_suffix}", params={"name": name})
+                await self._session.ocs("GET", f"{self._session.ae_url}/{_EP_SUFFIX}", params={"name": name})
             )
         except NextcloudExceptionNotFound:
             return None
 
     async def report_result(self, task_id: int, result: str = "", error: str = "") -> None:
         """Report results of the text processing to Nextcloud."""
         require_capabilities("app_api", await self._session.capabilities)
         with contextlib.suppress(NextcloudException):
             await self._session.ocs(
                 "PUT",
-                f"{self._session.ae_url}/{self._ep_suffix}",
+                f"{self._session.ae_url}/{_EP_SUFFIX}",
                 json={"taskId": task_id, "result": result, "error": error},
             )
```

### Comparing `nc_py_api-0.8.0/nc_py_api/ex_app/ui/files_actions.py` & `nc_py_api-0.9.0/nc_py_api/ex_app/ui/files_actions.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/nc_py_api/ex_app/ui/resources.py` & `nc_py_api-0.9.0/nc_py_api/ex_app/ui/resources.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/nc_py_api/ex_app/ui/top_menu.py` & `nc_py_api-0.9.0/nc_py_api/ex_app/ui/top_menu.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/nc_py_api/ex_app/ui/ui.py` & `nc_py_api-0.9.0/nc_py_api/ex_app/ui/ui.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/nc_py_api/files/__init__.py` & `nc_py_api-0.9.0/nc_py_api/files/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """APIs related to Files and Shares."""
 
 import dataclasses
 import datetime
 import email.utils
 import enum
+import warnings
 
 from .. import _misc
 
 
 @dataclasses.dataclass
 class FsNodeInfo:
     """Extra FS object attributes from Nextcloud."""
@@ -295,84 +296,107 @@
     """Share to the Reva instance(Science Mesh)"""
 
 
 class Share:
     """Information about Share."""
 
     def __init__(self, raw_data: dict):
-        self.raw_data = raw_data
+        self._raw_data = raw_data
+
+    def __getattr__(self, name):
+        if name == "raw_data":
+            warnings.warn(
+                f"{name} is deprecated and will be removed in 0.10.0 version.", DeprecationWarning, stacklevel=2
+            )
+            return self._raw_data
+        return getattr(self, name)
 
     @property
     def share_id(self) -> int:
         """Unique ID of the share."""
-        return int(self.raw_data["id"])
+        return int(self._raw_data["id"])
 
     @property
     def share_type(self) -> ShareType:
         """Type of the share."""
-        return ShareType(int(self.raw_data["share_type"]))
+        return ShareType(int(self._raw_data["share_type"]))
 
     @property
     def share_with(self) -> str:
         """To whom Share was created."""
-        return self.raw_data["share_with"]
+        return self._raw_data["share_with"]
 
     @property
     def permissions(self) -> FilePermissions:
         """Recipient permissions."""
-        return FilePermissions(int(self.raw_data["permissions"]))
+        return FilePermissions(int(self._raw_data["permissions"]))
 
     @property
     def url(self) -> str:
         """URL at which Share is avalaible."""
-        return self.raw_data.get("url", "")
+        return self._raw_data.get("url", "")
 
     @property
     def path(self) -> str:
         """Share path relative to the user's root directory."""
-        return self.raw_data.get("path", "").lstrip("/")
+        return self._raw_data.get("path", "").lstrip("/")
 
     @property
     def label(self) -> str:
         """Label for the Shared object."""
-        return self.raw_data.get("label", "")
+        return self._raw_data.get("label", "")
 
     @property
     def note(self) -> str:
         """Note for the Shared object."""
-        return self.raw_data.get("note", "")
+        return self._raw_data.get("note", "")
 
     @property
     def mimetype(self) -> str:
         """Mimetype of the Shared object."""
-        return self.raw_data.get("mimetype", "")
+        return self._raw_data.get("mimetype", "")
 
     @property
     def share_owner(self) -> str:
         """Share's creator ID."""
-        return self.raw_data.get("uid_owner", "")
+        return self._raw_data.get("uid_owner", "")
 
     @property
     def file_owner(self) -> str:
         """File/directory owner ID."""
-        return self.raw_data.get("uid_file_owner", "")
+        return self._raw_data.get("uid_file_owner", "")
 
     @property
     def password(self) -> str:
         """Password to access share."""
-        return self.raw_data.get("password", "")
+        return self._raw_data.get("password", "")
 
     @property
     def send_password_by_talk(self) -> bool:
         """Flag indicating was password send by Talk."""
-        return self.raw_data.get("send_password_by_talk", False)
+        return self._raw_data.get("send_password_by_talk", False)
 
     @property
     def expire_date(self) -> datetime.datetime:
         """Share expiration time."""
-        return _misc.nc_iso_time_to_datetime(self.raw_data.get("expiration", ""))
+        return _misc.nc_iso_time_to_datetime(self._raw_data.get("expiration", ""))
+
+    @property
+    def file_source_id(self) -> int:
+        """File source ID."""
+        return self._raw_data.get("file_source", 0)
+
+    @property
+    def can_edit(self) -> bool:
+        """Does caller have ``write`` permissions."""
+        return self._raw_data.get("can_edit", False)
+
+    @property
+    def can_delete(self) -> bool:
+        """Does caller have ``delete`` permissions."""
+        return self._raw_data.get("can_delete", False)
 
     def __str__(self):
         return (
             f"{self.share_type.name}: `{self.path}` with id={self.share_id}"
             f" from {self.share_owner} to {self.share_with}"
         )
```

### Comparing `nc_py_api-0.8.0/nc_py_api/files/_files.py` & `nc_py_api-0.9.0/nc_py_api/files/_files.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/nc_py_api/files/files.py` & `nc_py_api-0.9.0/nc_py_api/files/files.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/nc_py_api/files/sharing.py` & `nc_py_api-0.9.0/nc_py_api/files/sharing.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/.gitignore` & `nc_py_api-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/AUTHORS` & `nc_py_api-0.9.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/LICENSE.txt` & `nc_py_api-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/README.md` & `nc_py_api-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 | Users & Groups        |      ✅       |      ✅       |      ✅       |      ✅       |
 | User & Weather status |      ✅       |      ✅       |      ✅       |      ✅       |
 | Other APIs***         |      ✅       |      ✅       |      ✅       |      ✅       |
 | Talk Bot API*         |     N/A      |      ✅       |      ✅       |      ✅       |
 | AI Providers API**    |     N/A      |     N/A      |     N/A      |      ✅       |
 
 &ast;_available only for **NextcloudApp**_<br>
-&ast;&ast;_available only for **NextcloudApp**: SpeechToText, TextProcessing_<br>
+&ast;&ast;_available only for **NextcloudApp**: SpeechToText, TextProcessing, Translation_<br>
 &ast;&ast;&ast;_Activity, Notes_
 
 ### Differences between the Nextcloud and NextcloudApp classes
 
 The **Nextcloud** class functions as a standard Nextcloud client,
 enabling you to make API requests using a username and password.
```

### Comparing `nc_py_api-0.8.0/pyproject.toml` & `nc_py_api-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.8.0/PKG-INFO` & `nc_py_api-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nc-py-api
-Version: 0.8.0
+Version: 0.9.0
 Summary: Nextcloud Python Framework
 Project-URL: Changelog, https://github.com/cloud-py-api/nc_py_api/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://cloud-py-api.github.io/nc_py_api/
 Project-URL: Source, https://github.com/cloud-py-api/nc_py_api
 Author-email: Alexander Piskun <bigcat88@icloud.com>
 License-Expression: BSD-3-Clause
 License-File: AUTHORS
@@ -99,15 +99,15 @@
 | Users & Groups        |      ✅       |      ✅       |      ✅       |      ✅       |
 | User & Weather status |      ✅       |      ✅       |      ✅       |      ✅       |
 | Other APIs***         |      ✅       |      ✅       |      ✅       |      ✅       |
 | Talk Bot API*         |     N/A      |      ✅       |      ✅       |      ✅       |
 | AI Providers API**    |     N/A      |     N/A      |     N/A      |      ✅       |
 
 &ast;_available only for **NextcloudApp**_<br>
-&ast;&ast;_available only for **NextcloudApp**: SpeechToText, TextProcessing_<br>
+&ast;&ast;_available only for **NextcloudApp**: SpeechToText, TextProcessing, Translation_<br>
 &ast;&ast;&ast;_Activity, Notes_
 
 ### Differences between the Nextcloud and NextcloudApp classes
 
 The **Nextcloud** class functions as a standard Nextcloud client,
 enabling you to make API requests using a username and password.
```

