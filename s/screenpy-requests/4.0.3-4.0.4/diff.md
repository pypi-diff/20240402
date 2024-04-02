# Comparing `tmp/screenpy_requests-4.0.3.tar.gz` & `tmp/screenpy_requests-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screenpy_requests-4.0.3.tar", last modified: Fri Feb  3 15:00:02 2023, max compression
+gzip compressed data, was "screenpy_requests-4.0.4.tar", max compression
```

## Comparing `screenpy_requests-4.0.3.tar` & `screenpy_requests-4.0.4.tar`

### file list

```diff
@@ -1,31 +1,19 @@
-drwxr-xr-x   0 perry      (501) staff       (20)        0 2023-02-03 15:00:02.830975 screenpy_requests-4.0.3/
--rw-r--r--   0 perry      (501) staff       (20)     1071 2023-01-12 06:12:34.000000 screenpy_requests-4.0.3/LICENSE
--rw-r--r--   0 perry      (501) staff       (20)     2788 2023-02-03 15:00:02.830848 screenpy_requests-4.0.3/PKG-INFO
--rw-r--r--   0 perry      (501) staff       (20)     2018 2022-03-14 04:23:07.000000 screenpy_requests-4.0.3/README.md
-drwxr-xr-x   0 perry      (501) staff       (20)        0 2023-02-03 15:00:02.828567 screenpy_requests-4.0.3/screenpy_requests/
--rw-r--r--   0 perry      (501) staff       (20)      862 2023-02-03 06:11:34.000000 screenpy_requests-4.0.3/screenpy_requests/__init__.py
--rw-r--r--   0 perry      (501) staff       (20)      650 2023-02-03 14:59:18.000000 screenpy_requests-4.0.3/screenpy_requests/__version__.py
-drwxr-xr-x   0 perry      (501) staff       (20)        0 2023-02-03 15:00:02.829482 screenpy_requests-4.0.3/screenpy_requests/abilities/
--rw-r--r--   0 perry      (501) staff       (20)      141 2022-02-23 03:06:04.000000 screenpy_requests-4.0.3/screenpy_requests/abilities/__init__.py
--rw-r--r--   0 perry      (501) staff       (20)     2150 2021-12-30 18:06:41.000000 screenpy_requests-4.0.3/screenpy_requests/abilities/make_api_requests.py
-drwxr-xr-x   0 perry      (501) staff       (20)        0 2023-02-03 15:00:02.830004 screenpy_requests-4.0.3/screenpy_requests/actions/
--rw-r--r--   0 perry      (501) staff       (20)     5527 2022-12-06 23:25:51.000000 screenpy_requests-4.0.3/screenpy_requests/actions/__init__.py
--rw-r--r--   0 perry      (501) staff       (20)     2417 2023-02-03 14:53:40.000000 screenpy_requests-4.0.3/screenpy_requests/actions/add_header.py
--rw-r--r--   0 perry      (501) staff       (20)     1951 2023-02-03 14:45:27.000000 screenpy_requests-4.0.3/screenpy_requests/actions/send_api_request.py
--rw-r--r--   0 perry      (501) staff       (20)     2730 2023-02-03 14:53:35.000000 screenpy_requests-4.0.3/screenpy_requests/actions/set_headers.py
--rw-r--r--   0 perry      (501) staff       (20)      199 2022-02-23 03:10:38.000000 screenpy_requests-4.0.3/screenpy_requests/exceptions.py
--rw-r--r--   0 perry      (501) staff       (20)       39 2022-02-22 22:22:40.000000 screenpy_requests-4.0.3/screenpy_requests/py.typed
-drwxr-xr-x   0 perry      (501) staff       (20)        0 2023-02-03 15:00:02.830666 screenpy_requests-4.0.3/screenpy_requests/questions/
--rw-r--r--   0 perry      (501) staff       (20)      978 2022-12-06 23:25:51.000000 screenpy_requests-4.0.3/screenpy_requests/questions/__init__.py
--rw-r--r--   0 perry      (501) staff       (20)     1385 2022-03-10 15:51:59.000000 screenpy_requests-4.0.3/screenpy_requests/questions/body_of_the_last_response.py
--rw-r--r--   0 perry      (501) staff       (20)      869 2022-03-10 15:51:59.000000 screenpy_requests-4.0.3/screenpy_requests/questions/cookies.py
--rw-r--r--   0 perry      (501) staff       (20)     1147 2023-02-03 06:08:59.000000 screenpy_requests-4.0.3/screenpy_requests/questions/headers_of_the_last_response.py
--rw-r--r--   0 perry      (501) staff       (20)     1115 2022-03-10 15:51:59.000000 screenpy_requests-4.0.3/screenpy_requests/questions/status_code_of_the_last_response.py
-drwxr-xr-x   0 perry      (501) staff       (20)        0 2023-02-03 15:00:02.829230 screenpy_requests-4.0.3/screenpy_requests.egg-info/
--rw-r--r--   0 perry      (501) staff       (20)     2788 2023-02-03 15:00:02.000000 screenpy_requests-4.0.3/screenpy_requests.egg-info/PKG-INFO
--rw-r--r--   0 perry      (501) staff       (20)      866 2023-02-03 15:00:02.000000 screenpy_requests-4.0.3/screenpy_requests.egg-info/SOURCES.txt
--rw-r--r--   0 perry      (501) staff       (20)        1 2023-02-03 15:00:02.000000 screenpy_requests-4.0.3/screenpy_requests.egg-info/dependency_links.txt
--rw-r--r--   0 perry      (501) staff       (20)       33 2023-02-03 15:00:02.000000 screenpy_requests-4.0.3/screenpy_requests.egg-info/requires.txt
--rw-r--r--   0 perry      (501) staff       (20)       18 2023-02-03 15:00:02.000000 screenpy_requests-4.0.3/screenpy_requests.egg-info/top_level.txt
--rw-r--r--   0 perry      (501) staff       (20)       38 2023-02-03 15:00:02.831010 screenpy_requests-4.0.3/setup.cfg
--rw-r--r--   0 perry      (501) staff       (20)     1250 2023-01-12 06:12:12.000000 screenpy_requests-4.0.3/setup.py
+-rw-r--r--   0        0        0     1071 2024-04-02 19:22:22.164183 screenpy_requests-4.0.4/LICENSE
+-rw-r--r--   0        0        0     3023 2024-04-02 19:22:22.164183 screenpy_requests-4.0.4/README.md
+-rw-r--r--   0        0        0     6175 2024-04-02 19:22:22.164183 screenpy_requests-4.0.4/pyproject.toml
+-rw-r--r--   0        0        0      884 2024-04-02 19:22:22.164183 screenpy_requests-4.0.4/screenpy_requests/__init__.py
+-rw-r--r--   0        0        0      740 2024-04-02 19:22:22.164183 screenpy_requests-4.0.4/screenpy_requests/__version__.py
+-rw-r--r--   0        0        0      139 2024-04-02 19:22:22.164183 screenpy_requests-4.0.4/screenpy_requests/abilities/__init__.py
+-rw-r--r--   0        0        0     2299 2024-04-02 19:22:22.164183 screenpy_requests-4.0.4/screenpy_requests/abilities/make_api_requests.py
+-rw-r--r--   0        0        0     5553 2024-04-02 19:22:22.164183 screenpy_requests-4.0.4/screenpy_requests/actions/__init__.py
+-rw-r--r--   0        0        0     2508 2024-04-02 19:22:22.164183 screenpy_requests-4.0.4/screenpy_requests/actions/add_header.py
+-rw-r--r--   0        0        0     2055 2024-04-02 19:22:22.164183 screenpy_requests-4.0.4/screenpy_requests/actions/send_api_request.py
+-rw-r--r--   0        0        0     2838 2024-04-02 19:22:22.164183 screenpy_requests-4.0.4/screenpy_requests/actions/set_headers.py
+-rw-r--r--   0        0        0      197 2024-04-02 19:22:22.164183 screenpy_requests-4.0.4/screenpy_requests/exceptions.py
+-rw-r--r--   0        0        0       39 2024-04-02 19:22:22.164183 screenpy_requests-4.0.4/screenpy_requests/py.typed
+-rw-r--r--   0        0        0      976 2024-04-02 19:22:22.164183 screenpy_requests-4.0.4/screenpy_requests/questions/__init__.py
+-rw-r--r--   0        0        0     2615 2024-04-02 19:22:22.164183 screenpy_requests-4.0.4/screenpy_requests/questions/body_of_the_last_response.py
+-rw-r--r--   0        0        0      960 2024-04-02 19:22:22.164183 screenpy_requests-4.0.4/screenpy_requests/questions/cookies.py
+-rw-r--r--   0        0        0     1241 2024-04-02 19:22:22.164183 screenpy_requests-4.0.4/screenpy_requests/questions/headers_of_the_last_response.py
+-rw-r--r--   0        0        0     1228 2024-04-02 19:22:22.164183 screenpy_requests-4.0.4/screenpy_requests/questions/status_code_of_the_last_response.py
+-rw-r--r--   0        0        0     5005 1970-01-01 00:00:00.000000 screenpy_requests-4.0.4/PKG-INFO
```

### Comparing `screenpy_requests-4.0.3/LICENSE` & `screenpy_requests-4.0.4/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022-2023 Perry Goy
+Copyright (c) 2022-2024 Perry Goy
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `screenpy_requests-4.0.3/PKG-INFO` & `screenpy_requests-4.0.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,19 @@
-Metadata-Version: 2.1
-Name: screenpy_requests
-Version: 4.0.3
-Summary: ScreenPy extension to enable interacting with Requests.
-Home-page: https://github.com/ScreenPyHQ/screenpy_requests
-Author: Perry Goy
-Author-email: perry.goy@gmail.com
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Quality Assurance
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Software Development :: Testing :: BDD
-Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ScreenPy Requests
 =================
 
+[![Build Status](../../actions/workflows/tests.yml/badge.svg)](../../actions/workflows/tests.yml)
+[![Build Status](../../actions/workflows/lint.yml/badge.svg)](../../actions/workflows/lint.yml)
+
+[![Supported Versions](https://img.shields.io/pypi/pyversions/screenpy_requests.svg)](https://pypi.org/project/screenpy_requests)
+[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+
 ```
 TITLE CARD:
                                "ScreenPy Requests"
 TITLE DISAPPEARS.
                                                                       FADE IN:
 INT. DOCUMENTATION - MIDDAY
 
@@ -62,22 +52,27 @@
 
 or
 
     pip install screenpy[requests]
 
 
 Documentation
-----------
+-------------
 Please check out the [Read The Docs documentation](https://screenpy-requests-docs.readthedocs.io/en/latest/) for the latest information about this module!
 
 You can also read the [ScreenPy Docs](https://screenpy-docs.readthedocs.io/en/latest/) for more information about ScreenPy in general.
 
 
 Contributing
 ------------
 You want to contribute? Great! Here are the things you should do before submitting your PR:
 
-1. Install [`pre-commit`](https://pre-commit.com/)
-1. run `pre-commit install` once.
-1. run `tox` to perform tests frequently.
+1. Fork the repo and git clone your fork.
+1. `dev` install the project package:
+    1. `pip install -e .[dev]`
+    1. Optional (poetry users):
+        1. `poetry install --extras dev`
+1. Run `pre-commit install` once.
+1. Run `tox` to perform tests frequently.
+1. Create pull-request from your branch.
 
 That's it! :)
```

### Comparing `screenpy_requests-4.0.3/screenpy_requests/__init__.py` & `screenpy_requests-4.0.4/screenpy_requests/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-# -*- coding: utf-8 -*-
-
 # █▀ █▀▀ █▀█ █▀▀ █▀▀ █▄░█ █▀█ █▄█   █▀█ █▀▀ █▀█ █░█ █▀▀ █▀ ▀█▀ █▀
 # ▄█ █▄▄ █▀▄ ██▄ ██▄ █░▀█ █▀▀ ░█░   █▀▄ ██▄ ▀▀█ █▄█ ██▄ ▄█ ░█░ ▄█
 
 """
-                                ScreenPy Requests
+                                ScreenPy Requests.
+
                                                                       FADE IN:
-INT. SITEPACKAGES DIRECTORY
+
+INT. SITEPACKAGES DIRECTORY.
 
 ScreenPy Requests is an extension for ScreenPy, enabling interaction with
 Requests.
 
-:copyright: (c) 2022–2023 by Perry Goy.
+:copyright: (c) 2022-2024 by Perry Goy.
 :license: MIT, see LICENSE for more details.
 """
 
-from .abilities import *  # noqa: import all for ease-of-use
-from .actions import *  # noqa: import all for ease-of-use
-from .questions import *  # noqa: import all for ease-of-use
+from . import abilities, actions, questions
+from .abilities import *  # noqa: F403
+from .actions import *  # noqa: F403
+from .questions import *  # noqa: F403
+
+__all__ = abilities.__all__ + actions.__all__ + questions.__all__
```

### Comparing `screenpy_requests-4.0.3/screenpy_requests/abilities/make_api_requests.py` & `screenpy_requests-4.0.4/screenpy_requests/abilities/make_api_requests.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,76 @@
-"""
-Enable the Actor to make API requests and store the responses.
-"""
+"""Enable the Actor to make API requests and store the responses."""
 
-from typing import Any, Callable, Dict, List, Optional
+from __future__ import annotations
 
-from requests import Response, Session
+from typing import TYPE_CHECKING, Any, Callable
+
+from requests import Session
 
 from ..exceptions import RequestError
 
+if TYPE_CHECKING:
+    from requests import Response
+
 
 class MakeAPIRequests:
     """Use Requests to enable sending API requests.
 
     Examples::
 
         Perry = AnActor.named("Perry").who_can(MakeAPIRequests())
 
         Perry = AnActor.named("Perry").who_can(
             MakeAPIRequests.using(session_instance)
         )
     """
 
     @staticmethod
-    def using(session: Session) -> "MakeAPIRequests":
+    def using(session: Session) -> MakeAPIRequests:
         """Provide a |Requests| session for the Ability to use."""
         return MakeAPIRequests(session=session)
 
-    def to_send(self, method: str, url: str, **kwargs: Any) -> None:
+    def to_send(self, method: str, url: str, **kwargs: Any) -> None:  # noqa: ANN401
         """Send a request.
 
         This is a pass-through to the session's ``request`` method and has the
         same parameter signature. The response is stored in this Ability.
 
         Args:
             method: the HTTP method of the request - GET, POST, etc.
             url: the URL to which to send the request.
             kwargs: additional keyword arguments to pass through to |request|.
         """
-        http_requests: Dict[str, Callable] = {
+        http_requests: dict[str, Callable] = {
             "DELETE": self.session.delete,
             "GET": self.session.get,
             "HEAD": self.session.head,
             "OPTIONS": self.session.options,
             "PATCH": self.session.patch,
             "POST": self.session.post,
             "PUT": self.session.put,
         }
         method = method.upper()
 
         if method not in http_requests:
-            raise RequestError(f'"{method}" is not a valid HTTP method.')
+            msg = f'"{method}" is not a valid HTTP method.'
+            raise RequestError(msg)
 
         self.responses.append(http_requests[method](url, **kwargs))
 
     send = to_send
 
     def forget(self) -> None:
         """Clean up the Session instance stored in this Ability."""
         self.session.close()
 
     def __repr__(self) -> str:
+        """Represents Making API Requests."""
         return "Make API Requests"
 
     __str__ = __repr__
 
-    def __init__(self, session: Optional[Session] = None) -> None:
+    def __init__(self, session: Session | None = None) -> None:
         if session is None:
             session = Session()
         self.session = session
-        self.responses: List[Response] = []
+        self.responses: list[Response] = []
```

### Comparing `screenpy_requests-4.0.3/screenpy_requests/actions/__init__.py` & `screenpy_requests-4.0.4/screenpy_requests/actions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-"""
-Actions an Actor can perform using their Ability to MakeAPIRequests.
-"""
+"""Actions an Actor can perform using their Ability to MakeAPIRequests."""
 
-from typing import Protocol, Type
+from __future__ import annotations
+
+from typing import Protocol
 
 from .add_header import AddHeader
 from .send_api_request import SendAPIRequest
 from .set_headers import SetHeaders
 
 
 class APIMethodAction(Protocol):
     """Describes the available methods for a SendMETHODRequest Action."""
 
     @staticmethod
     def to(url: str) -> SendAPIRequest:
         """Set the URL this request will be sent to."""
 
 
-def generate_send_method_class(method: str) -> Type[APIMethodAction]:
-    """
-    Generates a class for a specific HTTP method call.
-    """
+def generate_send_method_class(method: str) -> type[APIMethodAction]:
+    """Generates a class for a specific HTTP method call."""
 
     class SendMETHODRequest:
-        "Will be programmatically replaced."
+        """Will be programmatically replaced."""
 
         @staticmethod
         def to(url: str) -> SendAPIRequest:
-            "Will be programmatically replaced."
+            """Will be programmatically replaced."""
             return SendAPIRequest(method, url)
 
     SendMETHODRequest.__doc__ = f"""Send a {method} request to a URL.
 
 Abilities Required:
     :class:`~screenpy_requests.abilities.MakeAPIRequests`
```

### Comparing `screenpy_requests-4.0.3/screenpy_requests/actions/add_header.py` & `screenpy_requests-4.0.4/screenpy_requests/actions/add_header.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-"""
-Add headers to an Actor's API session.
-"""
+"""Add headers to an Actor's API session."""
 
-from typing import Iterable, Union
+from __future__ import annotations
 
-from screenpy import Actor, aside, beat
+from typing import TYPE_CHECKING, Iterable, cast
+
+from screenpy import aside, beat
 from screenpy.narration import AIRY
 
 from ..abilities import MakeAPIRequests
 
+if TYPE_CHECKING:
+    from screenpy import Actor
+
 
 class AddHeader:
     """Add one or more headers to the Actor's API session.
 
     Abilities Required:
         :class:`~screenpy_requests.abilities.MakeAPIRequests`
 
@@ -34,15 +37,15 @@
                     ("Authorization", TOKEN_AUTH_STRING),
                     ("ContentType", "application/JSON"),
                 )
             )
         )
     """
 
-    def which_should_be_kept_secret(self) -> "AddHeader":
+    def which_should_be_kept_secret(self) -> AddHeader:
         """Indicate the added headers should not be written to the log."""
         self.secret = True
         self.headers_to_log = "some"
         return self
 
     secretly = which_should_be_kept_secret
 
@@ -54,23 +57,22 @@
     def perform_as(self, the_actor: Actor) -> None:
         """Direct the Actor to add the given headers to their session."""
         if not self.secret:
             aside(f"... the headers are: {self.headers}", gravitas=AIRY)
         session = the_actor.ability_to(MakeAPIRequests).session
         session.headers.update(self.headers)
 
-    def __init__(
-        self, *header_pairs: Union[str, Iterable], **header_kwargs: str
-    ) -> None:
+    def __init__(self, *header_pairs: str | Iterable, **header_kwargs: str) -> None:
         self.headers = {}
         if len(header_pairs) == 1:
-            self.headers = dict(header_pairs[0])  # type: ignore
+            self.headers = dict(cast(Iterable, header_pairs[0]))
         elif header_pairs and len(header_pairs) % 2 == 0:
             self.headers = dict(zip(header_pairs[0::2], header_pairs[1::2]))
         elif header_pairs:
-            raise ValueError("AddHeader received an odd-number of key-value pairs.")
+            msg = "AddHeader received an odd-number of key-value pairs."
+            raise ValueError(msg)
 
         if header_kwargs:
             self.headers.update(header_kwargs)
 
         self.secret = False
         self.headers_to_log = ", ".join(self.headers)
```

### Comparing `screenpy_requests-4.0.3/screenpy_requests/actions/send_api_request.py` & `screenpy_requests-4.0.4/screenpy_requests/actions/send_api_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-"""
-Send an API request.
-"""
+"""Send an API request."""
 
-from typing import Any
+from __future__ import annotations
 
-from screenpy import Actor, aside, beat
+from typing import TYPE_CHECKING, Any
+
+from screenpy import aside, beat
 from screenpy.narration import AIRY
 
 from ..abilities import MakeAPIRequests
 
+if TYPE_CHECKING:
+    from screenpy import Actor
+
 
 class SendAPIRequest:
     """Send an API request.
 
     You can use this Action class directly if you wish, but the
     Send{METHOD}Request Actions are easier to read.
 
@@ -26,24 +29,24 @@
         the_actor.attempts_to(
             SendAPIRequest("POST", "http://www.example.com").with_(
                 data={"screenplay": "Citizen Kane"}
             )
         )
     """
 
-    def with_(self, **kwargs: Any) -> "SendAPIRequest":
+    def with_(self, **kwargs: Any) -> SendAPIRequest:  # noqa: ANN401
         """Set additional kwargs to send through to the session's request.
 
         Args:
             kwargs: keyword arguments that correspond to |request|'s API.
         """
         self.kwargs = kwargs
         return self
 
-    def which_should_be_kept_secret(self) -> "SendAPIRequest":
+    def which_should_be_kept_secret(self) -> SendAPIRequest:
         """Indicate the extra data should not be written to the log."""
         self.secret = True
         return self
 
     secretly = which_should_be_kept_secret
 
     def describe(self) -> str:
```

### Comparing `screenpy_requests-4.0.3/screenpy_requests/actions/set_headers.py` & `screenpy_requests-4.0.4/screenpy_requests/actions/set_headers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-"""
-Set the headers on the Actor's API session.
-"""
+"""Set the headers on the Actor's API session."""
 
-from typing import Iterable, Union
+from __future__ import annotations
 
-from screenpy import Actor, aside, beat
+from typing import TYPE_CHECKING, Iterable, cast
+
+from screenpy import aside, beat
 from screenpy.narration import AIRY
 
 from ..abilities import MakeAPIRequests
 
+if TYPE_CHECKING:
+    from screenpy import Actor
+
 
 class SetHeaders:
     """Set the headers of the Actor's API session to this specific set.
 
     Note this will remove all other headers on your session.
 
     Abilities Required:
@@ -38,20 +41,22 @@
                     ("Cookies", "csrf_token=1234"),
                     ("ContentType", "application/JSON"),
                 )
             )
         )
     """
 
+    headers: dict
+
     @staticmethod
-    def to(**kwargs: str) -> "SetHeaders":
+    def to(**kwargs: str) -> SetHeaders:
         """Specify the headers to set."""
         return SetHeaders(**kwargs)
 
-    def which_should_be_kept_secret(self) -> "SetHeaders":
+    def which_should_be_kept_secret(self) -> SetHeaders:
         """Indicate these headers should not be written to the log."""
         self.secret = True
         self.headers_to_log = "some"
         return self
 
     secretly = which_should_be_kept_secret
 
@@ -64,23 +69,22 @@
         """Direct the Actor to set the headers for their API session."""
         if not self.secret:
             aside(f"... the headers are:\n{self.headers}", gravitas=AIRY)
         session = the_actor.ability_to(MakeAPIRequests).session
         session.headers.clear()
         session.headers.update(self.headers)
 
-    def __init__(
-        self, *header_pairs: Union[str, Iterable], **header_kwargs: str
-    ) -> None:
+    def __init__(self, *header_pairs: str | Iterable, **header_kwargs: str) -> None:
         self.headers = {}
         if len(header_pairs) == 1:
-            self.headers = dict(header_pairs[0])  # type: ignore
+            self.headers = dict(cast(Iterable, header_pairs[0]))
         elif header_pairs and len(header_pairs) % 2 == 0:
             self.headers = dict(zip(header_pairs[0::2], header_pairs[1::2]))
         elif header_pairs:
-            raise ValueError("SetHeader received an odd-number of key-value pairs.")
+            msg = "SetHeader received an odd-number of key-value pairs."
+            raise ValueError(msg)
 
         if header_kwargs:
             self.headers.update(header_kwargs)
 
         self.secret = False
         self.headers_to_log = ", ".join(self.headers)
```

### Comparing `screenpy_requests-4.0.3/screenpy_requests/questions/__init__.py` & `screenpy_requests-4.0.4/screenpy_requests/questions/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Questions an Actor might ask about API requests they've made.
-"""
+"""Questions an Actor might ask about API requests they've made."""
 
 from .body_of_the_last_response import BodyOfTheLastResponse
 from .cookies import Cookies
 from .headers_of_the_last_response import HeadersOfTheLastResponse
 from .status_code_of_the_last_response import StatusCodeOfTheLastResponse
 
 # Natural-language-enabling syntactic sugar
```

### Comparing `screenpy_requests-4.0.3/screenpy_requests/questions/body_of_the_last_response.py` & `screenpy_requests-4.0.4/screenpy_requests/questions/status_code_of_the_last_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,40 @@
-"""
-Investigate the body of the last API response received by the Actor.
-"""
+"""Investigate the status code of the last API response received."""
 
-from json.decoder import JSONDecodeError
-from typing import Union
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
 
-from screenpy import Actor
 from screenpy.exceptions import UnableToAnswer
 from screenpy.pacing import beat
 
 from ..abilities import MakeAPIRequests
 
+if TYPE_CHECKING:
+    from screenpy import Actor
+
 
-class BodyOfTheLastResponse:
-    """Ask about the body of the last API response received by the Actor.
+class StatusCodeOfTheLastResponse:
+    """Ask about the status code of the last API response received.
 
     Abilities Required:
         :class:`~screenpy_requests.abilities.MakeAPIRequests`
 
     Examples::
 
         the_actor.should(
-            See.the(BodyOfTheLastResponse(), ContainsTheEntry(play="Hamlet"))
-        )
-
-        the_actor.should(
-            See.the(BodyOfTheLastResponse(), ReadsExactly("To be, or not to be"))
+            See.the(StatusCodeOfTheLastResponse(), IsEqualTo(200))
         )
     """
 
     def describe(self) -> str:
         """Describe the Question.."""
-        return "The body of the last response."
+        return "The HTTP status code of the last response."
 
-    @beat("{} examines the body of the last response they received.")
-    def answered_by(self, the_actor: Actor) -> Union[dict, str]:
-        """Direct the Actor to investigate the body of the last response."""
+    @beat("{} examines the status code of the last response they received.")
+    def answered_by(self, the_actor: Actor) -> float:
+        """Direct the Actor to investigate the status code of the last response."""
         responses = the_actor.ability_to(MakeAPIRequests).responses
         if len(responses) < 1:
-            raise UnableToAnswer(f"{the_actor} has not yet received any API responses.")
-        try:
-            return responses[-1].json()
-        except JSONDecodeError:
-            return responses[-1].text
+            msg = f"{the_actor} has not yet received any API responses."
+            raise UnableToAnswer(msg)
+        return responses[-1].status_code
```

### Comparing `screenpy_requests-4.0.3/screenpy_requests/questions/cookies.py` & `screenpy_requests-4.0.4/screenpy_requests/questions/cookies.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-"""
-Investigate the cookies on the Actor's web or API session.
-"""
+"""Investigate the cookies on the Actor's web or API session."""
+
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
 
-from screenpy import Actor
 from screenpy.pacing import beat
 
 from ..abilities import MakeAPIRequests
 
+if TYPE_CHECKING:
+    from screenpy import Actor
+
 
 class Cookies:
     """Ask about the cookies on the Actor's API session.
 
     Abilities Required:
         :class:`~screenpy_requests.abilities.MakeAPIRequests`
```

### Comparing `screenpy_requests-4.0.3/screenpy_requests/questions/headers_of_the_last_response.py` & `screenpy_requests-4.0.4/screenpy_requests/questions/headers_of_the_last_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-"""
-Investigate the headers of the last API response received.
-"""
+"""Investigate the headers of the last API response received."""
 
-from typing import MutableMapping
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, MutableMapping
 
-from screenpy import Actor
 from screenpy.exceptions import UnableToAnswer
 from screenpy.pacing import beat
 
 from ..abilities import MakeAPIRequests
 
+if TYPE_CHECKING:
+    from screenpy import Actor
+
 
 class HeadersOfTheLastResponse:
     """Ask about the headers of the last API response received.
 
     Abilities Required:
         :class:`~screenpy_requests.abilities.MakeAPIRequests`
 
@@ -29,9 +31,10 @@
         return "The headers of the last response."
 
     @beat("{} examines the headers of the last response they received.")
     def answered_by(self, the_actor: Actor) -> MutableMapping[str, str]:
         """Direct the Actor to investigate the headers of the last response."""
         responses = the_actor.ability_to(MakeAPIRequests).responses
         if len(responses) < 1:
-            raise UnableToAnswer(f"{the_actor} has not yet received any API responses.")
+            msg = f"{the_actor} has not yet received any API responses."
+            raise UnableToAnswer(msg)
         return responses[-1].headers
```

