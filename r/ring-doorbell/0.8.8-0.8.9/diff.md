# Comparing `tmp/ring_doorbell-0.8.8.tar.gz` & `tmp/ring_doorbell-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ring_doorbell-0.8.8.tar", max compression
+gzip compressed data, was "ring_doorbell-0.8.9.tar", max compression
```

## Comparing `ring_doorbell-0.8.8.tar` & `ring_doorbell-0.8.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      160 2024-03-18 10:26:12.423655 ring_doorbell-0.8.8/CHANGELOG.rst
--rw-r--r--   0        0        0     4723 2024-03-18 10:26:12.427656 ring_doorbell-0.8.8/CONTRIBUTING.rst
--rw-r--r--   0        0        0     7652 2024-03-18 10:26:12.427656 ring_doorbell-0.8.8/LICENSE
--rw-r--r--   0        0        0     8567 2024-03-18 10:26:12.427656 ring_doorbell-0.8.8/README.rst
--rw-r--r--   0        0        0     3100 2024-03-18 10:26:12.427656 ring_doorbell-0.8.8/pyproject.toml
--rw-r--r--   0        0        0      924 2024-03-18 10:26:12.427656 ring_doorbell-0.8.8/ring_doorbell/__init__.py
--rw-r--r--   0        0        0     5336 2024-03-18 10:26:12.427656 ring_doorbell-0.8.8/ring_doorbell/auth.py
--rw-r--r--   0        0        0     2486 2024-03-18 10:26:12.427656 ring_doorbell-0.8.8/ring_doorbell/chime.py
--rw-r--r--   0        0        0    19438 2024-03-18 10:26:12.427656 ring_doorbell-0.8.8/ring_doorbell/cli.py
--rw-r--r--   0        0        0     6478 2024-03-18 10:26:12.427656 ring_doorbell-0.8.8/ring_doorbell/const.py
--rw-r--r--   0        0        0    14377 2024-03-18 10:26:12.427656 ring_doorbell-0.8.8/ring_doorbell/doorbot.py
--rw-r--r--   0        0        0      426 2024-03-18 10:26:12.427656 ring_doorbell-0.8.8/ring_doorbell/event.py
--rw-r--r--   0        0        0      361 2024-03-18 10:26:12.427656 ring_doorbell-0.8.8/ring_doorbell/exceptions.py
--rw-r--r--   0        0        0     6442 2024-03-18 10:26:12.427656 ring_doorbell-0.8.8/ring_doorbell/generic.py
--rw-r--r--   0        0        0     2982 2024-03-18 10:26:12.427656 ring_doorbell-0.8.8/ring_doorbell/group.py
--rw-r--r--   0        0        0      395 2024-03-18 10:26:12.427656 ring_doorbell-0.8.8/ring_doorbell/listen/__init__.py
--rw-r--r--   0        0        0     7368 2024-03-18 10:26:12.427656 ring_doorbell-0.8.8/ring_doorbell/listen/eventlistener.py
--rw-r--r--   0        0        0      555 2024-03-18 10:26:12.427656 ring_doorbell-0.8.8/ring_doorbell/listen/listenerconfig.py
--rw-r--r--   0        0        0     8751 2024-03-18 10:26:12.427656 ring_doorbell-0.8.8/ring_doorbell/other.py
--rw-r--r--   0        0        0     7905 2024-03-18 10:26:12.427656 ring_doorbell-0.8.8/ring_doorbell/ring.py
--rw-r--r--   0        0        0     6150 2024-03-18 10:26:12.427656 ring_doorbell-0.8.8/ring_doorbell/stickup_cam.py
--rwxr-xr-x   0        0        0      483 2024-03-18 10:26:12.427656 ring_doorbell-0.8.8/scripts/ringcli.py
--rw-r--r--   0        0        0       43 2024-03-18 10:26:12.427656 ring_doorbell-0.8.8/tests/__init__.py
--rw-r--r--   0        0        0     5706 2024-03-18 10:26:12.427656 ring_doorbell-0.8.8/tests/conftest.py
--rw-r--r--   0        0        0      566 2024-03-18 10:26:12.427656 ring_doorbell-0.8.8/tests/fixtures/ring_chime_health_attrs.json
--rw-r--r--   0        0        0    15069 2024-03-18 10:26:12.427656 ring_doorbell-0.8.8/tests/fixtures/ring_devices.json
--rw-r--r--   0        0        0    10468 2024-03-18 10:26:12.427656 ring_doorbell-0.8.8/tests/fixtures/ring_devices_updated.json
--rw-r--r--   0        0        0     2451 2024-03-18 10:26:12.427656 ring_doorbell-0.8.8/tests/fixtures/ring_ding_active.json
--rw-r--r--   0        0        0      566 2024-03-18 10:26:12.427656 ring_doorbell-0.8.8/tests/fixtures/ring_doorboot_health_attrs.json
--rw-r--r--   0        0        0      566 2024-03-18 10:26:12.431656 ring_doorbell-0.8.8/tests/fixtures/ring_doorboot_health_attrs_id987653.json
--rw-r--r--   0        0        0      664 2024-03-18 10:26:12.431656 ring_doorbell-0.8.8/tests/fixtures/ring_doorbot_history.json
--rw-r--r--   0        0        0      743 2024-03-18 10:26:12.431656 ring_doorbell-0.8.8/tests/fixtures/ring_group_devices.json
--rw-r--r--   0        0        0      786 2024-03-18 10:26:12.431656 ring_doorbell-0.8.8/tests/fixtures/ring_groups.json
--rw-r--r--   0        0        0     2663 2024-03-18 10:26:12.431656 ring_doorbell-0.8.8/tests/fixtures/ring_intercom_history.json
--rw-r--r--   0        0        0    10602 2024-03-18 10:26:12.431656 ring_doorbell-0.8.8/tests/fixtures/ring_intercom_settings.json
--rw-r--r--   0        0        0      661 2024-03-18 10:26:12.431656 ring_doorbell-0.8.8/tests/fixtures/ring_intercom_users.json
--rw-r--r--   0        0        0      347 2024-03-18 10:26:12.431656 ring_doorbell-0.8.8/tests/fixtures/ring_listen_credentials.json
--rw-r--r--   0        0        0      834 2024-03-18 10:26:12.431656 ring_doorbell-0.8.8/tests/fixtures/ring_listen_ding.json
--rw-r--r--   0        0        0      181 2024-03-18 10:26:12.431656 ring_doorbell-0.8.8/tests/fixtures/ring_listen_fcmdata.json
--rw-r--r--   0        0        0      302 2024-03-18 10:26:12.431656 ring_doorbell-0.8.8/tests/fixtures/ring_listen_intercom_unlock.json
--rw-r--r--   0        0        0      970 2024-03-18 10:26:12.431656 ring_doorbell-0.8.8/tests/fixtures/ring_listen_motion.json
--rw-r--r--   0        0        0      201 2024-03-18 10:26:12.431656 ring_doorbell-0.8.8/tests/fixtures/ring_oauth.json
--rw-r--r--   0        0        0     1248 2024-03-18 10:26:12.431656 ring_doorbell-0.8.8/tests/fixtures/ring_session.json
--rw-r--r--   0        0        0     7890 2024-03-18 10:26:12.431656 ring_doorbell-0.8.8/tests/test_cli.py
--rw-r--r--   0        0        0     7633 2024-03-18 10:26:12.431656 ring_doorbell-0.8.8/tests/test_listen.py
--rw-r--r--   0        0        0     3769 2024-03-18 10:26:12.431656 ring_doorbell-0.8.8/tests/test_other.py
--rw-r--r--   0        0        0     5286 2024-03-18 10:26:12.431656 ring_doorbell-0.8.8/tests/test_ring.py
--rw-r--r--   0        0        0    10259 1970-01-01 00:00:00.000000 ring_doorbell-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0      160 2024-04-02 10:33:33.511656 ring_doorbell-0.8.9/CHANGELOG.rst
+-rw-r--r--   0        0        0     4723 2024-04-02 10:33:33.511656 ring_doorbell-0.8.9/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     7652 2024-04-02 10:33:33.511656 ring_doorbell-0.8.9/LICENSE
+-rw-r--r--   0        0        0     8909 2024-04-02 10:33:33.511656 ring_doorbell-0.8.9/README.rst
+-rw-r--r--   0        0        0     3432 2024-04-02 10:33:33.511656 ring_doorbell-0.8.9/pyproject.toml
+-rw-r--r--   0        0        0     1061 2024-04-02 10:33:33.511656 ring_doorbell-0.8.9/ring_doorbell/__init__.py
+-rw-r--r--   0        0        0     5789 2024-04-02 10:33:33.511656 ring_doorbell-0.8.9/ring_doorbell/auth.py
+-rw-r--r--   0        0        0     2956 2024-04-02 10:33:33.511656 ring_doorbell-0.8.9/ring_doorbell/chime.py
+-rw-r--r--   0        0        0    20178 2024-04-02 10:33:33.511656 ring_doorbell-0.8.9/ring_doorbell/cli.py
+-rw-r--r--   0        0        0     7423 2024-04-02 10:33:33.511656 ring_doorbell-0.8.9/ring_doorbell/const.py
+-rw-r--r--   0        0        0    14941 2024-04-02 10:33:33.511656 ring_doorbell-0.8.9/ring_doorbell/doorbot.py
+-rw-r--r--   0        0        0      493 2024-04-02 10:33:33.511656 ring_doorbell-0.8.9/ring_doorbell/event.py
+-rw-r--r--   0        0        0      361 2024-04-02 10:33:33.511656 ring_doorbell-0.8.9/ring_doorbell/exceptions.py
+-rw-r--r--   0        0        0     7191 2024-04-02 10:33:33.511656 ring_doorbell-0.8.9/ring_doorbell/generic.py
+-rw-r--r--   0        0        0     3498 2024-04-02 10:33:33.511656 ring_doorbell-0.8.9/ring_doorbell/group.py
+-rw-r--r--   0        0        0      395 2024-04-02 10:33:33.511656 ring_doorbell-0.8.9/ring_doorbell/listen/__init__.py
+-rw-r--r--   0        0        0     8266 2024-04-02 10:33:33.511656 ring_doorbell-0.8.9/ring_doorbell/listen/eventlistener.py
+-rw-r--r--   0        0        0      466 2024-04-02 10:33:33.511656 ring_doorbell-0.8.9/ring_doorbell/listen/listenerconfig.py
+-rw-r--r--   0        0        0     9181 2024-04-02 10:33:33.511656 ring_doorbell-0.8.9/ring_doorbell/other.py
+-rw-r--r--   0        0        0    11450 2024-04-02 10:33:33.511656 ring_doorbell-0.8.9/ring_doorbell/ring.py
+-rw-r--r--   0        0        0     6213 2024-04-02 10:33:33.511656 ring_doorbell-0.8.9/ring_doorbell/stickup_cam.py
+-rwxr-xr-x   0        0        0      483 2024-04-02 10:33:33.511656 ring_doorbell-0.8.9/scripts/ringcli.py
+-rw-r--r--   0        0        0       43 2024-04-02 10:33:33.511656 ring_doorbell-0.8.9/tests/__init__.py
+-rw-r--r--   0        0        0     5706 2024-04-02 10:33:33.511656 ring_doorbell-0.8.9/tests/conftest.py
+-rw-r--r--   0        0        0      566 2024-04-02 10:33:33.511656 ring_doorbell-0.8.9/tests/fixtures/ring_chime_health_attrs.json
+-rw-r--r--   0        0        0    16691 2024-04-02 10:33:33.511656 ring_doorbell-0.8.9/tests/fixtures/ring_devices.json
+-rw-r--r--   0        0        0    10468 2024-04-02 10:33:33.511656 ring_doorbell-0.8.9/tests/fixtures/ring_devices_updated.json
+-rw-r--r--   0        0        0     2451 2024-04-02 10:33:33.515656 ring_doorbell-0.8.9/tests/fixtures/ring_ding_active.json
+-rw-r--r--   0        0        0      566 2024-04-02 10:33:33.515656 ring_doorbell-0.8.9/tests/fixtures/ring_doorboot_health_attrs.json
+-rw-r--r--   0        0        0      566 2024-04-02 10:33:33.515656 ring_doorbell-0.8.9/tests/fixtures/ring_doorboot_health_attrs_id987653.json
+-rw-r--r--   0        0        0      664 2024-04-02 10:33:33.515656 ring_doorbell-0.8.9/tests/fixtures/ring_doorbot_history.json
+-rw-r--r--   0        0        0      743 2024-04-02 10:33:33.515656 ring_doorbell-0.8.9/tests/fixtures/ring_group_devices.json
+-rw-r--r--   0        0        0      786 2024-04-02 10:33:33.515656 ring_doorbell-0.8.9/tests/fixtures/ring_groups.json
+-rw-r--r--   0        0        0     2663 2024-04-02 10:33:33.515656 ring_doorbell-0.8.9/tests/fixtures/ring_intercom_history.json
+-rw-r--r--   0        0        0    10602 2024-04-02 10:33:33.515656 ring_doorbell-0.8.9/tests/fixtures/ring_intercom_settings.json
+-rw-r--r--   0        0        0      661 2024-04-02 10:33:33.515656 ring_doorbell-0.8.9/tests/fixtures/ring_intercom_users.json
+-rw-r--r--   0        0        0      347 2024-04-02 10:33:33.515656 ring_doorbell-0.8.9/tests/fixtures/ring_listen_credentials.json
+-rw-r--r--   0        0        0      834 2024-04-02 10:33:33.515656 ring_doorbell-0.8.9/tests/fixtures/ring_listen_ding.json
+-rw-r--r--   0        0        0      181 2024-04-02 10:33:33.515656 ring_doorbell-0.8.9/tests/fixtures/ring_listen_fcmdata.json
+-rw-r--r--   0        0        0      302 2024-04-02 10:33:33.515656 ring_doorbell-0.8.9/tests/fixtures/ring_listen_intercom_unlock.json
+-rw-r--r--   0        0        0      970 2024-04-02 10:33:33.515656 ring_doorbell-0.8.9/tests/fixtures/ring_listen_motion.json
+-rw-r--r--   0        0        0      201 2024-04-02 10:33:33.515656 ring_doorbell-0.8.9/tests/fixtures/ring_oauth.json
+-rw-r--r--   0        0        0     1248 2024-04-02 10:33:33.515656 ring_doorbell-0.8.9/tests/fixtures/ring_session.json
+-rw-r--r--   0        0        0     7983 2024-04-02 10:33:33.515656 ring_doorbell-0.8.9/tests/test_cli.py
+-rw-r--r--   0        0        0     7633 2024-04-02 10:33:33.515656 ring_doorbell-0.8.9/tests/test_listen.py
+-rw-r--r--   0        0        0     3769 2024-04-02 10:33:33.515656 ring_doorbell-0.8.9/tests/test_other.py
+-rw-r--r--   0        0        0     5399 2024-04-02 10:33:33.515656 ring_doorbell-0.8.9/tests/test_ring.py
+-rw-r--r--   0        0        0    10601 1970-01-01 00:00:00.000000 ring_doorbell-0.8.9/PKG-INFO
```

### Comparing `ring_doorbell-0.8.8/CONTRIBUTING.rst` & `ring_doorbell-0.8.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ring_doorbell-0.8.8/LICENSE` & `ring_doorbell-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ring_doorbell-0.8.8/README.rst` & `ring_doorbell-0.8.9/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -105,48 +105,57 @@
 #.  Run ``ring-doorbell --help`` or ``ring-doorbell videos --help`` for full options
 
 Initializing your Ring object
 -----------------------------
 
 .. code-block:: python
 
-    import json
     import getpass
+    import json
     from pathlib import Path
     from pprint import pprint
 
-    from ring_doorbell import Ring, Auth
-    from oauthlib.oauth2 import MissingTokenError
+    from ring_doorbell import Auth, AuthenticationError, Requires2FAError, Ring
 
-
-    cache_file = Path("test_token.cache")
+    user_agent = "YourProjectName-1.0"  # Change this
+    cache_file = Path(user_agent + ".token.cache")
 
 
     def token_updated(token):
         cache_file.write_text(json.dumps(token))
 
 
     def otp_callback():
         auth_code = input("2FA code: ")
         return auth_code
 
 
+    def do_auth():
+        username = input("Username: ")
+        password = getpass.getpass("Password: ")
+        auth = Auth(user_agent, None, token_updated)
+        try:
+            auth.fetch_token(username, password)
+        except Requires2FAError:
+            auth.fetch_token(username, password, otp_callback())
+        return auth
+
+
     def main():
-        if cache_file.is_file():
-            auth = Auth("MyProject/1.0", json.loads(cache_file.read_text()), token_updated)
-        else:
-            username = input("Username: ")
-            password = getpass.getpass("Password: ")
-            auth = Auth("MyProject/1.0", None, token_updated)
+        if cache_file.is_file():  # auth token is cached
+            auth = Auth(user_agent, json.loads(cache_file.read_text()), token_updated)
+            ring = Ring(auth)
             try:
-                auth.fetch_token(username, password)
-            except MissingTokenError:
-                auth.fetch_token(username, password, otp_callback())
+                ring.create_session()  # auth token still valid
+            except AuthenticationError:  # auth token has expired
+                auth = do_auth()
+        else:
+            auth = do_auth()  # Get new auth token
+            ring = Ring(auth)
 
-        ring = Ring(auth)
         ring.update_data()
 
         devices = ring.devices()
         pprint(devices)
 
 
     if __name__ == "__main__":
```

### Comparing `ring_doorbell-0.8.8/pyproject.toml` & `ring_doorbell-0.8.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ring-doorbell"
-version = "0.8.8"
+version = "0.8.9"
 description = "A Python library to communicate with Ring Door Bell (https://ring.com/)"
 authors = ["Marcelo Moreira de Mello <tchello.mello@gmail.com>"]
 license = "LGPLv3+"
 readme = "README.rst"
 homepage = "https://github.com/tchellomello/python-ring-doorbell"
 repository = "https://github.com/tchellomello/python-ring-doorbell"
 documentation = "http://python-ring-doorbell.readthedocs.io/"
@@ -45,29 +45,32 @@
 oauthlib = ">=3.0.0,<4"
 pytz = ">=2022.0"
 asyncclick = ">=8"
 anyio = "*" # see https://github.com/python-trio/asyncclick/issues/18
 sphinx = {version = "<7.2.6", optional = true}
 sphinx-rtd-theme = {version = "^1.3.0", optional = true}
 sphinx-github-changelog = {version = "^1.2.1", optional = true}
-firebase-messaging = {version = "^0.2.0", optional = true}
+firebase-messaging = {version = "^0.2.1", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "*"
 mock = "*"
 pre-commit = "*"
 pylint = "*"
 pytest = "*"
 pytest-cov = "*"
 requests-mock = "*"
 tox = "*"
 pytest-asyncio = "*"
 pytest-mock = "*"
 black = "*"
 pytest-socket = "^0.6.0"
+types-requests-oauthlib = "1.3"
+types-pytz = "^2024.1.0.20240203"
+types-click = "^7.1.8"
 
 [tool.poetry.extras]
 docs = ["sphinx", "sphinx-rtd-theme", "sphinx-github-changelog"]
 listen = ["firebase-messaging"]
 
 [tool.pytest.ini_options]
 testpaths = [
@@ -118,10 +121,23 @@
     "E501", # ignore line-too-longs
 ]
 "docs/source/conf.py" = [
     "D100",
     "D103",
 ]
 
+[tool.mypy]
+exclude = [
+    '/scripts/',  # TOML literal string (single-quotes, no escaping necessary)
+    'tests/.*',
+]
+disallow_untyped_defs = true
+
+[[tool.mypy.overrides]]
+module = [
+    "ring_doorbell.cli"
+]
+disallow_untyped_defs = false
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ring_doorbell-0.8.8/ring_doorbell/__init__.py` & `ring_doorbell-0.8.9/ring_doorbell/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 """Python Package for interacting with Ring devices."""
 from importlib.metadata import version
 
 __version__ = version("ring_doorbell")
 
 from ring_doorbell.auth import Auth
 from ring_doorbell.chime import RingChime
+from ring_doorbell.const import RingCapability, RingEventKind
 from ring_doorbell.doorbot import RingDoorBell
 from ring_doorbell.event import RingEvent
 from ring_doorbell.exceptions import (
     AuthenticationError,
     Requires2FAError,
     RingError,
     RingTimeout,
 )
 from ring_doorbell.generic import RingGeneric
 from ring_doorbell.group import RingLightGroup
 from ring_doorbell.other import RingOther
-from ring_doorbell.ring import Ring
+from ring_doorbell.ring import Ring, RingDevices
 from ring_doorbell.stickup_cam import RingStickUpCam
 
 __all__ = [
     "Ring",
     "Auth",
+    "RingDevices",
     "RingChime",
+    "RingCapability",
+    "RingEventKind",
     "RingStickUpCam",
     "RingLightGroup",
     "RingDoorBell",
     "RingOther",
     "RingEvent",
     "RingError",
     "AuthenticationError",
```

### Comparing `ring_doorbell-0.8.8/ring_doorbell/auth.py` & `ring_doorbell-0.8.9/ring_doorbell/auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # vim:sw=4:ts=4:et:
 """Python Ring Auth Class."""
 import uuid
 from json import dumps as json_dumps
+from typing import Any, Callable, Dict, Optional
 
 from oauthlib.oauth2 import (
     LegacyApplicationClient,
     MissingTokenError,
     OAuth2Error,
     TokenExpiredError,
 )
-from requests import HTTPError, Timeout
+from requests import HTTPError, Response, Timeout
 from requests.adapters import HTTPAdapter, Retry
 from requests_oauthlib import OAuth2Session
 
 from ring_doorbell.const import API_URI, NAMESPACE_UUID, TIMEOUT, OAuth
 from ring_doorbell.exceptions import (
     AuthenticationError,
     Requires2FAError,
@@ -21,23 +22,30 @@
     RingTimeout,
 )
 
 
 class Auth:
     """A Python Auth class for Ring"""
 
-    def __init__(self, user_agent, token=None, token_updater=None, hardware_id=None):
+    def __init__(
+        self,
+        user_agent: str,
+        token: Optional[Dict[str, Any]] = None,
+        token_updater: Optional[Callable[[Dict[str, Any]], None]] = None,
+        hardware_id: Optional[str] = None,
+    ) -> None:
         """
         :type token: Optional[Dict[str, str]]
         :type token_updater: Optional[Callable[[str], None]]
         """
         self.user_agent = user_agent
 
-        self.hardware_id = hardware_id
-        if self.hardware_id is None:
+        if hardware_id:
+            self.hardware_id = hardware_id
+        else:
             # Generate a UUID that will stay the same
             # for this physical device to prevent
             # multiple auth entries in ring.com
             self.hardware_id = str(
                 uuid.uuid5(uuid.UUID(NAMESPACE_UUID), str(uuid.getnode()) + user_agent)
             )
 
@@ -46,15 +54,17 @@
         self._oauth = OAuth2Session(
             client=LegacyApplicationClient(client_id=OAuth.CLIENT_ID), token=token
         )
         retries = Retry(connect=5, read=0, backoff_factor=2)
 
         self._oauth.mount(API_URI, HTTPAdapter(max_retries=retries))
 
-    def fetch_token(self, username, password, otp_code=None):
+    def fetch_token(
+        self, username: str, password: str, otp_code: Optional[str] = None
+    ) -> Dict[str, Any]:
         """Initial token fetch with username/password & 2FA
         :type username: str
         :type password: str
         :type otp_code: str
         """
         headers = {"User-Agent": self.user_agent, "hardware_id": self.hardware_id}
 
@@ -76,81 +86,81 @@
             raise AuthenticationError(ex) from ex
 
         if self.token_updater is not None:
             self.token_updater(token)
 
         return token
 
-    def refresh_tokens(self):
+    def refresh_tokens(self) -> Dict[str, Any]:
         """Refreshes the auth tokens"""
         try:
             token = self._oauth.refresh_token(
                 OAuth.ENDPOINT, headers={"User-Agent": self.user_agent}
             )
         except OAuth2Error as ex:
             raise AuthenticationError(ex) from ex
 
         if self.token_updater is not None:
             self.token_updater(token)
 
         return token
 
-    def get_hardware_id(self):
+    def get_hardware_id(self) -> str:
         """Get hardware ID."""
         return self.hardware_id
 
-    def get_device_model(self):
+    def get_device_model(self) -> str:
         """Get device model."""
         return self.device_model
 
     def query(
         self,
-        url,
-        method="GET",
-        extra_params=None,
-        data=None,
-        json=None,
-        timeout=None,
-        raise_for_status=True,
-    ):
+        url: str,
+        method: str = "GET",
+        extra_params: Optional[Dict[str, Any]] = None,
+        data: Optional[bytes] = None,
+        json: Optional[Dict[Any, Any]] = None,
+        timeout: Optional[float] = None,
+        raise_for_status: bool = True,
+    ) -> Response:
         """Query data from Ring API."""
         if timeout is None:
             timeout = TIMEOUT
 
         params = {}
 
         if extra_params:
             params.update(extra_params)
 
-        kwargs = {
+        kwargs: Dict[str, Any] = {
             "params": params,
             "headers": {"User-Agent": self.user_agent},
             "timeout": timeout,
         }
 
         if method in ["POST", "PUT"]:
             if json is not None:
                 kwargs["json"] = json
-                kwargs["headers"]["Content-Type"] = "application/json"
+                kwargs["headers"]["Content-Type"] = "application/json"  # type: ignore[index]
             if data is not None:
                 kwargs["data"] = data
 
         if method == "PATCH":
             # PATCH method of requests library does not have a json argument
             if json is not None:
                 kwargs["data"] = json_dumps(json)
                 kwargs["headers"]["Content-Type"] = "application/json"
             if data is not None:
                 kwargs["data"] = data
         try:
             try:
-                resp = getattr(self._oauth, method.lower())(url, **kwargs)
+                resp = self._oauth.request(method, url, **kwargs)
             except TokenExpiredError:
                 self._oauth.token = self.refresh_tokens()
-                resp = getattr(self._oauth, method.lower())(url, **kwargs)
+                resp = self._oauth.request(method, url, **kwargs)
         except AuthenticationError as ex:
             raise ex  # refresh_tokens will return this error if not valid
         except Timeout as ex:
             raise RingTimeout(f"Timeout error during query of url {url}: {ex}") from ex
         except Exception as ex:
             raise RingError(f"Unknown error during query of url {url}: {ex}") from ex
```

### Comparing `ring_doorbell-0.8.8/ring_doorbell/chime.py` & `ring_doorbell-0.8.9/ring_doorbell/chime.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,86 +1,93 @@
 # vim:sw=4:ts=4:et:
 """Python Ring Chime wrapper."""
 import logging
+from typing import Any, Dict, Union
 
 from ring_doorbell.const import (
     CHIME_KINDS,
     CHIME_PRO_KINDS,
     CHIME_TEST_SOUND_KINDS,
     CHIME_VOL_MAX,
     CHIME_VOL_MIN,
     CHIMES_ENDPOINT,
     HEALTH_CHIMES_ENDPOINT,
-    KIND_DING,
     LINKED_CHIMES_ENDPOINT,
     MSG_VOL_OUTBOUND,
     TESTSOUND_CHIME_ENDPOINT,
+    RingCapability,
+    RingEventKind,
 )
+from ring_doorbell.exceptions import RingError
 from ring_doorbell.generic import RingGeneric
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class RingChime(RingGeneric):
     """Implementation for Ring Chime."""
 
     @property
-    def family(self):
+    def family(self) -> str:
         """Return Ring device family type."""
         return "chimes"
 
-    def update_health_data(self):
+    def update_health_data(self) -> None:
         """Update health attrs."""
         self._health_attrs = (
             self._ring.query(HEALTH_CHIMES_ENDPOINT.format(self.device_api_id))
             .json()
             .get("device_health", {})
         )
 
     @property
-    def model(self):
+    def model(self) -> str:
         """Return Ring device model name."""
         if self.kind in CHIME_KINDS:
             return "Chime"
         if self.kind in CHIME_PRO_KINDS:
             return "Chime Pro"
-        return None
+        return "Unknown Chime"
 
-    def has_capability(self, capability):
+    def has_capability(self, capability: Union[RingCapability, str]) -> bool:
         """Return if device has specific capability."""
-        if capability == "volume":
+        capability = (
+            capability
+            if isinstance(capability, RingCapability)
+            else RingCapability.from_name(capability)
+        )
+        if capability == RingCapability.VOLUME:
             return True
         return False
 
     @property
-    def volume(self):
+    def volume(self) -> int:
         """Return if chime volume."""
-        return self._attrs.get("settings").get("volume")
+        return self._attrs["settings"].get("volume", 0)
 
     @volume.setter
-    def volume(self, value):
+    def volume(self, value: int) -> None:
         if not ((isinstance(value, int)) and (CHIME_VOL_MIN <= value <= CHIME_VOL_MAX)):
-            _LOGGER.error("%s", MSG_VOL_OUTBOUND.format(CHIME_VOL_MIN, CHIME_VOL_MAX))
-            return False
+            raise RingError(MSG_VOL_OUTBOUND.format(CHIME_VOL_MIN, CHIME_VOL_MAX))
 
         params = {
             "chime[description]": self.name,
             "chime[settings][volume]": str(value),
         }
         url = CHIMES_ENDPOINT.format(self.device_api_id)
         self._ring.query(url, extra_params=params, method="PUT")
         self._ring.update_devices()
-        return True
 
     @property
-    def linked_tree(self):
+    def linked_tree(self) -> Dict[str, Any]:
         """Return doorbell data linked to chime."""
         url = LINKED_CHIMES_ENDPOINT.format(self.device_api_id)
         return self._ring.query(url).json()
 
-    def test_sound(self, kind=KIND_DING):
+    def test_sound(self, kind: Union[RingEventKind, str] = RingEventKind.DING) -> bool:
         """Play chime to test sound."""
-        if kind not in CHIME_TEST_SOUND_KINDS:
+        kind_str = kind.value if isinstance(kind, RingEventKind) else kind
+        if kind_str not in CHIME_TEST_SOUND_KINDS:
             return False
         url = TESTSOUND_CHIME_ENDPOINT.format(self.device_api_id)
-        self._ring.query(url, method="POST", extra_params={"kind": kind})
+        self._ring.query(url, method="POST", extra_params={"kind": kind_str})
         return True
```

### Comparing `ring_doorbell-0.8.8/ring_doorbell/cli.py` & `ring_doorbell-0.8.9/ring_doorbell/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,36 +7,46 @@
 import json
 import logging
 import select
 import sys
 import traceback
 from datetime import datetime
 from pathlib import Path, PurePath
+from typing import Optional, Sequence, cast
 
 import asyncclick as click
 
-from ring_doorbell import Auth, AuthenticationError, Requires2FAError, Ring, RingEvent
-from ring_doorbell.const import CLI_TOKEN_FILE, PACKAGE_NAME, USER_AGENT
+from ring_doorbell import (
+    Auth,
+    AuthenticationError,
+    Requires2FAError,
+    Ring,
+    RingDoorBell,
+    RingEvent,
+    RingGeneric,
+)
+from ring_doorbell.const import CLI_TOKEN_FILE, GCM_TOKEN_FILE, PACKAGE_NAME, USER_AGENT
 from ring_doorbell.listen import can_listen
 
 
 def _header():
     _bar()
     echo("Ring CLI")
 
 
 def _bar():
     echo("---------------------------------")
 
 
-click.anyio_backend = "asyncio"
+click.anyio_backend = "asyncio"  # type: ignore[attr-defined]
 
 pass_ring = click.make_pass_decorator(Ring)
 
 cache_file = Path(CLI_TOKEN_FILE)
+gcm_cache_file = Path(GCM_TOKEN_FILE)
 
 
 class ExceptionHandlerGroup(click.Group):
     """Group to capture all exceptions and echo them nicely.
 
     Idea from https://stackoverflow.com/a/44347763
     """
@@ -114,17 +124,18 @@
     except Requires2FAError:
         auth.fetch_token(username, password, input("2FA Code: "))
         return auth
 
 
 def _get_ring(username, password, do_update_data, user_agent=USER_AGENT):
     # connect to Ring account
-    global cache_file
+    global cache_file, gcm_cache_file
     if user_agent != USER_AGENT:
         cache_file = Path(user_agent + ".token.cache")
+        gcm_cache_file = Path(user_agent + ".gcm_token.cache")
     if cache_file.is_file():
         auth = Auth(
             user_agent,
             json.loads(cache_file.read_text(encoding="utf-8")),
             token_updated,
         )
         ring = Ring(auth)
@@ -196,27 +207,24 @@
 
 
 @cli.command(name="list")
 @pass_ring
 async def list_command(ring: Ring):
     """List ring devices."""
     devices = ring.devices()
-
-    doorbells = devices["doorbots"]
-    chimes = devices["chimes"]
-    stickup_cams = devices["stickup_cams"]
-    other = devices["other"]
-
-    for device in doorbells:
+    device: Optional[RingGeneric] = None
+    for device in devices.doorbots:
         echo(device)
-    for device in chimes:
+    for device in devices.authorized_doorbots:
         echo(device)
-    for device in stickup_cams:
+    for device in devices.chimes:
         echo(device)
-    for device in other:
+    for device in devices.stickup_cams:
+        echo(device)
+    for device in devices.other:
         echo(device)
 
 
 @cli.command()
 @pass_ring
 @click.pass_context
 @click.option(
@@ -253,15 +261,15 @@
             f"No device with name {device_name} found."
             + " List of found device names (kind) is:"
         )
         return await ctx.invoke(list_command)
     if not device.has_capability("motion_detection"):
         echo(f"{str(device)} is not capable of motion detection")
         return
-
+    device = cast(RingDoorBell, device)
     state = "on" if device.motion_detection else "off"
     if not turn_on and not turn_off:
         echo(f"{str(device)} has motion detection {state}")
         return
     is_on = device.motion_detection
     if (turn_on and is_on) or (turn_off and not is_on):
         echo(f"{str(device)} already has motion detection {state}")
@@ -281,15 +289,15 @@
     default=None,
     help="Name of device, if ommited shows all devices",
 )
 @pass_ring
 @click.pass_context
 async def show(ctx, ring: Ring, device_name):
     """Display ring devices."""
-    devices = None
+    devices: Optional[Sequence[RingGeneric]] = None
 
     if device_name and (device := ring.get_device_by_name(device_name)):
         devices = [device]
     elif device_name:
         echo(
             f"No device with name {device_name} found. "
             + "List of found device names (kind) is:"
@@ -387,16 +395,18 @@
         echo(
             "(Pretty format coming soon, if you want json consistently "
             + "from this command provide the --json flag)"
         )
     if not ring.groups_data:
         echo("No ring device groups setup")
     else:
-        for group in ring.groups_data:
-            echo(json.dumps(group, indent=2))
+        for light_group in ring.groups().values():
+            light_group.update()
+            echo(json.dumps(light_group._attrs, indent=2))
+            echo(json.dumps(light_group._health_attrs, indent=2))
 
 
 @cli.command()
 @click.option(
     "--url",
     required=True,
     type=str,
@@ -502,15 +512,15 @@
 @pass_ring
 @click.pass_context
 async def videos(
     ctx, ring: Ring, count, download, download_all, max_count, download_to, device_name
 ):
     """Interact with ring videos."""
     device = None
-    if device_name and not (device := ring.get_device_by_name(device_name)):
+    if device_name and not (device := ring.get_video_device_by_name(device_name)):
         echo(
             f"No device with name {device_name} found. "
             + "List of found device names (kind) is:"
         )
         return await ctx.invoke(list_command)
     if device and not device.has_capability("video"):
         echo(f"Device {device.name} is not a video device")
@@ -522,16 +532,24 @@
         else:
             echo(
                 "No video devices found. "
                 + "List of found device names (with device kind) is:"
             )
             return await ctx.invoke(list_command)
 
-    if not count and not download and not download_all:
-        echo("Last recording url is: " + device.recording_url(device.last_recording_id))
+    if not device:  # Make mypy happy
+        return
+    if (
+        not count
+        and not download
+        and not download_all
+        and device.last_recording_id
+        and (url := device.recording_url(device.last_recording_id))
+    ):
+        echo("Last recording url is: " + url)
         return
 
     events = None
     if download_all:
         download = True
         max_count = -1
 
@@ -580,17 +598,17 @@
             counter += 1
             filename = str(PurePath(download_to, _format_filename(device.name, event)))
             echo(f"\t{counter}/{len(events)} Downloading {filename}")
 
             device.recording_download(event["id"], filename=filename, override=False)
 
 
-async def ainput(string: str) -> str:
+async def ainput(string: str):
     loop = asyncio.get_event_loop()
-    await loop.run_in_executor(None, lambda s=string: sys.stdout.write(s + " "))
+    await loop.run_in_executor(None, lambda s=string: sys.stdout.write(s + " "))  # type: ignore[misc]
 
     def read_with_timeout(timeout):
         if select.select(
             [
                 sys.stdin,
             ],
             [],
@@ -627,30 +645,30 @@
         echo(msg)
 
 
 @cli.command
 @click.option(
     "--credentials-file",
     required=False,
-    default="credentials.json",
+    default=None,
     help=(
         "File to store push credentials, "
         + "if not provided credentials will be recreated from scratch"
     ),
 )
 @click.option(
     "--store-credentials/--no-store-credentials",
-    default=False,
+    default=True,
     help="Whether or not to store the push credentials, default is false",
 )
 @click.option(
     "--show-credentials",
     default=False,
     is_flag=True,
-    help="Whether or not to store the push credentials, default is false",
+    help="Whether or not to show the push credentials, default is false",
 )
 @pass_ring
 @click.pass_context
 async def listen(
     ctx,
     ring,
     store_credentials,
@@ -672,16 +690,21 @@
             with open(credentials_file, "w", encoding="utf-8") as f:
                 json.dump(credentials, f)
         else:
             echo("New push credentials created:")
             if show_credentials:
                 echo(credentials)
 
+    if not credentials_file:
+        credentials_file = gcm_cache_file
+    else:
+        credentials_file = Path(credentials_file)
+
     credentials = None
-    if store_credentials and Path(credentials_file).is_file():
+    if store_credentials and credentials_file.is_file():
         # already registered, load previous credentials
         with open(credentials_file, encoding="utf-8") as f:
             credentials = json.load(f)
 
     event_listener = RingEventListener(ring, credentials, credentials_updated_callback)
     event_listener.start()
     event_listener.add_notification_callback(_event_handler(ring).on_event)
```

### Comparing `ring_doorbell-0.8.8/ring_doorbell/const.py` & `ring_doorbell-0.8.9/ring_doorbell/const.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,55 @@
 # vim:sw=4:ts=4:et:
-"""Constants."""
+"""Constants and enums."""
+
+from enum import Enum, auto
+
+from ring_doorbell.exceptions import RingError
 
 
 class OAuth:
     """OAuth class constants"""
 
     ENDPOINT = "https://oauth.ring.com/oauth/token"
     CLIENT_ID = "ring_official_android"
     SCOPE = ["client"]
 
 
+class RingEventKind(Enum):
+    """Enum of available ring events."""
+
+    DING = "ding"
+    MOTION = "motion"
+    INTERCOM_UNLOCK = "intercom_unlock"
+
+
+class RingCapability(Enum):
+    """Enum of available ring events."""
+
+    VIDEO = auto()
+    MOTION_DETECTION = auto()
+    HISTORY = auto()
+    LIGHT = auto()
+    SIREN = auto()
+    VOLUME = auto()
+    BATTERY = auto()
+    OPEN = auto()
+    KNOCK = auto()
+    PRE_ROLL = auto()
+
+    @staticmethod
+    def from_name(name: str) -> "RingCapability":
+        """Return ring capability from string value."""
+        capability = name.replace("-", "_").upper()
+        for ring_capability in RingCapability:
+            if ring_capability.name == capability:
+                return ring_capability
+        raise RingError(f"Unknown ring capability {name}")
+
+
 PACKAGE_NAME = "ring_doorbell"
 # timeout for HTTP requests
 TIMEOUT = 10
 
 # longer default timeout for recording downloads - typical video file sizes
 # are ~12 MB and empirical testing reveals a ~20 second download time over a
 # fast connection, suggesting speed is largely governed by capacity of Ring
@@ -31,14 +67,15 @@
 NAMESPACE_UUID = "379378b0-f747-4b67-a10f-3b13327e8879"
 
 DEFAULT_LISTEN_EVENT_EXPIRES_IN = 180
 # for Ring android app.  703521446232 for ring-site
 RING_SENDER_ID = 876313859327
 
 CLI_TOKEN_FILE = "ring_token.cache"  # noqa: S105
+GCM_TOKEN_FILE = "ring_gcm_token.cache"  # noqa: S105
 CHIMES_ENDPOINT = "/clients_api/chimes/{0}"
 DEVICES_ENDPOINT = "/clients_api/ring_devices"
 DINGS_ENDPOINT = "/clients_api/dings/active"
 DOORBELLS_ENDPOINT = "/clients_api/doorbots/{0}"
 PERSIST_TOKEN_ENDPOINT = "/clients_api/device"  # noqa: S105
 SUBSCRIPTION_ENDPOINT = "/clients_api/device"
 GROUPS_ENDPOINT = "/groups/v1/locations/{0}/groups"
```

### Comparing `ring_doorbell-0.8.8/ring_doorbell/doorbot.py` & `ring_doorbell-0.8.9/ring_doorbell/doorbot.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # vim:sw=4:ts=4:et:
 """Python Ring Doorbell wrapper."""
 import logging
 import os
 import time
+from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 from ring_doorbell.const import (
     DEFAULT_VIDEO_DOWNLOAD_TIMEOUT,
     DINGS_ENDPOINT,
     DOORBELL_2_KINDS,
     DOORBELL_3_KINDS,
     DOORBELL_3_PLUS_KINDS,
@@ -31,43 +32,47 @@
     MSG_VOL_OUTBOUND,
     PEEPHOLE_CAM_KINDS,
     SETTINGS_ENDPOINT,
     SNAPSHOT_ENDPOINT,
     SNAPSHOT_TIMESTAMP_ENDPOINT,
     URL_RECORDING,
     URL_RECORDING_SHARE_PLAY,
+    RingCapability,
 )
 from ring_doorbell.exceptions import RingError
 from ring_doorbell.generic import RingGeneric
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class RingDoorBell(RingGeneric):
     """Implementation for Ring Doorbell."""
 
-    def __init__(self, ring, device_api_id, shared=False):
+    if TYPE_CHECKING:
+        from ring_doorbell.ring import Ring
+
+    def __init__(self, ring: "Ring", device_api_id: int, shared: bool = False) -> None:
         super().__init__(ring, device_api_id)
         self.shared = shared
 
     @property
-    def family(self):
+    def family(self) -> str:
         """Return Ring device family type."""
         return "authorized_doorbots" if self.shared else "doorbots"
 
-    def update_health_data(self):
+    def update_health_data(self) -> None:
         """Update health attrs."""
         self._health_attrs = (
             self._ring.query(HEALTH_DOORBELL_ENDPOINT.format(self.device_api_id))
             .json()
             .get("device_health", {})
         )
 
     @property
-    def model(self):
+    def model(self) -> str:
         """Return Ring device model name."""
         if self.kind in DOORBELL_KINDS:
             return "Doorbell"
         if self.kind in DOORBELL_2_KINDS:
             return "Doorbell 2"
         if self.kind in DOORBELL_3_KINDS:
             return "Doorbell 3"
@@ -83,37 +88,42 @@
             return "Doorbell Elite"
         if self.kind in DOORBELL_WIRED_KINDS:
             return "Doorbell Wired"
         if self.kind in DOORBELL_GEN2_KINDS:
             return "Doorbell (2nd Gen)"
         if self.kind in PEEPHOLE_CAM_KINDS:
             return "Peephole Cam"
-        return None
+        return "Unknown Doorbell"
 
-    def has_capability(self, capability):
+    def has_capability(self, capability: Union[RingCapability, str]) -> bool:
         """Return if device has specific capability."""
-        if capability == "battery":
+        capability = (
+            capability
+            if isinstance(capability, RingCapability)
+            else RingCapability.from_name(capability)
+        )
+        if capability == RingCapability.BATTERY:
             return self.kind in (
                 DOORBELL_KINDS
                 + DOORBELL_2_KINDS
                 + DOORBELL_3_KINDS
                 + DOORBELL_3_PLUS_KINDS
                 + DOORBELL_4_KINDS
                 + DOORBELL_GEN2_KINDS
                 + PEEPHOLE_CAM_KINDS
             )
-        if capability == "knock":
+        if capability == RingCapability.KNOCK:
             return self.kind in PEEPHOLE_CAM_KINDS
-        if capability == "pre-roll":
+        if capability == RingCapability.PRE_ROLL:
             return self.kind in DOORBELL_3_PLUS_KINDS
-        if capability == "volume":
+        if capability == RingCapability.VOLUME:
             return True
-        if capability == "history":
+        if capability == RingCapability.HISTORY:
             return True
-        if capability in ("motion_detection", "video"):
+        if capability in [RingCapability.MOTION_DETECTION, RingCapability.VIDEO]:
             return self.kind in (
                 DOORBELL_KINDS
                 + DOORBELL_2_KINDS
                 + DOORBELL_3_KINDS
                 + DOORBELL_3_PLUS_KINDS
                 + DOORBELL_4_KINDS
                 + DOORBELL_PRO_KINDS
@@ -121,311 +131,302 @@
                 + DOORBELL_WIRED_KINDS
                 + DOORBELL_GEN2_KINDS
                 + PEEPHOLE_CAM_KINDS
             )
         return False
 
     @property
-    def battery_life(self):
+    def battery_life(self) -> Optional[int]:
         """Return battery life."""
         if (
-            self._attrs.get("battery_life") is None
-            and self._attrs.get("battery_life_2") is None
-        ):
+            bl1 := self._attrs.get("battery_life")
+        ) is None and "battery_life_2" not in self._attrs:
             return None
 
         value = 0
-        if "battery_life_2" in self._attrs:
-            # Camera has two battery bays
-            if self._attrs.get("battery_life") is not None:
-                # Bay 1
-                value += int(self._attrs.get("battery_life"))
-            if self._attrs.get("battery_life_2") is not None:
-                # Bay 2
-                value += int(self._attrs.get("battery_life_2"))
-            return value
-
-        # Camera has a single battery bay
-        # Latest stickup cam can be externally powered
-        value = int(self._attrs.get("battery_life"))
-        if value and value > 100:
-            value = 100
+        if bl1:
+            value += int(bl1)
 
+        if bl2 := self._attrs.get("battery_life_2"):  # Camera has two battery bays
+            value += int(bl2)
+
+        if value > 100:
+            value = 100
         return value
 
+    def _get_chime_setting(self, setting: str) -> Optional[Any]:
+        if (settings := self._attrs.get("settings")) and (
+            chime_settings := settings.get("chime_settings")
+        ):
+            return chime_settings.get(setting)
+        return None
+
     @property
-    def existing_doorbell_type(self):
+    def existing_doorbell_type(self) -> Optional[str]:
         """
         Return existing doorbell type.
 
         0: Mechanical
         1: Digital
         2: Not Present
         """
         try:
-            return DOORBELL_EXISTING_TYPE[
-                self._attrs.get("settings").get("chime_settings").get("type")
-            ]
+            if (dtype := self._get_chime_setting("type")) is not None:
+                return DOORBELL_EXISTING_TYPE[dtype]
+            return None
         except AttributeError:
             return None
 
     @existing_doorbell_type.setter
-    def existing_doorbell_type(self, value):
+    def existing_doorbell_type(self, value: int) -> None:
         """
         Return existing doorbell type.
 
         0: Mechanical
         1: Digital
         2: Not Present
         """
         if value not in DOORBELL_EXISTING_TYPE:
-            _LOGGER.error("%s", MSG_EXISTING_TYPE)
-            return False
+            raise RingError(f"value must be in {MSG_EXISTING_TYPE}")
         params = {
             "doorbot[description]": self.name,
             "doorbot[settings][chime_settings][type]": value,
         }
         if self.existing_doorbell_type:
             url = DOORBELLS_ENDPOINT.format(self.device_api_id)
             self._ring.query(url, extra_params=params, method="PUT")
             self._ring.update_devices()
-            return True
-        return None
 
     @property
-    def existing_doorbell_type_enabled(self):
+    def existing_doorbell_type_enabled(self) -> Optional[bool]:
         """Return if existing doorbell type is enabled."""
         if self.existing_doorbell_type:
             if self.existing_doorbell_type == DOORBELL_EXISTING_TYPE[2]:
                 return None
-            return self._attrs.get("settings").get("chime_settings").get("enable")
+            return self._get_chime_setting("enable")
         return False
 
     @existing_doorbell_type_enabled.setter
-    def existing_doorbell_type_enabled(self, value):
+    def existing_doorbell_type_enabled(self, value: bool) -> None:
         """Enable/disable the existing doorbell if Digital/Mechanical."""
         if self.existing_doorbell_type:
             if not isinstance(value, bool):
-                _LOGGER.error("%s", MSG_BOOLEAN_REQUIRED)
-                return None
+                raise RingError(MSG_BOOLEAN_REQUIRED)
 
             if self.existing_doorbell_type == DOORBELL_EXISTING_TYPE[2]:
-                return None
+                return
 
             params = {
                 "doorbot[description]": self.name,
                 "doorbot[settings][chime_settings][enable]": value,
             }
             url = DOORBELLS_ENDPOINT.format(self.device_api_id)
             self._ring.query(url, extra_params=params, method="PUT")
             self._ring.update_devices()
-            return True
-        return False
 
     @property
-    def existing_doorbell_type_duration(self):
+    def existing_doorbell_type_duration(self) -> Optional[int]:
         """Return duration for Digital chime."""
         if (
             self.existing_doorbell_type
             and self.existing_doorbell_type == DOORBELL_EXISTING_TYPE[1]
         ):
-            return self._attrs.get("settings").get("chime_settings").get("duration")
+            return self._get_chime_setting("duration")
         return None
 
     @existing_doorbell_type_duration.setter
-    def existing_doorbell_type_duration(self, value):
+    def existing_doorbell_type_duration(self, value: int) -> None:
         """Set duration for Digital chime."""
         if self.existing_doorbell_type:
             if not (
                 (isinstance(value, int))
                 and (DOORBELL_VOL_MIN <= value <= DOORBELL_VOL_MAX)
             ):
-                _LOGGER.error(
-                    "%s", MSG_VOL_OUTBOUND.format(DOORBELL_VOL_MIN, DOORBELL_VOL_MAX)
+                raise RingError(
+                    MSG_VOL_OUTBOUND.format(DOORBELL_VOL_MIN, DOORBELL_VOL_MAX)
                 )
-                return False
 
             if self.existing_doorbell_type == DOORBELL_EXISTING_TYPE[1]:
                 params = {
                     "doorbot[description]": self.name,
                     "doorbot[settings][chime_settings][duration]": value,
                 }
                 url = DOORBELLS_ENDPOINT.format(self.device_api_id)
                 self._ring.query(url, extra_params=params, method="PUT")
                 self._ring.update_devices()
-                return True
-        return None
 
     @property
-    def last_recording_id(self):
+    def last_recording_id(self) -> Optional[int]:
         """Return the last recording ID."""
         try:
-            return self.history(limit=1)[0]["id"]
+            res = self.history(limit=1)
+            return res[0].get("id") if res else None
         except (IndexError, TypeError):
             return None
 
     @property
-    def live_streaming_json(self):
+    def live_streaming_json(self) -> Optional[Dict[str, Any]]:
         """Return JSON for live streaming."""
         url = LIVE_STREAMING_ENDPOINT.format(self.device_api_id)
         req = self._ring.query(url, method="POST")
         if req and req.status_code == 200:
             url = DINGS_ENDPOINT
             try:
                 return self._ring.query(url).json()[0]
             except (IndexError, TypeError):
                 pass
         return None
 
     def recording_download(
         self,
-        recording_id,
-        filename=None,
-        override=False,
-        timeout=DEFAULT_VIDEO_DOWNLOAD_TIMEOUT,
-    ):
+        recording_id: int,
+        filename: Optional[str] = None,
+        override: bool = False,
+        timeout: int = DEFAULT_VIDEO_DOWNLOAD_TIMEOUT,
+    ) -> Optional[bytes]:
         """Save a recording in MP4 format to a file or return raw."""
         if not self.has_subscription:
             msg = "Your Ring account does not have an active subscription."
             _LOGGER.warning(msg)
-            return False
+            return None
 
         url = URL_RECORDING.format(recording_id)
         try:
             # Video download needs a longer timeout to get the large video file
             req = self._ring.query(url, timeout=timeout)
-            if req and req.status_code == 200:
+            if req.status_code == 200:
                 if filename:
                     if os.path.isfile(filename) and not override:
-                        _LOGGER.error("%s", FILE_EXISTS.format(filename))
-                        return False
+                        raise RingError(FILE_EXISTS.format(filename))
 
                     with open(filename, "wb") as recording:
                         recording.write(req.content)
-                        return True
+                        return None
                 else:
                     return req.content
+            else:
+                raise RingError(
+                    f"Could not get recording at url {url}, "
+                    + f"status code is {req.status_code}"
+                )
         except OSError as error:
             msg = f"Error downloading recording {recording_id}: {error}"
             _LOGGER.error(msg)
             raise RingError(msg) from error
-        return False
 
-    def recording_url(self, recording_id):
+    def recording_url(self, recording_id: int) -> Optional[str]:
         """Return HTTPS recording URL."""
         if not self.has_subscription:
             msg = "Your Ring account does not have an active subscription."
             _LOGGER.warning(msg)
-            return False
+            return None
 
         url = URL_RECORDING_SHARE_PLAY.format(recording_id)
         req = self._ring.query(url)
         data = req.json()
         if req and req.status_code == 200 and data is not None:
             return data["url"]
-        return False
+        return None
 
     @property
-    def subscribed(self):
+    def subscribed(self) -> bool:
         """Return if is online."""
         result = self._attrs.get("subscribed")
         if result is None:
             return False
         return True
 
     @property
-    def subscribed_motion(self):
+    def subscribed_motion(self) -> bool:
         """Return if is subscribed_motion."""
         result = self._attrs.get("subscribed_motions")
         if result is None:
             return False
         return True
 
     @property
-    def has_subscription(self):
+    def has_subscription(self) -> bool:
         """Return boolean if the account has subscription."""
-        return self._attrs.get("features").get("show_recordings")
+        if features := self._attrs.get("features"):
+            return features.get("show_recordings", False)
+        return False
 
     @property
-    def volume(self):
+    def volume(self) -> int:
         """Return volume."""
-        return self._attrs.get("settings").get("doorbell_volume")
+        return self._attrs["settings"].get("doorbell_volume", 0)
 
     @volume.setter
-    def volume(self, value):
+    def volume(self, value: int) -> None:
         if not (
             (isinstance(value, int)) and (DOORBELL_VOL_MIN <= value <= DOORBELL_VOL_MAX)
         ):
-            _LOGGER.error(
-                "%s", MSG_VOL_OUTBOUND.format(DOORBELL_VOL_MIN, DOORBELL_VOL_MAX)
-            )
-            return False
+            raise RingError(MSG_VOL_OUTBOUND.format(DOORBELL_VOL_MIN, DOORBELL_VOL_MAX))
 
         params = {
             "doorbot[description]": self.name,
             "doorbot[settings][doorbell_volume]": str(value),
         }
         url = DOORBELLS_ENDPOINT.format(self.device_api_id)
         self._ring.query(url, extra_params=params, method="PUT")
         self._ring.update_devices()
-        return True
 
     @property
-    def connection_status(self):
+    def connection_status(self) -> Optional[str]:
         """Return connection status."""
-        return self._attrs.get("alerts").get("connection")
+        if alerts := self._attrs.get("alerts"):
+            return alerts.get("connection")
+        return None
 
-    def get_snapshot(self, retries=3, delay=1, filename=None):
+    def get_snapshot(
+        self, retries: int = 3, delay: int = 1, filename: Optional[str] = None
+    ) -> Optional[bytes]:
         """Take a snapshot and download it"""
         url = SNAPSHOT_TIMESTAMP_ENDPOINT
         payload = {"doorbot_ids": [self._attrs.get("id")]}
         self._ring.query(url, method="POST", json=payload)
         request_time = time.time()
         for _ in range(retries):
             time.sleep(delay)
             response = self._ring.query(url, method="POST", json=payload).json()
             if response["timestamps"][0]["timestamp"] / 1000 > request_time:
                 snapshot = self._ring.query(
-                    SNAPSHOT_ENDPOINT.format(self._attrs.get("id")), raw=True
+                    SNAPSHOT_ENDPOINT.format(self._attrs.get("id"))
                 ).content
                 if filename:
                     with open(filename, "wb") as jpg:
                         jpg.write(snapshot)
-                    return True
+                    return None
                 return snapshot
-        return False
+        return None
 
-    def _motion_detection_state(self):
-        if "settings" in self._attrs and "motion_detection_enabled" in self._attrs.get(
-            "settings"
-        ):
-            return self._attrs.get("settings")["motion_detection_enabled"]
+    def _motion_detection_state(self) -> Optional[bool]:
+        if settings := self._attrs.get("settings"):
+            return settings.get("motion_detection_enabled")
         return None
 
     @property
-    def motion_detection(self):
+    def motion_detection(self) -> bool:
         """Return motion detection enabled state."""
-        return self._motion_detection_state()
+        return state if (state := self._motion_detection_state()) else False
 
     @motion_detection.setter
-    def motion_detection(self, state):
+    def motion_detection(self, state: bool) -> None:
         """Set the motion detection enabled state."""
         values = [True, False]
         if state not in values:
-            _LOGGER.error("%s", MSG_ALLOWED_VALUES.format(", ".join(values)))
-            return False
+            raise RingError(MSG_ALLOWED_VALUES.format("True, False"))
 
         if self._motion_detection_state() is None:
             _LOGGER.warning(
                 "%s",
                 MSG_EXPECTED_ATTRIBUTE_NOT_FOUND.format(
                     "settings[motion_detection_enabled]"
                 ),
             )
-            return False
+            return None
 
         url = SETTINGS_ENDPOINT.format(self.device_api_id)
         payload = {"motion_settings": {"motion_detection_enabled": state}}
 
         self._ring.query(url, method="PATCH", json=payload)
         self._ring.update_devices()
-        return True
```

### Comparing `ring_doorbell-0.8.8/ring_doorbell/generic.py` & `ring_doorbell-0.8.9/ring_doorbell/generic.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,158 +1,170 @@
 # vim:sw=4:ts=4:et:
 """Python Ring RingGeneric wrapper."""
 
 
 # pylint: disable=useless-object-inheritance
 import logging
 from datetime import datetime
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 import pytz
 
-from ring_doorbell.const import URL_DOORBELL_HISTORY
+from ring_doorbell.const import URL_DOORBELL_HISTORY, RingCapability
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class RingGeneric:
     """Generic Implementation for Ring Chime/Doorbell."""
 
-    # pylint: disable=redefined-builtin
-    # pylint:disable=invalid-name
-    def __init__(self, ring, device_api_id):
+    if TYPE_CHECKING:
+        from ring_doorbell.ring import Ring
+
+    def __init__(self, ring: "Ring", device_api_id: int) -> None:
         """Initialize Ring Generic."""
         self._ring = ring
         # This is the account ID of the device.
         # Not the same as device ID.
         self.device_api_id = device_api_id
         self.capability = False
         self.alert = None
-        self._health_attrs = {}
+        self._health_attrs: Dict[str, Any] = {}
 
         # alerts notifications
         self.alert_expires_at = None
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         """Return __repr__."""
         return f"<{self.__class__.__name__}: {self.name}>"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"{self.name} ({self.kind})"
 
-    def update(self):
+    def update(self) -> None:
         """Update this device info."""
         self.update_health_data()
 
-    def update_health_data(self):
+    def update_health_data(self) -> None:
         """Update the health data."""
         raise NotImplementedError
 
     @property
-    def _attrs(self):
+    def _attrs(self) -> Dict[str, Any]:
         """Return attributes."""
         return self._ring.devices_data[self.family][self.device_api_id]
 
     @property
-    def id(self):
+    def id(self) -> int:
         """Return ID."""
         return self.device_api_id
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Return name."""
         return self._attrs["description"]
 
     @property
-    def device_id(self):
+    def device_id(self) -> str:
         """Return device ID.
 
         This is the device_id returned by the api, usually the MAC.
         Not to be confused with the id for the device
         """
         return self._attrs["device_id"]
 
     @property
-    def family(self):
+    def location_id(self) -> Optional[str]:
+        """Return location id."""
+        return self._attrs.get("location_id", None)
+
+    @property
+    def family(self) -> str:
         """Return Ring device family type."""
         raise NotImplementedError
 
     @property
-    def model(self):
+    def model(self) -> str:
         """Return Ring device model name."""
         raise NotImplementedError
 
-    def has_capability(self, capability):
+    @property
+    def battery_life(self) -> Optional[int]:
+        """Return battery life."""
+        raise NotImplementedError
+
+    def has_capability(self, capability: Union[RingCapability, str]) -> bool:
         """Return if device has specific capability."""
         return self.capability
 
     @property
-    def address(self):
+    def address(self) -> Optional[str]:
         """Return address."""
         return self._attrs.get("address")
 
     @property
-    def firmware(self):
+    def firmware(self) -> Optional[str]:
         """Return firmware."""
         return self._attrs.get("firmware_version")
 
     @property
-    def latitude(self):
+    def latitude(self) -> Optional[float]:
         """Return latitude attr."""
         return self._attrs.get("latitude")
 
     @property
-    def longitude(self):
+    def longitude(self) -> Optional[float]:
         """Return longitude attr."""
         return self._attrs.get("longitude")
 
     @property
-    def kind(self):
+    def kind(self) -> str:
         """Return kind attr."""
-        return self._attrs.get("kind")
+        return self._attrs["kind"]
 
     @property
-    def timezone(self):
+    def timezone(self) -> Optional[str]:
         """Return timezone."""
         return self._attrs.get("time_zone")
 
     @property
-    def wifi_name(self):
+    def wifi_name(self) -> Optional[str]:
         """Return wifi ESSID name.
 
         Requires health data to be updated.
         """
         return self._health_attrs.get("wifi_name")
 
     @property
-    def wifi_signal_strength(self):
+    def wifi_signal_strength(self) -> Optional[int]:
         """Return wifi RSSI.
 
         Requires health data to be updated.
         """
         return self._health_attrs.get("latest_signal_strength")
 
     @property
-    def wifi_signal_category(self):
+    def wifi_signal_category(self) -> Optional[str]:
         """Return wifi signal category.
 
         Requires health data to be updated.
         """
         return self._health_attrs.get("latest_signal_category")
 
     def history(
         self,
-        limit=30,
-        timezone=None,
-        kind=None,
-        enforce_limit=False,
-        older_than=None,
-        retry=8,
+        limit: int = 30,
+        timezone: Optional[str] = None,
+        kind: Optional[str] = None,
+        enforce_limit: bool = False,
+        older_than: Optional[int] = None,
+        retry: int = 8,
         *,
-        convert_timezone=True,
-    ):
+        convert_timezone: bool = True,
+    ) -> List[Dict[str, Any]]:
         """
         Return history with datetime objects.
 
         :param limit: specify number of objects to be returned
         :param timezone: determine which timezone to convert data objects
         :param kind: filter by kind (ding, motion, on_demand)
         :param enforce_limit: when True, this will enforce the limit and kind
@@ -167,15 +179,15 @@
 
         # set cap for max queries
         # pylint:disable=consider-using-min-builtin
         if retry > 10:
             retry = 10
 
         while True:
-            params = {"limit": str(limit)}
+            params = {"limit": limit}
             if older_than:
                 params["older_than"] = older_than
 
             url = URL_DOORBELL_HISTORY.format(self.device_api_id)
             response = self._ring.query(url, extra_params=params).json()
 
             # cherrypick only the selected kind events
```

### Comparing `ring_doorbell-0.8.8/ring_doorbell/listen/eventlistener.py` & `ring_doorbell-0.8.9/ring_doorbell/listen/eventlistener.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Module for listening to firebase cloud messages and updating dings"""
+import asyncio
 import json
 import logging
 import time
 from datetime import datetime
+from typing import Any, Callable, Dict, Optional
 
 from firebase_messaging import FcmPushClient
 
 from ring_doorbell.const import (
     API_URI,
     API_VERSION,
     DEFAULT_LISTEN_EVENT_EXPIRES_IN,
@@ -19,50 +21,54 @@
     RING_SENDER_ID,
     SUBSCRIPTION_ENDPOINT,
 )
 from ring_doorbell.exceptions import RingError
 from ring_doorbell.ring import Ring
 
 from ..event import RingEvent
-from ..generic import RingGeneric
 from .listenerconfig import RingEventListenerConfig
 
 _logger = logging.getLogger(__name__)
 
+OnNotificationCallable = Callable[[RingEvent], None]
+CredentialsUpdatedCallable = Callable[[Dict[str, Any]], None]
+
 
 class RingEventListener:
     """Class to connect to firebase cloud messaging."""
 
     def __init__(
         self,
         ring: Ring,
-        credentials=None,
-        credentials_updated_callback=None,
+        credentials: Optional[Dict[str, Any]] = None,
+        credentials_updated_callback: Optional[CredentialsUpdatedCallable] = None,
         *,
-        config: RingEventListenerConfig = RingEventListenerConfig.default_config,
-    ):
+        config: Optional[RingEventListenerConfig] = None,
+    ) -> None:
         self._ring = ring
 
-        self._callbacks = {}
+        self._callbacks: Dict[int, OnNotificationCallable] = {}
         self.subscribed = False
         self.started = False
         self._app_id = self._ring.auth.get_hardware_id()
         self._device_model = self._ring.auth.get_device_model()
 
         self._credentials = credentials
         self._credentials_updated_callback = credentials_updated_callback
 
-        self._receiver = None
-        self._config = config or RingEventListenerConfig.default_config
+        self._receiver: Optional[FcmPushClient] = None
+        self._config: RingEventListenerConfig = (
+            config or RingEventListenerConfig.default_config()
+        )
 
         self._subscription_counter = 1
-        self._intercom_unlock_counter = {}
+        self._intercom_unlock_counter: Dict[int, int] = {}
 
-    def add_subscription_to_ring(self, token) -> bool:
-        # "hardware_id": self.auth.get_hardware_id(),
+    def add_subscription_to_ring(self, token: str) -> None:
+        """Add subscription to ring."""
         if not self._ring.session:
             self._ring.create_session()
 
         session_patch_data = {
             "device": {
                 "metadata": {
                     "api_version": API_VERSION,
@@ -89,49 +95,56 @@
             self.subscribed = False
             return
 
         self.subscribed = True
         # Update devices for the intercom unlock events
         if not self._ring.devices_data:
             self._ring.update_devices()
-        if self._ring.dings_data is None:
+        if not self._ring.dings_data:
             self._ring.update_dings()
 
-    def add_notification_callback(self, callback):
+    def add_notification_callback(self, callback: OnNotificationCallable) -> int:
         sub_id = self._subscription_counter
 
         self._callbacks[sub_id] = callback
         self._subscription_counter += 1
 
         return sub_id
 
-    def remove_notification_callback(self, subscription_id):
+    def remove_notification_callback(self, subscription_id: int) -> None:
         if subscription_id == 1:
             raise RingError(
                 "Cannot remove the default callback for ring-doorbell with value 1"
             )
 
         if subscription_id not in self._callbacks:
             raise RingError(f"ID {subscription_id} is not a valid callback id")
 
         del self._callbacks[subscription_id]
 
         if len(self._callbacks) == 0 and self._receiver:
             self._receiver.stop()
             self._receiver = None
 
-    def stop(self):
+    def stop(self) -> None:
         if self._receiver:
             self.started = False
             self._receiver.stop()
             self._receiver = None
 
         self._callbacks = {}
 
-    def start(self, callback=None, *, listen_loop=None, callback_loop=None, timeout=30):
+    def start(
+        self,
+        callback: Optional[OnNotificationCallable] = None,
+        *,
+        listen_loop: Optional[asyncio.AbstractEventLoop] = None,
+        callback_loop: Optional[asyncio.AbstractEventLoop] = None,
+        timeout: int = 30,
+    ) -> bool:
         if not callback:
             callback = self._ring.add_event_to_dings_data
 
         if not self._receiver:
             self._receiver = FcmPushClient(
                 credentials=self._credentials,
                 credentials_updated_callback=self._credentials_updated_callback,
@@ -157,15 +170,15 @@
             while not self._receiver.is_started() and now - start < timeout:
                 time.sleep(0.1)
                 now = time.time()
             self.started = self._receiver.is_started()
 
         return self.subscribed and self.started
 
-    def _get_ding_event(self, gcm_data):
+    def _get_ding_event(self, gcm_data: Dict[str, Any]) -> RingEvent:
         ding = gcm_data["ding"]
         action = gcm_data["action"]
         subtype = gcm_data["subtype"]
         if action.lower() == PUSH_ACTION_MOTION.lower():
             kind = KIND_MOTION
             state = subtype
         elif action.lower == PUSH_ACTION_DING.lower():
@@ -187,17 +200,21 @@
             device_kind=ding["device_kind"],
             now=create_seconds,
             expires_in=DEFAULT_LISTEN_EVENT_EXPIRES_IN,
             state=state,
         )
         return re
 
-    def _get_intercom_unlock_event(self, gcm_data):
+    def _get_intercom_unlock_event(
+        self, gcm_data: Dict[str, Any]
+    ) -> Optional[RingEvent]:
         device_api_id = gcm_data["alarm_meta"]["device_zid"]
-        device: RingGeneric = self._ring.get_device_by_api_id(device_api_id)
+        if (device := self._ring.get_device_by_api_id(device_api_id)) is None:
+            _logger.debug("Event received for unknown device id: %s", device_api_id)
+            return None
 
         if device_api_id not in self._intercom_unlock_counter:
             self._intercom_unlock_counter[device_api_id] = 0
         self._intercom_unlock_counter[device_api_id] += 1
         re = RingEvent(
             id=self._intercom_unlock_counter[device_api_id],
             kind=KIND_INTERCOM_UNLOCK,
@@ -206,23 +223,29 @@
             device_kind=device.kind,
             now=time.time(),
             expires_in=DEFAULT_LISTEN_EVENT_EXPIRES_IN,
             state="unlock",
         )
         return re
 
-    def on_notification(self, notification, persistent_id, obj=None):
+    def on_notification(
+        self,
+        notification: Dict[str, Dict[str, str]],
+        persistent_id: str,
+        obj: Optional[Any] = None,
+    ) -> None:
         gcm_data = json.loads(notification["data"]["gcmData"])
 
+        re: Optional[RingEvent] = None
         if "ding" in gcm_data:
             re = self._get_ding_event(gcm_data)
         elif gcm_data.get("action") == PUSH_ACTION_INTERCOM_UNLOCK:
             re = self._get_intercom_unlock_event(gcm_data)
         elif "community_alert" not in gcm_data:
             _logger.debug(
                 "Unexpected alert type in gcmData.  Full message is:\n%s",
                 json.dumps(notification),
             )
             return
-
-        for callback in self._callbacks.values():
-            callback(re)
+        if re:
+            for callback in self._callbacks.values():
+                callback(re)
```

### Comparing `ring_doorbell-0.8.8/ring_doorbell/other.py` & `ring_doorbell-0.8.9/ring_doorbell/other.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # vim:sw=4:ts=4:et:
 """Python Ring Other (Intercom) wrapper."""
 import json
 import logging
 import uuid
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 from ring_doorbell.const import (
     DOORBELLS_ENDPOINT,
     HEALTH_DOORBELL_ENDPOINT,
     INTERCOM_ALLOWED_USERS,
     INTERCOM_INVITATIONS_DELETE_ENDPOINT,
     INTERCOM_INVITATIONS_ENDPOINT,
@@ -16,220 +17,216 @@
     MIC_VOL_MIN,
     MSG_VOL_OUTBOUND,
     OTHER_DOORBELL_VOL_MAX,
     OTHER_DOORBELL_VOL_MIN,
     SETTINGS_ENDPOINT,
     VOICE_VOL_MAX,
     VOICE_VOL_MIN,
+    RingCapability,
 )
+from ring_doorbell.exceptions import RingError
 from ring_doorbell.generic import RingGeneric
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class RingOther(RingGeneric):
     """Implementation for Ring Intercom."""
 
-    def __init__(self, ring, device_api_id, shared=False):
+    if TYPE_CHECKING:
+        from ring_doorbell.ring import Ring
+
+    def __init__(self, ring: "Ring", device_api_id: int, shared: bool = False) -> None:
         super().__init__(ring, device_api_id)
         self.shared = shared
 
     @property
-    def family(self):
+    def family(self) -> str:
         """Return Ring device family type."""
         return "other"
 
-    def update_health_data(self):
+    def update_health_data(self) -> None:
         """Update health attrs."""
         self._health_attrs = (
             self._ring.query(HEALTH_DOORBELL_ENDPOINT.format(self.device_api_id))
             .json()
             .get("device_health", {})
         )
 
     @property
-    def model(self):
+    def model(self) -> str:
         """Return Ring device model name."""
         if self.kind in INTERCOM_KINDS:
             return "Intercom"
-        return None
+        return "Unknown Other"
 
-    def has_capability(self, capability):
+    def has_capability(self, capability: Union[RingCapability, str]) -> bool:
         """Return if device has specific capability."""
-        if capability in ("open", "history"):
+        capability = (
+            capability
+            if isinstance(capability, RingCapability)
+            else RingCapability.from_name(capability)
+        )
+        if capability in [RingCapability.OPEN, RingCapability.HISTORY]:
             return self.kind in INTERCOM_KINDS
         return False
 
     @property
-    def battery_life(self):
+    def battery_life(self) -> Optional[int]:
         """Return battery life."""
         if self.kind in INTERCOM_KINDS:
             if self._attrs.get("battery_life") is None:
                 return None
 
             value = int(self._attrs.get("battery_life", 0))
             if value and value > 100:
                 value = 100
 
             return value
         return None
 
     @property
-    def subscribed(self):
+    def subscribed(self) -> bool:
         """Return if is online."""
         if self.kind in INTERCOM_KINDS:
             result = self._attrs.get("subscribed")
             if result is None:
                 return False
             return True
-        return None
+        return False
 
     @property
-    def has_subscription(self):
+    def has_subscription(self) -> bool:
         """Return boolean if the account has subscription."""
-        if self.kind in INTERCOM_KINDS:
-            return self._attrs.get("features").get("show_recordings")
-        return None
+        if self.kind in INTERCOM_KINDS and (features := self._attrs.get("features")):
+            return features.get("show_recordings", False)
+        return False
 
     @property
-    def unlock_duration(self):
+    def unlock_duration(self) -> Optional[str]:
         """Return time unlock switch is held closed"""
-        json.loads(
-            self._attrs.get("settings").get("intercom_settings").get("config")
-        ).get("analog", {}).get("unlock_duration")
+        return (
+            json.loads(self._attrs["settings"]["intercom_settings"]["config"])
+            .get("analog", {})
+            .get("unlock_duration")
+        )
 
     @property
-    def doorbell_volume(self):
+    def doorbell_volume(self) -> int:
         """Return doorbell volume."""
         if self.kind in INTERCOM_KINDS:
-            return self._attrs.get("settings").get("doorbell_volume")
-        return None
+            return self._attrs["settings"].get("doorbell_volume", 0)
+        return 0
 
     @doorbell_volume.setter
-    def doorbell_volume(self, value):
+    def doorbell_volume(self, value: int) -> None:
         if not (
             (isinstance(value, int))
             and (OTHER_DOORBELL_VOL_MIN <= value <= OTHER_DOORBELL_VOL_MAX)
         ):
-            _LOGGER.error(
-                "%s",
-                MSG_VOL_OUTBOUND.format(OTHER_DOORBELL_VOL_MIN, OTHER_DOORBELL_VOL_MAX),
+            raise RingError(
+                MSG_VOL_OUTBOUND.format(OTHER_DOORBELL_VOL_MIN, OTHER_DOORBELL_VOL_MAX)
             )
-            return False
 
         params = {
             "doorbot[settings][doorbell_volume]": str(value),
         }
         url = DOORBELLS_ENDPOINT.format(self.device_api_id)
         self._ring.query(url, extra_params=params, method="PUT")
         self._ring.update_devices()
-        return True
 
     @property
-    def keep_alive_auto(self):
+    def keep_alive_auto(self) -> Optional[float]:
         if self.kind in INTERCOM_KINDS:
-            return self._attrs.get("settings").get("keep_alive_auto")
+            return self._attrs["settings"].get("keep_alive_auto")
         return None
 
     @keep_alive_auto.setter
-    def keep_alive_auto(self, value):
+    def keep_alive_auto(self, value: float) -> None:
         url = SETTINGS_ENDPOINT.format(self.device_api_id)
         payload = {"keep_alive_settings": {"keep_alive_auto": value}}
 
         self._ring.query(url, method="PATCH", json=payload)
         self._ring.update_devices()
-        return True
 
     @property
-    def mic_volume(self):
+    def mic_volume(self) -> Optional[int]:
         """Return mic volume."""
         if self.kind in INTERCOM_KINDS:
-            return self._attrs.get("settings").get("mic_volume")
+            return self._attrs["settings"].get("mic_volume")
         return None
 
     @mic_volume.setter
-    def mic_volume(self, value):
+    def mic_volume(self, value: int) -> None:
         if not ((isinstance(value, int)) and (MIC_VOL_MIN <= value <= MIC_VOL_MAX)):
-            _LOGGER.error("%s", MSG_VOL_OUTBOUND.format(MIC_VOL_MIN, MIC_VOL_MAX))
-            return False
+            raise RingError(MSG_VOL_OUTBOUND.format(MIC_VOL_MIN, MIC_VOL_MAX))
 
         url = SETTINGS_ENDPOINT.format(self.device_api_id)
         payload = {"volume_settings": {"mic_volume": value}}
 
         self._ring.query(url, method="PATCH", json=payload)
         self._ring.update_devices()
-        return True
 
     @property
-    def voice_volume(self):
+    def voice_volume(self) -> Optional[int]:
         """Return voice volume."""
         if self.kind in INTERCOM_KINDS:
-            return self._attrs.get("settings").get("voice_volume")
+            return self._attrs["settings"].get("voice_volume")
         return None
 
     @voice_volume.setter
-    def voice_volume(self, value):
+    def voice_volume(self, value: int) -> None:
         if not ((isinstance(value, int)) and (VOICE_VOL_MIN <= value <= VOICE_VOL_MAX)):
-            _LOGGER.error("%s", MSG_VOL_OUTBOUND.format(VOICE_VOL_MIN, VOICE_VOL_MAX))
-            return False
+            raise RingError(MSG_VOL_OUTBOUND.format(VOICE_VOL_MIN, VOICE_VOL_MAX))
 
         url = SETTINGS_ENDPOINT.format(self.device_api_id)
         payload = {"volume_settings": {"voice_volume": value}}
 
         self._ring.query(url, method="PATCH", json=payload)
         self._ring.update_devices()
-        return True
 
     @property
-    def clip_length_max(self):
+    def clip_length_max(self) -> Optional[int]:
         # this value sets an effective refractory period on consecutive rigns
         # eg if set to default value of 60, rings occuring with 60 seconds of
         # first will not be detected
 
         url = SETTINGS_ENDPOINT.format(self.device_api_id)
 
         return (
             self._ring.query(url, method="GET")
             .json()
-            .get("video_settings")
+            .get("video_settings", {})
             .get("clip_length_max")
         )
 
     @clip_length_max.setter
-    def clip_length_max(self, value):
+    def clip_length_max(self, value: int) -> None:
         url = SETTINGS_ENDPOINT.format(self.device_api_id)
         payload = {"video_settings": {"clip_length_max": value}}
         self._ring.query(url, method="PATCH", json=payload)
         self._ring.update_devices()
-        return True
 
     @property
-    def connection_status(self):
+    def connection_status(self) -> Optional[str]:
         """Return connection status."""
         if self.kind in INTERCOM_KINDS:
-            return self._attrs.get("alerts").get("connection")
-        return None
-
-    @property
-    def location_id(self):
-        """Return location id."""
-        if self.kind in INTERCOM_KINDS:
-            return self._attrs.get("location_id", None)
+            return self._attrs.get("alerts", {}).get("connection")
         return None
 
     @property
-    def allowed_users(self):
+    def allowed_users(self) -> Optional[List[Dict[str, Any]]]:
         """Return list of users allowed or invited to access"""
         if self.kind in INTERCOM_KINDS:
             url = INTERCOM_ALLOWED_USERS.format(self.location_id)
             return self._ring.query(url, method="GET").json()
 
         return None
 
-    def open_door(self, user_id=-1):
+    def open_door(self, user_id: int = -1) -> bool:
         """Open the door"""
         if self.kind in INTERCOM_KINDS:
             url = INTERCOM_OPEN_ENDPOINT.format(self.device_api_id)
             request_id = str(uuid.uuid4())
             # request_timestamp = int(time.time() * 1000)
             payload = {
                 "command_name": "device_rpc",
@@ -249,15 +246,15 @@
             response = self._ring.query(url, method="PUT", json=payload).json()
             self._ring.update_devices()
             if response.get("result", {}).get("code", -1) == 0:
                 return True
 
         return False
 
-    def invite_access(self, email):
+    def invite_access(self, email: str) -> bool:
         """Invite user"""
         if self.kind in INTERCOM_KINDS:
             url = INTERCOM_INVITATIONS_ENDPOINT.format(self.location_id)
             payload = {
                 "invitation": {
                     "doorbot_ids": [self.device_api_id],
                     "invited_email": email,
@@ -265,15 +262,15 @@
                 }
             }
             self._ring.query(url, method="POST", json=payload)
             return True
 
         return False
 
-    def remove_access(self, user_id):
+    def remove_access(self, user_id: int) -> bool:
         """Remove user access or invitation"""
         if self.kind in INTERCOM_KINDS:
             url = INTERCOM_INVITATIONS_DELETE_ENDPOINT.format(self.location_id, user_id)
             self._ring.query(url, method="DELETE")
             return True
 
         return False
```

### Comparing `ring_doorbell-0.8.8/ring_doorbell/ring.py` & `ring_doorbell-0.8.9/ring_doorbell/ring.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,78 @@
 # vim:sw=4:ts=4:et:
 """Python Ring Doorbell module."""
 import logging
+from itertools import chain
 from time import time
-from typing import List
+from typing import Any, Dict, Iterator, List, Mapping, Optional, Sequence, Tuple
+
+from requests import Response
 
 from ring_doorbell import RingEvent
 from ring_doorbell.auth import Auth
 from ring_doorbell.chime import RingChime
 from ring_doorbell.doorbot import RingDoorBell
+from ring_doorbell.exceptions import RingError
+from ring_doorbell.generic import RingGeneric
 from ring_doorbell.group import RingLightGroup
 from ring_doorbell.other import RingOther
 from ring_doorbell.stickup_cam import RingStickUpCam
 
 from .const import (
     API_URI,
     API_VERSION,
     DEVICES_ENDPOINT,
     DINGS_ENDPOINT,
     GROUPS_ENDPOINT,
+    INTERCOM_KINDS,
     NEW_SESSION_ENDPOINT,
 )
 
 _logger = logging.getLogger(__name__)
 
 
-TYPES = {
-    "stickup_cams": RingStickUpCam,
-    "chimes": RingChime,
-    "doorbots": RingDoorBell,
-    "authorized_doorbots": lambda ring, description: RingDoorBell(
-        ring, description, shared=True
-    ),
-    "other": RingOther,
-}
-
-
-# pylint: disable=useless-object-inheritance
 class Ring:
     """A Python Abstraction object to Ring Door Bell."""
 
     def __init__(self, auth: Auth):
         """Initialize the Ring object."""
         self.auth: Auth = auth
         self.session = None
         self.subscription = None
-        self.devices_data = None
+        self.devices_data: Dict[str, Dict[int, Dict[str, Any]]] = {}
         self.chime_health_data = None
         self.doorbell_health_data = None
-        self.dings_data = None
-        self.push_dings_data = []
-        self.groups_data = None
+        self.dings_data: Dict[Any, Any] = {}
+        self.push_dings_data: List[RingEvent] = []
+        self.groups_data: Dict[str, Dict[str, Any]] = {}
         self.init_loop = None
 
-    def update_data(self):
+    def update_data(self) -> None:
         """Update all data."""
         self._update_data()
 
-    def _update_data(self):
+    def _update_data(self) -> None:
         if self.session is None:
             self.create_session()
 
         self.update_devices()
 
         self.update_dings()
 
         self.update_groups()
 
-    def add_event_to_dings_data(self, ring_event: RingEvent):
+    def add_event_to_dings_data(self, ring_event: RingEvent) -> None:
         # Purge expired push_dings
         now = time()
         self.push_dings_data = [
             re for re in self.push_dings_data if now < re.now + re.expires_in
         ]
         self.push_dings_data.append(ring_event)
 
-    def create_session(self):
+    def create_session(self) -> None:
         """Create a new Ring session."""
         session_post_data = {
             "device": {
                 "hardware_id": self.auth.get_hardware_id(),
                 "metadata": {
                     "api_version": API_VERSION,
                     "device_model": self.auth.get_device_model(),
@@ -89,65 +83,77 @@
 
         self.session = self._query(
             NEW_SESSION_ENDPOINT,
             method="POST",
             json=session_post_data,
         ).json()
 
-    def update_devices(self):
+    def update_devices(self) -> None:
         """Update device data."""
         if self.session is None:
             self.create_session()
 
-        data = self._query(DEVICES_ENDPOINT).json()
+        data: Dict[Any, Any] = self._query(DEVICES_ENDPOINT).json()
 
         # Index data by device ID.
         self.devices_data = {
             device_type: {obj["id"]: obj for obj in devices}
             for device_type, devices in data.items()
         }
 
-    def update_dings(self):
+    def update_dings(self) -> None:
         """Update dings data."""
         if self.session is None:
             self.create_session()
 
         self.dings_data = self._query(DINGS_ENDPOINT).json()
 
-    def update_groups(self):
+    def update_groups(self) -> None:
         """Update groups data."""
         if self.session is None:
             self.create_session()
         # Get all locations
         locations = set()
-        for devices in self.devices_data.values():
-            for dev in devices.values():
-                if "location_id" in dev:
-                    locations.add(dev["location_id"])
+        devices = self.devices()
+        for device_type in devices:
+            for dev in devices[device_type]:
+                if dev.location_id is not None:
+                    locations.add(dev.location_id)
 
         # Query for groups
         self.groups_data = {}
-        locations.discard(None)
         for location in locations:
             data = self._query(GROUPS_ENDPOINT.format(location)).json()
-            if data["device_groups"] is not None:
+            if data["device_groups"]:
                 for group in data["device_groups"]:
                     self.groups_data[group["device_group_id"]] = group
 
     def query(
-        self, url, method="GET", extra_params=None, data=None, json=None, timeout=None
-    ):
+        self,
+        url: str,
+        method: str = "GET",
+        extra_params: Optional[Dict[str, Any]] = None,
+        data: Optional[bytes] = None,
+        json: Optional[Dict[Any, Any]] = None,
+        timeout: Optional[float] = None,
+    ) -> Response:
         """Query data from Ring API."""
         if self.session is None:
             self.create_session()
         return self._query(url, method, extra_params, data, json, timeout)
 
     def _query(
-        self, url, method="GET", extra_params=None, data=None, json=None, timeout=None
-    ):
+        self,
+        url: str,
+        method: str = "GET",
+        extra_params: Optional[Dict[str, Any]] = None,
+        data: Optional[bytes] = None,
+        json: Optional[Dict[Any, Any]] = None,
+        timeout: Optional[float] = None,
+    ) -> Response:
         _logger.debug(
             "url: %s\nmethod: %s\njson: %s\ndata: %s\n extra_params: %s",
             url,
             method,
             json,
             data,
             extra_params,
@@ -159,89 +165,91 @@
             data=data,
             json=json,
             timeout=timeout,
         )
         _logger.debug("response_text %s", response.text)
         return response
 
-    def devices(self):
+    def devices(self) -> "RingDevices":
         """Get all devices."""
-        devices = {}
-
-        for dev_type, convertor in TYPES.items():
-            devices[dev_type] = [
-                convertor(self, obj["id"])
-                for obj in self.devices_data.get(dev_type, {}).values()
-            ]
+        return RingDevices(self, self.devices_data)
 
-        return devices
-
-    def get_device_list(self):
+    def get_device_list(self) -> Sequence[RingGeneric]:
         """Get a combined list of all devices."""
         devices = self.devices()
-        return (
-            devices["doorbots"]
-            + devices["authorized_doorbots"]
-            + devices["stickup_cams"]
-            + devices["chimes"]
-            + devices["other"]
+        return list(
+            chain(
+                devices["doorbots"],
+                devices["authorized_doorbots"],
+                devices["stickup_cams"],
+                devices["chimes"],
+                devices["other"],
+            )
         )
 
-    def get_device_by_name(self, device_name):
+    def get_device_by_name(self, device_name: str) -> Optional[RingGeneric]:
         """Return a device using it's name."""
         all_devices = self.get_device_list()
         names_to_idx = {device.name: idx for (idx, device) in enumerate(all_devices)}
         device = (
             None
             if device_name not in names_to_idx
             else all_devices[names_to_idx[device_name]]
         )
         return device
 
-    def get_device_by_api_id(self, device_api_id):
+    def get_video_device_by_name(self, device_name: str) -> Optional[RingDoorBell]:
+        """Return a device using it's name."""
+        video_devices = self.video_devices()
+        names_to_idx = {device.name: idx for (idx, device) in enumerate(video_devices)}
+        device = (
+            None
+            if device_name not in names_to_idx
+            else video_devices[names_to_idx[device_name]]
+        )
+        return device
+
+    def get_device_by_api_id(self, device_api_id: int) -> Optional[RingGeneric]:
         """Return a device using it's id."""
         all_devices = self.get_device_list()
         api_id_to_idx = {
             device.device_api_id: idx for (idx, device) in enumerate(all_devices)
         }
         device = (
             None
             if device_api_id not in api_id_to_idx
             else all_devices[api_id_to_idx[device_api_id]]
         )
         return device
 
-    def video_devices(self):
+    def video_devices(self) -> Sequence[RingDoorBell]:
         """Get all devices."""
         devices = self.devices()
-
-        return (
-            devices["doorbots"]
-            + devices["authorized_doorbots"]
-            + devices["stickup_cams"]
+        return list(
+            chain(devices.doorbots, devices.authorized_doorbots, devices.stickup_cams)
         )
 
-    def groups(self):
+    def groups(self) -> Mapping[str, RingLightGroup]:
         """Get all groups."""
         groups = {}
 
         for group_id in self.groups_data:
             groups[group_id] = RingLightGroup(self, group_id)
 
         return groups
 
-    def active_alerts(self) -> List[RingEvent]:
+    def active_alerts(self) -> Sequence[RingEvent]:
         """Get active alerts."""
         now = time()
         # Purge expired push_dings
         self.push_dings_data = [
             re for re in self.push_dings_data if now < re.now + re.expires_in
         ]
         # Get unique id dictionary
-        alerts = {}
+        alerts: Dict[Tuple[int, int, str], RingEvent] = {}
         for re in self.push_dings_data:
             key = (re.doorbot_id, re.id, re.kind)
             if key not in alerts or re.now > alerts[key].now:
                 alerts[key] = re
 
         for ding_data in self.dings_data:
             expires_at = ding_data.get("now") + ding_data.get("expires_in")
@@ -257,8 +265,82 @@
                     kind=ding_data["kind"],
                     state=ding_data["state"],
                 )
                 key = (re.doorbot_id, re.id, re.kind)
                 if key not in alerts or re.now > alerts[key].now:
                     alerts[key] = re
 
-        return alerts.values()
+        return list(alerts.values())
+
+
+class RingDevices:
+    """Class to represent collection of devices."""
+
+    def __init__(
+        self, ring: "Ring", devices_data: Dict[str, Dict[int, Dict[str, Any]]]
+    ) -> None:
+        self._stickup_cams: List[RingStickUpCam] = []
+        self._chimes: List[RingChime] = []
+        self._doorbots: List[RingDoorBell] = []
+        self._authorized_doorbots: List[RingDoorBell] = []
+        self._other: List[RingOther] = []
+
+        for device_type, devices in devices_data.items():
+            if device_type == "stickup_cams":
+                self._stickup_cams = [
+                    RingStickUpCam(ring, device_id) for device_id in devices
+                ]
+            if device_type == "chimes":
+                self._chimes = [RingChime(ring, device_id) for device_id in devices]
+            if device_type == "doorbots":
+                self._doorbots = [
+                    RingDoorBell(ring, device_id) for device_id in devices
+                ]
+            if device_type == "authorized_doorbots":
+                self._authorized_doorbots = [
+                    RingDoorBell(ring, device_id, shared=True) for device_id in devices
+                ]
+            if device_type == "other":
+                self._other = [
+                    RingOther(ring, device_id, shared=True)
+                    for device_id, device in devices.items()
+                    if (device_kind := device.get("kind"))
+                    and device_kind in INTERCOM_KINDS
+                ]
+
+    def __getitem__(self, device_type: str) -> Sequence[RingGeneric]:
+        if device_type == "stickup_cams":
+            return self._stickup_cams
+        if device_type == "chimes":
+            return self._chimes
+        if device_type == "doorbots":
+            return self._doorbots
+        if device_type == "authorized_doorbots":
+            return self._authorized_doorbots
+        if device_type == "other":
+            return self._other
+        raise RingError(f"Invalid device_type {device_type}")
+
+    def __iter__(self) -> Iterator[str]:
+        return iter(
+            ["stickup_cams", "chimes", "doorbots", "authorized_doorbots", "other"]
+        )
+
+    @property
+    def stickup_cams(self) -> Sequence[RingStickUpCam]:
+        return self._stickup_cams
+
+    @property
+    def chimes(self) -> Sequence[RingChime]:
+        return self._chimes
+
+    @property
+    def doorbots(self) -> Sequence[RingDoorBell]:
+        return self._doorbots
+
+    @property
+    def authorized_doorbots(self) -> Sequence[RingDoorBell]:
+        return self._authorized_doorbots
+
+    @property
+    def other(self) -> Sequence[RingOther]:
+        return self._other
```

### Comparing `ring_doorbell-0.8.8/ring_doorbell/stickup_cam.py` & `ring_doorbell-0.8.9/ring_doorbell/stickup_cam.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # vim:sw=4:ts=4:et:
 """Python Ring Doorbell wrapper."""
 import logging
+from typing import Union
 
 from ring_doorbell.const import (
     FLOODLIGHT_CAM_KINDS,
     FLOODLIGHT_CAM_PLUS_KINDS,
     FLOODLIGHT_CAM_PRO_KINDS,
-    HEALTH_DOORBELL_ENDPOINT,
     INDOOR_CAM_GEN2_KINDS,
     INDOOR_CAM_KINDS,
     LIGHTS_ENDPOINT,
     MSG_ALLOWED_VALUES,
     MSG_VOL_OUTBOUND,
     SIREN_DURATION_MAX,
     SIREN_DURATION_MIN,
@@ -19,38 +19,32 @@
     SPOTLIGHT_CAM_PLUS_KINDS,
     SPOTLIGHT_CAM_PRO_KINDS,
     SPOTLIGHT_CAM_WIRED_KINDS,
     STICKUP_CAM_BATTERY_KINDS,
     STICKUP_CAM_ELITE_KINDS,
     STICKUP_CAM_GEN3_KINDS,
     STICKUP_CAM_KINDS,
+    RingCapability,
 )
 from ring_doorbell.doorbot import RingDoorBell
+from ring_doorbell.exceptions import RingError
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class RingStickUpCam(RingDoorBell):
     """Implementation for RingStickUpCam."""
 
     @property
-    def family(self):
+    def family(self) -> str:
         """Return Ring device family type."""
         return "stickup_cams"
 
-    def update_health_data(self):
-        """Update health attrs."""
-        self._health_attrs = (
-            self._ring.query(HEALTH_DOORBELL_ENDPOINT.format(self.device_api_id))
-            .json()
-            .get("device_health", {})
-        )
-
     @property
-    def model(self):
+    def model(self) -> str:
         """Return Ring device model name."""
         if self.kind in FLOODLIGHT_CAM_KINDS:
             return "Floodlight Cam"
         if self.kind in FLOODLIGHT_CAM_PRO_KINDS:
             return "Floodlight Cam Pro"
         if self.kind in FLOODLIGHT_CAM_PLUS_KINDS:
             return "Floodlight Cam Plus"
@@ -75,53 +69,58 @@
         if self.kind in STICKUP_CAM_BATTERY_KINDS:
             return "Stick Up Cam Battery"
         if self.kind in STICKUP_CAM_ELITE_KINDS:
             return "Stick Up Cam Wired"
         if self.kind in STICKUP_CAM_GEN3_KINDS:
             return "Stick Up Cam (3rd Gen)"
         _LOGGER.error("Unknown kind: %s", self.kind)
-        return None
+        return "Unknown Stickup Cam"
 
-    def has_capability(self, capability):
+    def has_capability(self, capability: Union[RingCapability, str]) -> bool:
         """Return if device has specific capability."""
-        if capability == "history":
+        capability = (
+            capability
+            if isinstance(capability, RingCapability)
+            else RingCapability.from_name(capability)
+        )
+        if capability == RingCapability.HISTORY:
             return True
-        if capability == "battery":
+        if capability == RingCapability.BATTERY:
             return self.kind in (
                 SPOTLIGHT_CAM_BATTERY_KINDS
                 + STICKUP_CAM_KINDS
                 + STICKUP_CAM_BATTERY_KINDS
                 + STICKUP_CAM_GEN3_KINDS
             )
-        if capability == "light":
+        if capability == RingCapability.LIGHT:
             return self.kind in (
                 FLOODLIGHT_CAM_KINDS
                 + FLOODLIGHT_CAM_PRO_KINDS
                 + FLOODLIGHT_CAM_PLUS_KINDS
                 + SPOTLIGHT_CAM_BATTERY_KINDS
                 + SPOTLIGHT_CAM_WIRED_KINDS
                 + SPOTLIGHT_CAM_PLUS_KINDS
                 + SPOTLIGHT_CAM_PRO_KINDS
             )
-        if capability == "siren":
+        if capability == RingCapability.SIREN:
             return self.kind in (
                 FLOODLIGHT_CAM_KINDS
                 + FLOODLIGHT_CAM_PRO_KINDS
                 + FLOODLIGHT_CAM_PLUS_KINDS
                 + INDOOR_CAM_KINDS
                 + INDOOR_CAM_GEN2_KINDS
                 + SPOTLIGHT_CAM_BATTERY_KINDS
                 + SPOTLIGHT_CAM_WIRED_KINDS
                 + SPOTLIGHT_CAM_PLUS_KINDS
                 + SPOTLIGHT_CAM_PRO_KINDS
                 + STICKUP_CAM_BATTERY_KINDS
                 + STICKUP_CAM_ELITE_KINDS
                 + STICKUP_CAM_GEN3_KINDS
             )
-        if capability in ("motion_detection", "video"):
+        if capability in [RingCapability.MOTION_DETECTION, RingCapability.VIDEO]:
             return self.kind in (
                 FLOODLIGHT_CAM_KINDS
                 + FLOODLIGHT_CAM_PRO_KINDS
                 + FLOODLIGHT_CAM_PLUS_KINDS
                 + INDOOR_CAM_KINDS
                 + INDOOR_CAM_GEN2_KINDS
                 + SPOTLIGHT_CAM_BATTERY_KINDS
@@ -132,53 +131,49 @@
                 + STICKUP_CAM_BATTERY_KINDS
                 + STICKUP_CAM_ELITE_KINDS
                 + STICKUP_CAM_GEN3_KINDS
             )
         return False
 
     @property
-    def lights(self):
+    def lights(self) -> str:
         """Return lights status."""
-        return self._attrs.get("led_status")
+        return self._attrs.get("led_status", "")
 
     @lights.setter
-    def lights(self, state):
+    def lights(self, state: str) -> None:
         """Control the lights."""
         values = ["on", "off"]
         if state not in values:
-            _LOGGER.error("%s", MSG_ALLOWED_VALUES.format(", ".join(values)))
-            return False
+            raise RingError(MSG_ALLOWED_VALUES.format(", ".join(values)))
 
         url = LIGHTS_ENDPOINT.format(self.device_api_id, state)
         self._ring.query(url, method="PUT")
         self._ring.update_devices()
-        return True
 
     @property
-    def siren(self):
+    def siren(self) -> int:
         """Return siren status."""
-        if self._attrs.get("siren_status"):
-            return self._attrs.get("siren_status").get("seconds_remaining")
-        return None
+        if siren_status := self._attrs.get("siren_status"):
+            return siren_status.get("seconds_remaining", 0)
+        return 0
 
     @siren.setter
-    def siren(self, duration):
+    def siren(self, duration: int) -> None:
         """Control the siren."""
         if not (
             (isinstance(duration, int))
             and (SIREN_DURATION_MIN <= duration <= SIREN_DURATION_MAX)
         ):
-            _LOGGER.error(
-                "%s", MSG_VOL_OUTBOUND.format(SIREN_DURATION_MIN, SIREN_DURATION_MAX)
+            raise RingError(
+                MSG_VOL_OUTBOUND.format(SIREN_DURATION_MIN, SIREN_DURATION_MAX)
             )
-            return False
 
         if duration > 0:
             state = "on"
             params = {"duration": duration}
         else:
             state = "off"
             params = {}
         url = SIREN_ENDPOINT.format(self.device_api_id, state)
         self._ring.query(url, extra_params=params, method="PUT")
         self._ring.update_devices()
-        return True
```

### Comparing `ring_doorbell-0.8.8/tests/conftest.py` & `ring_doorbell-0.8.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ring_doorbell-0.8.8/tests/fixtures/ring_chime_health_attrs.json` & `ring_doorbell-0.8.9/tests/fixtures/ring_chime_health_attrs.json`

 * *Files identical despite different names*

### Comparing `ring_doorbell-0.8.8/tests/fixtures/ring_devices.json` & `ring_doorbell-0.8.9/tests/fixtures/ring_devices.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'other'": "{insert: [(1, OrderedDict([('id', 99999999), ('kind', 'three_p_cam'), ('description', "*

 * *            "'Third party Cam'), ('location_id', '**REDACTED**'), ('schema_id', None), "*

 * *            "('is_sidewalk_gateway', True), ('deactivated_at', None), ('hardware_id', "*

 * *            "'ABCD12345'), ('time_zone', 'America/Phoenix'), ('stolen', False), ('owned', True), "*

 * *            "('settings', OrderedDict([('enable_vod', 0), ('powered_on', None), "*

 * *            "('supported_capabilities', OrderedDict() […]*

```diff
@@ -238,14 +238,61 @@
                 "theft_alarm_enable": 0,
                 "use_cached_domain": 1,
                 "use_server_ip": 0,
                 "voice_volume": 11
             },
             "subscribed": false,
             "time_zone": "Europe/Rome"
+        },
+        {
+            "alerts": {
+                "connection": "online"
+            },
+            "deactivated_at": null,
+            "description": "Third party Cam",
+            "features": {
+                "cfes_eligible": false,
+                "motion_zone_recommendation": false,
+                "motions_enabled": true,
+                "show_offline_motion_events": false,
+                "show_recordings": false,
+                "show_vod_settings": true
+            },
+            "hardware_id": "ABCD12345",
+            "id": 99999999,
+            "is_sidewalk_gateway": true,
+            "kind": "three_p_cam",
+            "location_id": "**REDACTED**",
+            "metadata": {
+                "is_sidewalk_gateway": true,
+                "third_party_dsn": "ABCD12345",
+                "third_party_manufacturer": "amazon1p",
+                "third_party_model": "A3RMGO6LYLH7YN"
+            },
+            "owned": true,
+            "owner": {
+                "email": "",
+                "first_name": "",
+                "id": "**REDACTED**",
+                "last_name": ""
+            },
+            "ring_net_id": "**REDACTED**",
+            "schema_id": null,
+            "settings": {
+                "camera_stream_configurations": [],
+                "enable_vod": 0,
+                "powered_on": null,
+                "supported_capabilities": {}
+            },
+            "stolen": false,
+            "third_party_dsn": "ABCD12345",
+            "third_party_manufacturer": "amazon1p",
+            "third_party_model": "A3RMGO6LYLH7YN",
+            "third_party_tags": [],
+            "time_zone": "America/Phoenix"
         }
     ],
     "stickup_cams": [
         {
             "address": "123 Main St",
             "alerts": {
                 "connection": "online"
```

### Comparing `ring_doorbell-0.8.8/tests/fixtures/ring_devices_updated.json` & `ring_doorbell-0.8.9/tests/fixtures/ring_devices_updated.json`

 * *Files identical despite different names*

### Comparing `ring_doorbell-0.8.8/tests/fixtures/ring_ding_active.json` & `ring_doorbell-0.8.9/tests/fixtures/ring_ding_active.json`

 * *Files identical despite different names*

### Comparing `ring_doorbell-0.8.8/tests/fixtures/ring_doorboot_health_attrs.json` & `ring_doorbell-0.8.9/tests/fixtures/ring_doorboot_health_attrs.json`

 * *Files identical despite different names*

### Comparing `ring_doorbell-0.8.8/tests/fixtures/ring_doorboot_health_attrs_id987653.json` & `ring_doorbell-0.8.9/tests/fixtures/ring_doorboot_health_attrs_id987653.json`

 * *Files identical despite different names*

### Comparing `ring_doorbell-0.8.8/tests/fixtures/ring_doorbot_history.json` & `ring_doorbell-0.8.9/tests/fixtures/ring_doorbot_history.json`

 * *Files identical despite different names*

### Comparing `ring_doorbell-0.8.8/tests/fixtures/ring_group_devices.json` & `ring_doorbell-0.8.9/tests/fixtures/ring_group_devices.json`

 * *Files identical despite different names*

### Comparing `ring_doorbell-0.8.8/tests/fixtures/ring_groups.json` & `ring_doorbell-0.8.9/tests/fixtures/ring_groups.json`

 * *Files identical despite different names*

### Comparing `ring_doorbell-0.8.8/tests/fixtures/ring_intercom_history.json` & `ring_doorbell-0.8.9/tests/fixtures/ring_intercom_history.json`

 * *Files identical despite different names*

### Comparing `ring_doorbell-0.8.8/tests/fixtures/ring_intercom_settings.json` & `ring_doorbell-0.8.9/tests/fixtures/ring_intercom_settings.json`

 * *Files identical despite different names*

### Comparing `ring_doorbell-0.8.8/tests/fixtures/ring_intercom_users.json` & `ring_doorbell-0.8.9/tests/fixtures/ring_intercom_users.json`

 * *Files identical despite different names*

### Comparing `ring_doorbell-0.8.8/tests/fixtures/ring_listen_ding.json` & `ring_doorbell-0.8.9/tests/fixtures/ring_listen_ding.json`

 * *Files identical despite different names*

### Comparing `ring_doorbell-0.8.8/tests/fixtures/ring_listen_motion.json` & `ring_doorbell-0.8.9/tests/fixtures/ring_listen_motion.json`

 * *Files identical despite different names*

### Comparing `ring_doorbell-0.8.8/tests/fixtures/ring_session.json` & `ring_doorbell-0.8.9/tests/fixtures/ring_session.json`

 * *Files identical despite different names*

### Comparing `ring_doorbell-0.8.8/tests/test_cli.py` & `ring_doorbell-0.8.9/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     devices_command,
     list_command,
     listen,
     motion_detection,
     show,
     videos,
 )
+from ring_doorbell.const import GCM_TOKEN_FILE
 from ring_doorbell.listen import can_listen
 from tests.conftest import load_fixture
 
 
 async def test_cli_default(ring):
     runner = CliRunner()
     with runner.isolated_filesystem():
@@ -74,15 +75,15 @@
 
 
 async def test_list(ring):
     runner = CliRunner()
     with runner.isolated_filesystem():
         res = await runner.invoke(list_command, obj=ring)
 
-        expected = "Front Door (lpd_v1)\nDownstairs (chime)\nFront (hp_cam_v1)\n"
+        expected = "Front Door (lpd_v1)\nBack Door (lpd_v1)\nDownstairs (chime)\nFront (hp_cam_v1)\nIngress (intercom_handset_audio)\n"
 
         assert res.exit_code == 0
         assert expected in res.output
 
 
 async def test_videos(ring, mocker):
     runner = CliRunner()
@@ -188,18 +189,18 @@
         mocker.patch(
             "firebase_messaging.FcmPushClient.register", return_value=credentials
         )
         mocker.patch("firebase_messaging.FcmPushClient.start")
         mocker.patch("firebase_messaging.FcmPushClient.is_started", return_value=True)
 
         ring = Ring(auth)
-        assert not os.path.isfile("credentials.json")
+        assert not os.path.isfile(GCM_TOKEN_FILE)
 
         await runner.invoke(listen, ["--store-credentials"], obj=ring)
-        assert os.path.isfile("credentials.json")
+        assert os.path.isfile(GCM_TOKEN_FILE)
         assert firebase_messaging.fcmpushclient.gcm_check_in.call_count == 0
         assert firebase_messaging.FcmPushClient.register.call_count == 1
         assert firebase_messaging.FcmPushClient.start.call_count == 1
 
         ring = Ring(auth)
         await runner.invoke(listen, ["--store-credentials"], obj=ring)
         assert firebase_messaging.fcmpushclient.gcm_check_in.call_count == 1
```

### Comparing `ring_doorbell-0.8.8/tests/test_listen.py` & `ring_doorbell-0.8.9/tests/test_listen.py`

 * *Files identical despite different names*

### Comparing `ring_doorbell-0.8.8/tests/test_other.py` & `ring_doorbell-0.8.9/tests/test_other.py`

 * *Files identical despite different names*

### Comparing `ring_doorbell-0.8.8/tests/test_ring.py` & `ring_doorbell-0.8.9/tests/test_ring.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 """The tests for the Ring platform."""
+import pytest
+
+from ring_doorbell import RingError
 
 
 def test_basic_attributes(ring):
     """Test the Ring class and methods."""
     data = ring.devices()
     assert len(data["chimes"]) == 1
     assert len(data["doorbots"]) == 1
@@ -117,29 +120,31 @@
 
     assert group.name == "Landscape"
     assert group.family == "group"
     assert group.group_id == "mock-group-id"
     assert group.location_id == "mock-location-id"
     assert group.model == "Light Group"
     assert group.has_capability("light") is True
-    assert group.has_capability("something-else") is False
+    with pytest.raises(RingError):
+        group.has_capability("something-else")
 
     assert group.lights is False
 
     # Attempt turning on lights
     group.lights = True
 
     # Attempt turning off lights
     group.lights = False
 
     # Attempt turning on lights for 30 seconds
     group.lights = (True, 30)
 
     # Attempt setting lights to invalid value
-    group.lights = 30
+    with pytest.raises(RingError):
+        group.lights = 30
 
 
 def test_motion_detection_enable(ring, requests_mock):
     dev = ring.devices()["doorbots"][0]
 
     dev.motion_detection = True
     dev.motion_detection = False
```

### Comparing `ring_doorbell-0.8.8/PKG-INFO` & `ring_doorbell-0.8.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ring-doorbell
-Version: 0.8.8
+Version: 0.8.9
 Summary: A Python library to communicate with Ring Door Bell (https://ring.com/)
 Home-page: https://github.com/tchellomello/python-ring-doorbell
 License: LGPLv3+
 Keywords: ring,door bell,camera,home automation
 Author: Marcelo Moreira de Mello
 Author-email: tchello.mello@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: docs
 Provides-Extra: listen
 Requires-Dist: anyio
 Requires-Dist: asyncclick (>=8)
-Requires-Dist: firebase-messaging (>=0.2.0,<0.3.0) ; extra == "listen"
+Requires-Dist: firebase-messaging (>=0.2.1,<0.3.0) ; extra == "listen"
 Requires-Dist: oauthlib (>=3.0.0,<4)
 Requires-Dist: pytz (>=2022.0)
 Requires-Dist: requests (>=2.0.0)
 Requires-Dist: requests-oauthlib (>=1.3.0,<2)
 Requires-Dist: sphinx (<7.2.6) ; extra == "docs"
 Requires-Dist: sphinx-github-changelog (>=1.2.1,<2.0.0) ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme (>=1.3.0,<2.0.0) ; extra == "docs"
@@ -143,48 +143,57 @@
 #.  Run ``ring-doorbell --help`` or ``ring-doorbell videos --help`` for full options
 
 Initializing your Ring object
 -----------------------------
 
 .. code-block:: python
 
-    import json
     import getpass
+    import json
     from pathlib import Path
     from pprint import pprint
 
-    from ring_doorbell import Ring, Auth
-    from oauthlib.oauth2 import MissingTokenError
+    from ring_doorbell import Auth, AuthenticationError, Requires2FAError, Ring
 
-
-    cache_file = Path("test_token.cache")
+    user_agent = "YourProjectName-1.0"  # Change this
+    cache_file = Path(user_agent + ".token.cache")
 
 
     def token_updated(token):
         cache_file.write_text(json.dumps(token))
 
 
     def otp_callback():
         auth_code = input("2FA code: ")
         return auth_code
 
 
+    def do_auth():
+        username = input("Username: ")
+        password = getpass.getpass("Password: ")
+        auth = Auth(user_agent, None, token_updated)
+        try:
+            auth.fetch_token(username, password)
+        except Requires2FAError:
+            auth.fetch_token(username, password, otp_callback())
+        return auth
+
+
     def main():
-        if cache_file.is_file():
-            auth = Auth("MyProject/1.0", json.loads(cache_file.read_text()), token_updated)
-        else:
-            username = input("Username: ")
-            password = getpass.getpass("Password: ")
-            auth = Auth("MyProject/1.0", None, token_updated)
+        if cache_file.is_file():  # auth token is cached
+            auth = Auth(user_agent, json.loads(cache_file.read_text()), token_updated)
+            ring = Ring(auth)
             try:
-                auth.fetch_token(username, password)
-            except MissingTokenError:
-                auth.fetch_token(username, password, otp_callback())
+                ring.create_session()  # auth token still valid
+            except AuthenticationError:  # auth token has expired
+                auth = do_auth()
+        else:
+            auth = do_auth()  # Get new auth token
+            ring = Ring(auth)
 
-        ring = Ring(auth)
         ring.update_data()
 
         devices = ring.devices()
         pprint(devices)
 
 
     if __name__ == "__main__":
```

