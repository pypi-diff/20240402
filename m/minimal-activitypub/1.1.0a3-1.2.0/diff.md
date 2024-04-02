# Comparing `tmp/minimal_activitypub-1.1.0a3.tar.gz` & `tmp/minimal_activitypub-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minimal_activitypub-1.1.0a3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "minimal_activitypub-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `minimal_activitypub-1.1.0a3.tar` & `minimal_activitypub-1.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3501 2024-03-16 03:43:04.150088 minimal_activitypub-1.1.0a3/README.rst
--rw-r--r--   0        0        0     1752 2024-03-16 06:56:19.246745 minimal_activitypub-1.1.0a3/pyproject.toml
--rw-r--r--   0        0        0      399 2024-03-16 03:43:04.150088 minimal_activitypub-1.1.0a3/src/minimal_activitypub/__init__.py
--rw-r--r--   0        0        0    41239 2024-03-16 06:55:43.349950 minimal_activitypub-1.1.0a3/src/minimal_activitypub/client_2_server.py
--rw-r--r--   0        0        0     4597 1970-01-01 00:00:00.000000 minimal_activitypub-1.1.0a3/PKG-INFO
+-rw-r--r--   0        0        0     3501 2024-03-17 08:58:03.178899 minimal_activitypub-1.2.0/README.rst
+-rw-r--r--   0        0        0     1750 2024-04-02 08:09:30.887185 minimal_activitypub-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      610 2024-04-02 08:09:30.887185 minimal_activitypub-1.2.0/src/minimal_activitypub/__init__.py
+-rw-r--r--   0        0        0    41298 2024-04-02 08:09:30.890519 minimal_activitypub-1.2.0/src/minimal_activitypub/client_2_server.py
+-rw-r--r--   0        0        0     4595 1970-01-01 00:00:00.000000 minimal_activitypub-1.2.0/PKG-INFO
```

### Comparing `minimal_activitypub-1.1.0a3/README.rst` & `minimal_activitypub-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `minimal_activitypub-1.1.0a3/pyproject.toml` & `minimal_activitypub-1.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 dependencies = [
     "h2>=4.1.0",
     "httpx>=0.27.0",
     "python-dateutil>=2.9.0.post0",
 ]
-version = "1.1.0a3"
+version = "1.2.0"
 
 [project.urls]
 Documentation = "https://marvinsmastodontools.codeberg.page/minimal-activitypub/"
 Issues = "https://codeberg.org/MarvinsMastodonTools/minimal-activitypub/issues"
 Source = "https://codeberg.org/MarvinsMastodonTools/minimal-activitypub"
 Changelog = "https://codeberg.org/MarvinsMastodonTools/minimal-activitypub/src/branch/main/CHANGELOG.rst"
```

### Comparing `minimal_activitypub-1.1.0a3/src/minimal_activitypub/client_2_server.py` & `minimal_activitypub-1.2.0/src/minimal_activitypub/client_2_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from dateutil.parser import isoparse
 from httpx import AsyncClient
 from httpx import HTTPError
 from httpx import Response
 
 from minimal_activitypub import USER_AGENT
 from minimal_activitypub import Status
+from minimal_activitypub import Visibility
 from minimal_activitypub import __display_name__
 from minimal_activitypub import __version__
 
 logger = logging.getLogger(__display_name__)
 
 
 ActivityPubClass = TypeVar("ActivityPubClass", bound="ActivityPub")
@@ -721,15 +722,15 @@
             json.dumps(response_dict, indent=4),
         )
         return (response_dict["client_id"]), (response_dict["client_secret"])
 
     async def post_status(  # noqa: PLR0913  - No way around needing all this parameters
         self: ActivityPubClass,
         status: str,
-        visibility: str = "public",
+        visibility: Visibility = Visibility.PUBLIC,
         media_ids: Optional[List[str]] = None,
         sensitive: bool = False,
         spoiler_text: Optional[str] = None,
     ) -> Status:
         """Post a status to the fediverse.
 
         :param status: The text to be posted on the timeline.
```

### Comparing `minimal_activitypub-1.1.0a3/PKG-INFO` & `minimal_activitypub-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minimal-activitypub
-Version: 1.1.0a3
+Version: 1.2.0
 Summary: Minimal inplementation of ActivityPub Interface
 Keywords: 
 Author-email: marvin8 <marvin8@tuta.io>
 Requires-Python: >=3.9, <3.13
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

