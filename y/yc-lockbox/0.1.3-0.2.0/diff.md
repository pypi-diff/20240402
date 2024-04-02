# Comparing `tmp/yc-lockbox-0.1.3.tar.gz` & `tmp/yc-lockbox-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yc-lockbox-0.1.3.tar", last modified: Tue Mar 26 10:57:27 2024, max compression
+gzip compressed data, was "yc-lockbox-0.2.0.tar", last modified: Tue Apr  2 08:10:38 2024, max compression
```

## Comparing `yc-lockbox-0.1.3.tar` & `yc-lockbox-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2024-03-26 10:57:27.347864 yc-lockbox-0.1.3/
--rw-r--r--   0 akimrx     (503) staff       (20)     1074 2024-03-21 07:59:37.000000 yc-lockbox-0.1.3/LICENSE
--rw-r--r--   0 akimrx     (503) staff       (20)     6429 2024-03-26 10:57:27.347940 yc-lockbox-0.1.3/PKG-INFO
--rw-r--r--   0 akimrx     (503) staff       (20)     5428 2024-03-26 10:56:59.000000 yc-lockbox-0.1.3/README.md
--rw-r--r--   0 akimrx     (503) staff       (20)     1135 2024-03-25 18:16:29.000000 yc-lockbox-0.1.3/pyproject.toml
--rw-r--r--   0 akimrx     (503) staff       (20)      486 2024-03-26 10:57:27.348397 yc-lockbox-0.1.3/setup.cfg
--rw-r--r--   0 akimrx     (503) staff       (20)     2580 2024-03-24 10:58:52.000000 yc-lockbox-0.1.3/setup.py
-drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2024-03-26 10:57:27.346890 yc-lockbox-0.1.3/yc_lockbox/
--rw-r--r--   0 akimrx     (503) staff       (20)     1700 2024-03-26 10:40:14.000000 yc-lockbox-0.1.3/yc_lockbox/__init__.py
--rw-r--r--   0 akimrx     (503) staff       (20)     8147 2024-03-26 09:46:49.000000 yc-lockbox-0.1.3/yc_lockbox/_abc.py
--rw-r--r--   0 akimrx     (503) staff       (20)     6237 2024-03-26 10:39:21.000000 yc-lockbox-0.1.3/yc_lockbox/_adapters.py
--rw-r--r--   0 akimrx     (503) staff       (20)     2880 2024-03-24 15:09:54.000000 yc-lockbox-0.1.3/yc_lockbox/_auth.py
--rw-r--r--   0 akimrx     (503) staff       (20)      930 2024-03-24 15:26:24.000000 yc-lockbox-0.1.3/yc_lockbox/_constants.py
--rw-r--r--   0 akimrx     (503) staff       (20)      456 2024-03-25 18:20:13.000000 yc-lockbox-0.1.3/yc_lockbox/_exceptions.py
--rw-r--r--   0 akimrx     (503) staff       (20)    19477 2024-03-26 09:45:05.000000 yc-lockbox-0.1.3/yc_lockbox/_lockbox.py
--rw-r--r--   0 akimrx     (503) staff       (20)    12958 2024-03-26 09:39:33.000000 yc-lockbox-0.1.3/yc_lockbox/_models.py
--rw-r--r--   0 akimrx     (503) staff       (20)      414 2024-03-26 08:07:04.000000 yc-lockbox-0.1.3/yc_lockbox/_types.py
-drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2024-03-26 10:57:27.347702 yc-lockbox-0.1.3/yc_lockbox.egg-info/
--rw-r--r--   0 akimrx     (503) staff       (20)     6429 2024-03-26 10:57:27.000000 yc-lockbox-0.1.3/yc_lockbox.egg-info/PKG-INFO
--rw-r--r--   0 akimrx     (503) staff       (20)      423 2024-03-26 10:57:27.000000 yc-lockbox-0.1.3/yc_lockbox.egg-info/SOURCES.txt
--rw-r--r--   0 akimrx     (503) staff       (20)        1 2024-03-26 10:57:27.000000 yc-lockbox-0.1.3/yc_lockbox.egg-info/dependency_links.txt
--rw-r--r--   0 akimrx     (503) staff       (20)      117 2024-03-26 10:57:27.000000 yc-lockbox-0.1.3/yc_lockbox.egg-info/requires.txt
--rw-r--r--   0 akimrx     (503) staff       (20)       11 2024-03-26 10:57:27.000000 yc-lockbox-0.1.3/yc_lockbox.egg-info/top_level.txt
+drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2024-04-02 08:10:38.125980 yc-lockbox-0.2.0/
+-rw-r--r--   0 akimrx     (503) staff       (20)     1074 2024-03-21 07:59:37.000000 yc-lockbox-0.2.0/LICENSE
+-rw-r--r--   0 akimrx     (503) staff       (20)     7816 2024-04-02 08:10:38.126046 yc-lockbox-0.2.0/PKG-INFO
+-rw-r--r--   0 akimrx     (503) staff       (20)     6816 2024-04-02 08:08:06.000000 yc-lockbox-0.2.0/README.md
+-rw-r--r--   0 akimrx     (503) staff       (20)     1135 2024-03-25 18:16:29.000000 yc-lockbox-0.2.0/pyproject.toml
+-rw-r--r--   0 akimrx     (503) staff       (20)      486 2024-04-02 08:10:38.126388 yc-lockbox-0.2.0/setup.cfg
+-rw-r--r--   0 akimrx     (503) staff       (20)     2580 2024-03-24 10:58:52.000000 yc-lockbox-0.2.0/setup.py
+drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2024-04-02 08:10:38.125255 yc-lockbox-0.2.0/yc_lockbox/
+-rw-r--r--   0 akimrx     (503) staff       (20)     1806 2024-04-02 08:07:53.000000 yc-lockbox-0.2.0/yc_lockbox/__init__.py
+-rw-r--r--   0 akimrx     (503) staff       (20)     8147 2024-03-26 09:46:49.000000 yc-lockbox-0.2.0/yc_lockbox/_abc.py
+-rw-r--r--   0 akimrx     (503) staff       (20)     6372 2024-04-02 08:07:53.000000 yc-lockbox-0.2.0/yc_lockbox/_adapters.py
+-rw-r--r--   0 akimrx     (503) staff       (20)     2880 2024-03-24 15:09:54.000000 yc-lockbox-0.2.0/yc_lockbox/_auth.py
+-rw-r--r--   0 akimrx     (503) staff       (20)      930 2024-03-24 15:26:24.000000 yc-lockbox-0.2.0/yc_lockbox/_constants.py
+-rw-r--r--   0 akimrx     (503) staff       (20)      456 2024-03-25 18:20:13.000000 yc-lockbox-0.2.0/yc_lockbox/_exceptions.py
+-rw-r--r--   0 akimrx     (503) staff       (20)    39801 2024-04-02 08:07:53.000000 yc-lockbox-0.2.0/yc_lockbox/_lockbox.py
+-rw-r--r--   0 akimrx     (503) staff       (20)    13506 2024-04-02 08:07:53.000000 yc-lockbox-0.2.0/yc_lockbox/_models.py
+-rw-r--r--   0 akimrx     (503) staff       (20)      641 2024-04-02 08:07:53.000000 yc-lockbox-0.2.0/yc_lockbox/_types.py
+drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2024-04-02 08:10:38.125879 yc-lockbox-0.2.0/yc_lockbox.egg-info/
+-rw-r--r--   0 akimrx     (503) staff       (20)     7816 2024-04-02 08:10:38.000000 yc-lockbox-0.2.0/yc_lockbox.egg-info/PKG-INFO
+-rw-r--r--   0 akimrx     (503) staff       (20)      423 2024-04-02 08:10:38.000000 yc-lockbox-0.2.0/yc_lockbox.egg-info/SOURCES.txt
+-rw-r--r--   0 akimrx     (503) staff       (20)        1 2024-04-02 08:10:38.000000 yc-lockbox-0.2.0/yc_lockbox.egg-info/dependency_links.txt
+-rw-r--r--   0 akimrx     (503) staff       (20)      117 2024-04-02 08:10:38.000000 yc-lockbox-0.2.0/yc_lockbox.egg-info/requires.txt
+-rw-r--r--   0 akimrx     (503) staff       (20)       11 2024-04-02 08:10:38.000000 yc-lockbox-0.2.0/yc_lockbox.egg-info/top_level.txt
```

### Comparing `yc-lockbox-0.1.3/LICENSE` & `yc-lockbox-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yc-lockbox-0.1.3/PKG-INFO` & `yc-lockbox-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,18 @@
-Metadata-Version: 2.1
-Name: yc-lockbox
-Version: 0.1.3
-Summary: Yandex Lockbox client
-Home-page: https://github.com/akimrx/python-yc-lockbox
-Author: Akim Faskhutdinov
-Author-email: akimstrong@yandex.ru
-License: MIT
-Keywords: yandex,cloud,vault,secrets,lockbox
-Platform: osx
-Platform: linux
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: System Administrators
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Typing :: Typed
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: aio
-License-File: LICENSE
-
 # Yandex Lockbox Client
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/yc-lockbox.svg)](https://pypi.org/project/yc-lockbox/)
 [![PyPi Package](https://img.shields.io/pypi/v/yc-lockbox.svg)](https://pypi.org/project/yc-lockbox/)
 [![Codecov](https://codecov.io/gh/akimrx/python-yc-lockbox/branch/master/graph/badge.svg)](https://app.codecov.io/gh/akimrx/python-yc-lockbox)
 [![Tests](https://github.com/akimrx/python-yc-lockbox/workflows/Tests/badge.svg)](https://github.com/akimrx/python-yc-lockbox)
 
 This library is a simple client for working with **[Yandex Lockbox](https://cloud.yandex.ru/en/docs/lockbox/)** over [REST API](https://cloud.yandex.ru/en/docs/lockbox/api-ref/), simplifying work with secrets and allowing you to work with them in the OOP paradigm.
 
+Supports two modes: synchronous and asynchronous.
+
 **[Full library documentation link](https://akimrx.github.io/python-yc-lockbox/)**
 
 **Supported Python versions**:
 
 * 3.10
 * 3.11
 * 3.12
@@ -47,46 +21,57 @@
 
 * [Pydantic V2](https://github.com/pydantic/pydantic)
 * [Crypthography](https://github.com/pyca/cryptography)
 * [PyJWT](https://github.com/jpadilla/pyjwt)
 * [Requests](https://github.com/psf/requests)
 
 
+**Extra dependencies:**
+
+* [aiohttp](https://github.com/aio-libs/aiohttp)
+
+
 **Currently, the following operations are not supported by the library:**
 
 * List secret access bindings
 * Set secret access bindings
 * Update secret access bindings
 * List secret operations
 
 
 **In the near future release:**
 
-- [ ] Async client implementation
+- [x] Tests
+- [x] Async client implementation
 - [ ] Implement access bindings methods and view operations
-- [ ] Tests
 - [ ] Ansible action and lookup plugins
 
 
 ## Install
 
-Installing with PIP:
+Installing via [pip](https://pypi.org/project/yc-lockbox/):
 
 ```
 pip install yc-lockbox
 ```
 
 Also, you can install from source with:
 
 ```
 git clone https://github.com/akimrx/python-yc-lockbox
 cd python-yc-lockbox 
 make install
 ```
 
+For async mode support use
+
+```
+pip install yc-lockbox[aio]
+```
+
 
 ## Usage
 
 
 * **Authenticate via your [OAuth token](https://oauth.yandex.com/authorize?response_type=token&client_id=1a6990aa636648e9b2ef855fa7bec2fb)**
 
 ```python
@@ -214,7 +199,54 @@
 
     for version in secret.list_versions(iterator=True):  # if iterator=False returns paginated list with ``next_page_token``
         if version.id != secret.current_version.id:
             version.schedule_version_destruction()
             version.cancel_version_destruction()
 
 ```
+
+## Async mode
+
+The client supports asynchronous mode using the aiohttp library. The signature of the methods does not differ from the synchronous implementation.
+
+
+Just import async client:
+
+```python
+
+from yc_lockbox import AsyncYandexLockboxClient
+
+lockbox = AsyncYandexLockboxClient("oauth_or_iam_token")
+```
+
+Alternative:
+
+```python
+
+from yc_lockbox import YandexLockboxFacade
+
+lockbox = YandexLockboxFacade("oauth_or_iam_token", enable_async=True).client
+```
+
+Example usage:
+
+```python
+secret: Secret = await lockbox.get_secret("e6qxxxxxxxxxx")
+payload = await secret.payload()
+print(payload.entries)  # list of SecretPayloadEntry objects
+
+# Direct access
+
+entry = payload["secret_entry_1"]  # or payload.get("secret_entry_1")
+
+print(entry.text_value)  # return MASKED value like ***********
+print(entry.reveal_text_value())  # similar to entry.text_value.get_secret_value()
+
+# Async iterators
+
+secret_versions = await secret.list_versions(iterator=True)
+
+async for version in secret_versions:
+    if version.id != secret.current_version.id:
+        await version.schedule_version_destruction()
+        await version.cancel_version_destruction()
+```
```

### Comparing `yc-lockbox-0.1.3/README.md` & `yc-lockbox-0.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,46 @@
+Metadata-Version: 2.1
+Name: yc-lockbox
+Version: 0.2.0
+Summary: Yandex Lockbox client
+Home-page: https://github.com/akimrx/python-yc-lockbox
+Author: Akim Faskhutdinov
+Author-email: akimstrong@yandex.ru
+License: MIT
+Keywords: yandex,cloud,vault,secrets,lockbox
+Platform: osx
+Platform: linux
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Typing :: Typed
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: aio
+License-File: LICENSE
+
 # Yandex Lockbox Client
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/yc-lockbox.svg)](https://pypi.org/project/yc-lockbox/)
 [![PyPi Package](https://img.shields.io/pypi/v/yc-lockbox.svg)](https://pypi.org/project/yc-lockbox/)
 [![Codecov](https://codecov.io/gh/akimrx/python-yc-lockbox/branch/master/graph/badge.svg)](https://app.codecov.io/gh/akimrx/python-yc-lockbox)
 [![Tests](https://github.com/akimrx/python-yc-lockbox/workflows/Tests/badge.svg)](https://github.com/akimrx/python-yc-lockbox)
 
 This library is a simple client for working with **[Yandex Lockbox](https://cloud.yandex.ru/en/docs/lockbox/)** over [REST API](https://cloud.yandex.ru/en/docs/lockbox/api-ref/), simplifying work with secrets and allowing you to work with them in the OOP paradigm.
 
+Supports two modes: synchronous and asynchronous.
+
 **[Full library documentation link](https://akimrx.github.io/python-yc-lockbox/)**
 
 **Supported Python versions**:
 
 * 3.10
 * 3.11
 * 3.12
@@ -19,46 +49,57 @@
 
 * [Pydantic V2](https://github.com/pydantic/pydantic)
 * [Crypthography](https://github.com/pyca/cryptography)
 * [PyJWT](https://github.com/jpadilla/pyjwt)
 * [Requests](https://github.com/psf/requests)
 
 
+**Extra dependencies:**
+
+* [aiohttp](https://github.com/aio-libs/aiohttp)
+
+
 **Currently, the following operations are not supported by the library:**
 
 * List secret access bindings
 * Set secret access bindings
 * Update secret access bindings
 * List secret operations
 
 
 **In the near future release:**
 
-- [ ] Async client implementation
+- [x] Tests
+- [x] Async client implementation
 - [ ] Implement access bindings methods and view operations
-- [ ] Tests
 - [ ] Ansible action and lookup plugins
 
 
 ## Install
 
-Installing with PIP:
+Installing via [pip](https://pypi.org/project/yc-lockbox/):
 
 ```
 pip install yc-lockbox
 ```
 
 Also, you can install from source with:
 
 ```
 git clone https://github.com/akimrx/python-yc-lockbox
 cd python-yc-lockbox 
 make install
 ```
 
+For async mode support use
+
+```
+pip install yc-lockbox[aio]
+```
+
 
 ## Usage
 
 
 * **Authenticate via your [OAuth token](https://oauth.yandex.com/authorize?response_type=token&client_id=1a6990aa636648e9b2ef855fa7bec2fb)**
 
 ```python
@@ -185,8 +226,55 @@
     secret.activate()
 
     for version in secret.list_versions(iterator=True):  # if iterator=False returns paginated list with ``next_page_token``
         if version.id != secret.current_version.id:
             version.schedule_version_destruction()
             version.cancel_version_destruction()
 
-```
+```
+
+## Async mode
+
+The client supports asynchronous mode using the aiohttp library. The signature of the methods does not differ from the synchronous implementation.
+
+
+Just import async client:
+
+```python
+
+from yc_lockbox import AsyncYandexLockboxClient
+
+lockbox = AsyncYandexLockboxClient("oauth_or_iam_token")
+```
+
+Alternative:
+
+```python
+
+from yc_lockbox import YandexLockboxFacade
+
+lockbox = YandexLockboxFacade("oauth_or_iam_token", enable_async=True).client
+```
+
+Example usage:
+
+```python
+secret: Secret = await lockbox.get_secret("e6qxxxxxxxxxx")
+payload = await secret.payload()
+print(payload.entries)  # list of SecretPayloadEntry objects
+
+# Direct access
+
+entry = payload["secret_entry_1"]  # or payload.get("secret_entry_1")
+
+print(entry.text_value)  # return MASKED value like ***********
+print(entry.reveal_text_value())  # similar to entry.text_value.get_secret_value()
+
+# Async iterators
+
+secret_versions = await secret.list_versions(iterator=True)
+
+async for version in secret_versions:
+    if version.id != secret.current_version.id:
+        await version.schedule_version_destruction()
+        await version.cancel_version_destruction()
+```
```

### Comparing `yc-lockbox-0.1.3/pyproject.toml` & `yc-lockbox-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yc-lockbox-0.1.3/setup.py` & `yc-lockbox-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `yc-lockbox-0.1.3/yc_lockbox/__init__.py` & `yc-lockbox-0.2.0/yc_lockbox/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,34 +20,36 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-from yc_lockbox._lockbox import YandexLockboxClient
+from yc_lockbox._lockbox import AsyncYandexLockboxClient, YandexLockboxClient, YandexLockboxFacade
 from yc_lockbox._models import (
     Secret,
     INewSecretPayloadEntry,
     INewSecret,
     INewSecretVersion,
     IUpdateSecret,
     Operation,
     YandexCloudError,
 )
 
-__version__ = "0.1.3"
+__version__ = "0.2.0"
 __author__ = "Akim Faskhutdinov"
 __author_email__ = "akimstrong@yandex.ru"
 __license__ = "MIT"
 __url__ = "https://github.com/akimrx/python-yc-lockbox"
 
 __all__ = [
     "Secret",
     "INewSecretPayloadEntry",
     "INewSecret",
     "INewSecretVersion",
     "IUpdateSecret",
+    "AsyncYandexLockboxClient",
     "YandexLockboxClient",
+    "YandexLockboxFacade",
     "Operation",
     "YandexCloudError",
 ]
```

### Comparing `yc-lockbox-0.1.3/yc_lockbox/_abc.py` & `yc-lockbox-0.2.0/yc_lockbox/_abc.py`

 * *Files identical despite different names*

### Comparing `yc-lockbox-0.1.3/yc_lockbox/_adapters.py` & `yc-lockbox-0.2.0/yc_lockbox/_adapters.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,17 @@
         except ImportError:
             raise ImportError(
                 "Async mode is unavailable cause mandatory library ``aiohttp`` is not installed. "
                 "Install ``aiohttp`` directly ``pip install aiohttp`` "
                 "or use ``pip install yc-lockbox[aio]`` for resolve it."
             )
 
+        if params is not None:
+            params = {k: v for k, v in params.items() if v is not None}  # aiohttp don't like NoneType
+
         async with aiohttp.ClientSession() as session:
             async with session.request(
                 method=method, url=url, data=data, json=json, headers=headers, params=params, **kwargs
             ) as response:
 
                 if response.status >= 400:
                     response_message = await response.read()
```

### Comparing `yc-lockbox-0.1.3/yc_lockbox/_auth.py` & `yc-lockbox-0.2.0/yc_lockbox/_auth.py`

 * *Files identical despite different names*

### Comparing `yc-lockbox-0.1.3/yc_lockbox/_constants.py` & `yc-lockbox-0.2.0/yc_lockbox/_constants.py`

 * *Files identical despite different names*

### Comparing `yc-lockbox-0.1.3/yc_lockbox/_lockbox.py` & `yc-lockbox-0.2.0/yc_lockbox/_lockbox.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
-from typing import Type, Optional, Callable, Iterator
+from typing import Any, AsyncGenerator, Coroutine, Type, Optional, Callable, Iterator
 
 from yc_lockbox._abc import AbstractYandexAuthClient, AbstractYandexLockboxClient, AbstractHTTPAdapter
-from yc_lockbox._adapters import HTTPAdapter
+from yc_lockbox._adapters import HTTPAdapter, AsyncHTTPAdapter
 from yc_lockbox._auth import YandexAuthClient
 from yc_lockbox._models import (
     Secret,
     SecretPayload,
     SecretVersion,
     SecretsList,
     SecretVersionsList,
@@ -475,27 +475,534 @@
 
     # TODO: implement
     def update_secret_access_bindings(self, *args, **kwargs):
         """Not ready yet."""
         raise NotImplementedError
 
 
-# TODO: implement
 class AsyncYandexLockboxClient(AbstractYandexLockboxClient):
-    """The same as :class:`YandexLockboxClient` but async."""
+    """
+    Yandex Lockbox secrets vault client.
+    The same as :class:`YandexLockboxClient` but async.
+
+    :param credentials: Credentials for authenticate requests.
+        Allowed types: service account key, OAuth token, IAM token.
+    :param auth_client: Optional client implementation for authenticate requests.
+        Defaults to ``YandexAuthClient``.
+    :param adapter: HTTP adapter for communicate with Yandex Cloud API.
+    :param lockbox_base_url: Lockbox base URL without resource path.
+    :param payload_lockbox_base_url: Lockbox payload base URL without resource path.
+    :param auth_base_url: IAM base URL without resource path.
+
+    .. note::
+
+        All the values of the secrets are masked, i.e. looks like ``***********``.
+        To get the real value of the secret, you need to call the injected methods
+        :func:`reveal_text_value()` or :func:`reveal_binary_value()`.
+
+    Usage::
+
+        from yc_lockbox import AsyncYandexLockboxClient, Secret
+
+        lockbox = AsyncYandexLockboxClient("y0_AgAEXXXXXXXXXXXXXXXXXXXXXXXXX")  # OAuth or IAM token
+
+        secret: Secret = await lockbox.get_secret("e6xxxxxxxxxxxxxxxx")
+        print(secret.name, secret.status, secret.description)
+
+        secret_versions = await secret.list_versions()
+        async for version in secret_versions:
+            print(version)
+            if version.id != secret.current_version.id:
+                await version.schedule_version_destruction()
+
+        payload = await secret.payload()
+
+        try:
+            value = payload["mykey"]
+            print(value.reveal_text_value())
+        except KeyError:
+            print("Invalid key!")
+
+        print(payload.get("foo"))  # None if not exists without raising exception
+        entry = payload[0]  # similar to payload.entries[0]
 
-    def __init__(self, *args, **kwargs) -> None:
-        raise NotImplementedError  # pragma: no cover
+    Authenticate via service account key::
 
+        import json
+
+        # generate json key for your SA
+        # yc iam key create --service-account-name my-sa --output key.json
+
+        with open("./key.json", "r") as infile:
+            credentials = json.load(infile)
+
+        lockbox = AsyncYandexLockboxClient(credentials)
 
-# TODO: implement
-class YandexLockbox:
+    """
+
+    enable_async = True
+
+    def __init__(
+        self,
+        credentials,
+        *,
+        auth_client: Optional[Type[AbstractYandexAuthClient]] = YandexAuthClient,
+        adapter: Optional[Type[AbstractHTTPAdapter]] = AsyncHTTPAdapter,
+        lockbox_base_url: str | None = None,
+        payload_lockbox_base_url: str | None = None,
+    ) -> None:
+        super().__init__(
+            lockbox_base_url=lockbox_base_url,
+            payload_lockbox_base_url=payload_lockbox_base_url,
+        )
+        self.auth: AbstractYandexAuthClient = auth_client(credentials)
+        self.adapter: AbstractHTTPAdapter = adapter
+
+    @property
+    def auth_headers(self) -> dict[str, str]:
+        """Returns headers for authenticate."""
+        return self.auth.get_auth_headers()
+
+    def _inject_client_to_items(self, items: list[T]) -> list[T]:
+        """Inject this client to each response model."""
+        return list(map(lambda item: item.inject_client(self), items))
+
+    async def _seekable_response(
+        self, func: Callable[..., BasePaginatedResponse], entrypoint: str, *args, **kwargs
+    ) -> AsyncGenerator[Any, T]:
+        """
+        Requests all data from the API using the generators, instead of a page-by-page response.
+        This method does not works with dict. Be careful.
+        Returns list of objects from model entrypoint.
+
+        :param func: Adapter func to get data from API.
+        :param entrypoint: Response attribute that contains list of useful data items.
+        :param args: Arguments for func. Will be passed when called inside.
+        :param kwargs: Keyword arguments for func. Similar to ``args``.
+        """
+
+        if kwargs.get("params") is None:
+            raise TypeError(
+                "This method works only with query string parameters. Check keyword arguments to resolve it."
+            )
+
+        next_token = ""  # nosec B105
+
+        while next_token is not None:
+            # There could potentially be a problem if some request doesn't have a 'pageToken' in query string params.
+            # However, this is already a question for a non-consistent API, I think.
+            # An unlikely story, but worth keeping in mind.
+            kwargs["params"]["pageToken"] = next_token
+
+            response = await func(*args, **kwargs)
+            next_token = response.next_page_token  # None or a new token from the API
+
+            if not hasattr(response, entrypoint):
+                raise AttributeError(f"Entrypoint {entrypoint} not exists in response model.")
+
+            for item in getattr(response, entrypoint):
+                if not hasattr(item, "inject_client"):
+                    raise AttributeError(
+                        f"Incorrect item. Method 'inject_client' is not exists in {item.__class__} {type(item)}"
+                    )
+                item.inject_client(self)
+                yield item
+
+    async def activate_secret(
+        self, secret_id: str, raise_for_status: bool = True
+    ) -> Coroutine[Any, Any, Operation | YandexCloudError]:
+        """
+        Activates the specified secret.
+
+        :param secret_id: Secret indentifier.
+        :param raise_for_status: If set to ``False`` returns :class:`YandexCloudError` instead throw exception.
+            Defaults to ``True``.
+        """
+        url = f"{self.lockbox_base_url}/secrets/{secret_id}:activate"
+        response = await self.adapter.request(
+            "POST",
+            url,
+            headers=self.auth_headers,
+            response_model=Operation,
+            raise_for_status=raise_for_status,
+        )
+        response.inject_client(self)
+        return response
+
+    async def add_secret_version(
+        self, secret_id: str, version: INewSecretVersion, raise_for_status: bool = True
+    ) -> Coroutine[Any, Any, Operation | YandexCloudError]:
+        """
+        Adds new version based on a previous one.
+
+        :param secret_id: Secret indentifier.
+        :param version: A new version object.
+        :param raise_for_status: If set to ``False`` returns :class:`YandexCloudError` instead throw exception.
+            Defaults to ``True``.
+        """
+        url = f"{self.lockbox_base_url}/secrets/{secret_id}:addVersion"
+        payload = version.model_dump_json(by_alias=True, exclude_none=True)
+        response = await self.adapter.request(
+            "POST",
+            url,
+            headers=self.auth_headers,
+            data=payload,
+            response_model=Operation,
+            raise_for_status=raise_for_status,
+        )
+        response.inject_client(self)
+        return response
+
+    async def create_secret(
+        self, secret: INewSecret, raise_for_status: bool = True
+    ) -> Coroutine[Any, Any, Operation | YandexCloudError]:
+        """
+        Creates a secret in the specified folder.
+
+        :param secret: A new secret object.
+        :param raise_for_status: If set to ``False`` returns :class:`YandexCloudError` instead throw exception.
+            Defaults to ``True``.
+        """
+        url = f"{self.lockbox_base_url}/secrets"
+        payload = secret.model_dump_json(by_alias=True, exclude_none=True)
+        response = await self.adapter.request(
+            "POST",
+            url,
+            headers=self.auth_headers,
+            data=payload,
+            response_model=Operation,
+            raise_for_status=raise_for_status,
+        )
+        response.inject_client(self)
+        return response
+
+    async def cancel_secret_version_destruction(
+        self, secret_id: str, version_id: str, raise_for_status: bool = True
+    ) -> Coroutine[Any, Any, Operation | YandexCloudError]:
+        """
+        Cancels previously scheduled version destruction, if the version hasn't been destroyed yet.
+
+        :param secret_id: Secret indentifier.
+        :param version_id: Secret version id to cancel destruction.
+        :param raise_for_status: If set to ``False`` returns :class:`YandexCloudError` instead throw exception.
+            Defaults to ``True``.
+        """
+        url = f"{self.lockbox_base_url}/secrets/{secret_id}:cancelVersionDestruction"
+        payload = {"versionId": version_id}
+        response = await self.adapter.request(
+            "POST",
+            url,
+            headers=self.auth_headers,
+            json=payload,
+            response_model=Operation,
+            raise_for_status=raise_for_status,
+        )
+        response.inject_client(self)
+        return response
+
+    async def deactivate_secret(
+        self, secret_id: str, raise_for_status: bool = True
+    ) -> Coroutine[Any, Any, Operation | YandexCloudError]:
+        """
+        Deactivate a secret.
+
+        :param secret_id: Secret indentifier.
+        :param raise_for_status: If set to ``False`` returns :class:`YandexCloudError` instead throw exception.
+            Defaults to ``True``.
+        """
+        url = f"{self.lockbox_base_url}/secrets/{secret_id}:deactivate"
+        response = await self.adapter.request(
+            "POST",
+            url,
+            headers=self.auth_headers,
+            response_model=Operation,
+            raise_for_status=raise_for_status,
+        )
+        response.inject_client(self)
+        return response
+
+    async def delete_secret(
+        self, secret_id: str, raise_for_status: bool = True
+    ) -> Coroutine[Any, Any, Operation | YandexCloudError]:
+        """
+        Deletes the specified secret.
+
+        :param secret_id: Secret indentifier.
+        :param raise_for_status: If set to ``False`` returns :class:`YandexCloudError` instead throw exception.
+            Defaults to ``True``.
+        """
+        url = f"{self.lockbox_base_url}/secrets/{secret_id}"
+        response = await self.adapter.request(
+            "DELETE",
+            url,
+            headers=self.auth_headers,
+            response_model=Operation,
+            raise_for_status=raise_for_status,
+        )
+        response.inject_client(self)
+        return response
+
+    async def get_secret(
+        self, secret_id: str, raise_for_status: bool = True
+    ) -> Coroutine[Any, Any, Secret | YandexCloudError]:
+        """
+        Get lockbox secret by ID.
+
+        :param secret_id: Secret identifier.
+        :param raise_for_status: If set to ``False`` returns :class:`YandexCloudError` instead throw exception.
+            Defaults to ``True``.
+        """
+        url = f"{self.lockbox_base_url}/secrets/{secret_id}"
+        response = await self.adapter.request(
+            "GET",
+            url,
+            headers=self.auth_headers,
+            response_model=Secret,
+            raise_for_status=raise_for_status,
+        )
+        response.inject_client(self)
+        return response
+
+    async def get_secret_payload(
+        self,
+        secret_id: str,
+        version_id: str | None = None,
+        raise_for_status: bool = True,
+    ) -> Coroutine[Any, Any, SecretPayload | YandexCloudError]:
+        """
+        Get lockbox secret payload by ID and optional version.
+
+        :param secret_id: Secret identifier.
+        :param version_id: Secret version. Optional.
+        :param raise_for_status: If set to ``False`` returns :class:`YandexCloudError` instead throw exception.
+            Defaults to ``True``.
+        """
+        url = f"{self.payload_lockbox_base_url}/secrets/{secret_id}/payload"
+        params = {"version_id": version_id} if version_id else None
+        return await self.adapter.request(
+            "GET",
+            url,
+            headers=self.auth_headers,
+            response_model=SecretPayload,
+            raise_for_status=raise_for_status,
+            params=params,
+        )
+
+    async def list_secrets(
+        self,
+        folder_id: str,
+        page_size: int = 100,
+        page_token: str | None = None,
+        raise_for_status: bool = True,
+        iterator: bool = False,
+    ) -> Coroutine[Any, Any, SecretsList | YandexCloudError] | AsyncGenerator[Any, Secret]:
+        """
+        Retrieves the list of secrets in the specified folder.
+
+        :param folder_id: ID of the folder to list secrets in.
+        :param page_size: The maximum number of results per page to return.
+            If the number of available results is larger than ``page_size``,
+            the service returns a ``next_page_token`` that can be used to get
+            the next page of results in subsequent list requests.
+            Default value: ``100``.
+            The maximum value is ``1000``.
+        :param page_token: Page token. To get the next page of results, set ``page_token``
+            to the ``next_page_token`` returned by a previous list request.
+        :param iterator: Returns all data as iterator (generator) instead paginated result.
+        """
+        args = (
+            "GET",
+            f"{self.lockbox_base_url}/secrets",
+        )
+        kwargs = {
+            "headers": self.auth_headers,
+            "params": {"folderId": folder_id, "pageSize": page_size, "pageToken": page_token},
+            "response_model": SecretsList,
+            "raise_for_status": raise_for_status,
+        }
+
+        if iterator:
+            return self._seekable_response(self.adapter.request, "secrets", *args, **kwargs)
+
+        response = await self.adapter.request(*args, **kwargs)
+        self._inject_client_to_items(response.secrets)
+        return response
+
+    # TODO: implement
+    async def list_secret_access_bindings(self, *args, **kwargs):
+        """Not ready yet."""
+        raise NotImplementedError
+
+    # TODO: implement
+    async def list_secret_operations(self, *args, **kwargs):
+        """Not ready yet."""
+        raise NotImplementedError
+
+    async def list_secret_versions(
+        self,
+        secret_id: str,
+        page_size: int = 100,
+        page_token: str | None = None,
+        raise_for_status: bool = True,
+        iterator: bool = False,
+    ) -> Coroutine[Any, Any, SecretVersionsList | YandexCloudError] | AsyncGenerator[Any, SecretVersion]:
+        """
+        Retrieves the list of versions of the specified secret.
+
+        :param secret_id: Secret identifier.
+        :param page_size: The maximum number of results per page to return.
+            If the number of available results is larger than ``page_size``,
+            the service returns a ``next_page_token`` that can be used to get
+            the next page of results in subsequent list requests.
+            Default value: ``100``.
+            The maximum value is ``1000``.
+        :param page_token: Page token. To get the next page of results, set ``page_token``
+            to the ``next_page_token`` returned by a previous list request.
+        :param iterator: Returns all data as iterator (generator) instead paginated result.
+        """
+        args = (
+            "GET",
+            f"{self.lockbox_base_url}/secrets/{secret_id}/versions",
+        )
+        kwargs = {
+            "headers": self.auth_headers,
+            "params": {"pageSize": page_size, "pageToken": page_token},
+            "response_model": SecretVersionsList,
+            "raise_for_status": raise_for_status,
+        }
+
+        if iterator:
+            print("IMA ITERATOR IMA ITERATOR IMA ITERATOR IMA ITERATOR")
+            return self._seekable_response(self.adapter.request, "versions", *args, **kwargs)
+
+        response = await self.adapter.request(*args, **kwargs)
+        self._inject_client_to_items(response.versions)
+        return response
+
+    async def schedule_secret_version_destruction(
+        self, secret_id: str, version_id: str, pending_period: int = 604800, raise_for_status: bool = True
+    ) -> Coroutine[Any, Any, Operation | YandexCloudError]:
+        """
+        Schedules the specified version for destruction.
+        Scheduled destruction can be cancelled with the :func:`cancel_secret_version_destruction()` method.
+
+        :param secret_id: Secret indentifier.
+        :param version_id: ID of the version to be destroyed.
+        :param pending_period: Time interval in seconds between the version destruction request and actual destruction.
+            Default value: ``604800`` (i.e. 7 days).
+        :param raise_for_status: If set to ``False`` returns :class:`YandexCloudError` instead throw exception.
+            Defaults to ``True``.
+        """
+        if isinstance(pending_period, int):
+            if pending_period <= 0:
+                raise ValueError("The ``pending_period`` value must be greater than 0.")
+            # protobuf duration compat
+            # https://github.com/protocolbuffers/protobuf/blob/main/src/google/protobuf/duration.proto
+            pending_period = str(pending_period) + "s"
+        else:
+            raise ValueError("The ``pending_period`` value must be integer.")
+
+        url = f"{self.lockbox_base_url}/secrets/{secret_id}:scheduleVersionDestruction"
+        payload = {"versionId": version_id, "pendingPeriod": pending_period}
+        response = await self.adapter.request(
+            "POST",
+            url,
+            headers=self.auth_headers,
+            json=payload,
+            response_model=Operation,
+            raise_for_status=raise_for_status,
+        )
+        response.inject_client(self)
+        return response
+
+    # TODO: implement
+    async def set_secret_access_bindings(self, *args, **kwargs):
+        """Not ready yet."""
+        raise NotImplementedError
+
+    async def update_secret(
+        self, secret_id: str, data: IUpdateSecret, raise_for_status: bool = True
+    ) -> Coroutine[Any, Any, Operation | YandexCloudError]:
+        """
+        Updates the specified secret.
+
+        :param secret_id: Secret identifier.
+        :param data: A new data for the secret as object.
+            Important. Field mask that specifies which attributes of the secret are going to be updated.
+            A comma-separated names off ALL fields to be updated. Only the specified fields will be changed.
+            The others will be left untouched. If the field is specified in updateMask and no value for
+            that field was sent in the request, the field's value will be reset to the default.
+            The default value for most fields is null or 0.
+            If ``updateMask`` is not sent in the request, all fields values will be updated.
+            Fields specified in the request will be updated to provided values. The rest of the fields will be reset to the default.
+        :param raise_for_status: If set to ``False`` returns :class:`YandexCloudError` instead throw exception.
+            Defaults to ``True``.
+        """
+        url = f"{self.lockbox_base_url}/secrets/{secret_id}"
+        payload = data.model_dump_json(by_alias=True)
+        response = await self.adapter.request(
+            "PATCH",
+            url,
+            headers=self.auth_headers,
+            data=payload,
+            response_model=Operation,
+            raise_for_status=raise_for_status,
+        )
+        response.inject_client(self)
+        return response
+
+    # TODO: implement
+    async def update_secret_access_bindings(self, *args, **kwargs):
+        """Not ready yet."""
+        raise NotImplementedError
+
+
+class YandexLockboxFacade:  # pragma: no cover
     """
     A facade for encapsulating the logic of synchronous and asynchronous client operations,
     providing uniform methods.
     """
 
-    def __init__(self) -> None:
-        raise NotImplementedError  # pragma: no cover
+    _client: AbstractYandexLockboxClient
+
+    def __init__(
+        self,
+        credentials,
+        *,
+        auth_client: Optional[Type[AbstractYandexAuthClient]] = YandexAuthClient,
+        lockbox_base_url: str | None = None,
+        payload_lockbox_base_url: str | None = None,
+        enable_async: bool = False,
+    ) -> None:
+        if enable_async:
+            self._client = AsyncYandexLockboxClient(
+                credentials,
+                auth_client=auth_client,
+                lockbox_base_url=lockbox_base_url,
+                payload_lockbox_base_url=payload_lockbox_base_url,
+            )
+        else:
+            self._client = YandexLockboxClient(
+                credentials,
+                auth_client=auth_client,
+                lockbox_base_url=lockbox_base_url,
+                payload_lockbox_base_url=payload_lockbox_base_url,
+            )
+
+    @property
+    def client(self) -> AbstractYandexLockboxClient:
+        """Returns initialized Lockbox client."""
+        return self._client
+
+    def __getattr__(self, name):
+        """Dynamically delegate method calls to the appropriate client."""
+
+        if name == "_client":
+            return self._client
+
+        if not hasattr(self._client, name):
+            raise AttributeError
+
+        return getattr(self._client, name)
 
 
-__all__ = ["AsyncYandexLockboxClient", "YandexLockboxClient", "YandexLockbox"]
+__all__ = ["AsyncYandexLockboxClient", "YandexLockboxClient", "YandexLockboxFacade"]
```

### Comparing `yc-lockbox-0.1.3/yc_lockbox/_models.py` & `yc-lockbox-0.2.0/yc_lockbox/_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
-from typing import Any, Iterator, Union
+from typing import Any, AsyncGenerator, Iterator, Union
 from datetime import datetime
 from pydantic import BaseModel, ConfigDict, Field, SecretStr, SecretBytes, computed_field
 
 from yc_lockbox._constants import RpcError
 from yc_lockbox._abc import AbstractYandexLockboxClient
-from yc_lockbox._types import T
+from yc_lockbox._types import T, SecretVersionsResponse
 from yc_lockbox._exceptions import LockboxError
 
 
 logger = logging.getLogger(__name__)
 
 
 class BaseDomainModel(BaseModel):
@@ -239,32 +239,46 @@
         return self.client.deactivate_secret(self.id, **kwargs)
 
     def delete(self, **kwargs) -> Union["Operation", "YandexCloudError"]:
         """Shortcut for delete the current secret."""
         self._raise_when_empty_client()
         return self.client.delete_secret(self.id, **kwargs)
 
-    def refresh(self, **kwargs) -> "Secret":
-        """Shortcut for refresh attributes for this secret."""
-        self._raise_when_empty_client()
+    async def _async_refresh(self, **kwargs) -> "Secret":
+        data = await self.client.get_secret(self.id, **kwargs)
+        self._update_attributes(data)
+        return self
+
+    def _sync_refresh(self, **kwargs) -> "Secret":
         data = self.client.get_secret(self.id, **kwargs)
+        self._update_attributes(data)
+        return self
 
+    def _update_attributes(self, data) -> None:
+        """Method for update model attributes after refresh."""
         for attr, value in data.model_dump().items():
-            if value != getattr(self, attr):
+            if value != getattr(self, attr, None):
                 setattr(self, attr, value)
 
-        return data
+    def refresh(self, **kwargs) -> "Secret":
+        """Shortcut for refresh attributes for this secret."""
+        self._raise_when_empty_client()
+
+        if hasattr(self.client, "enable_async") and self.client.enable_async:
+            return self._async_refresh(**kwargs)
+
+        return self._sync_refresh(**kwargs)
 
     def payload(self, version_id: str | None = None, **kwargs) -> Union["Operation", "YandexCloudError"]:
         self._raise_when_empty_client()
         return self.client.get_secret_payload(self.id, version_id, **kwargs)
 
     def list_versions(
         self, page_size: int = 100, page_token: str | None = None, iterator: bool = False, **kwargs
-    ) -> Union["SecretVersionsList", Iterator["SecretVersion"], "YandexCloudError"]:
+    ) -> SecretVersionsResponse:
         """Shortcut for list all available versions of the current secret."""
         self._raise_when_empty_client()
         return self.client.list_secret_versions(
             self.id, page_size=page_size, page_token=page_token, iterator=iterator, **kwargs
         )
 
     def schedule_version_destruction(
```

### Comparing `yc-lockbox-0.1.3/yc_lockbox.egg-info/PKG-INFO` & `yc-lockbox-0.2.0/yc_lockbox.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yc-lockbox
-Version: 0.1.3
+Version: 0.2.0
 Summary: Yandex Lockbox client
 Home-page: https://github.com/akimrx/python-yc-lockbox
 Author: Akim Faskhutdinov
 Author-email: akimstrong@yandex.ru
 License: MIT
 Keywords: yandex,cloud,vault,secrets,lockbox
 Platform: osx
@@ -31,14 +31,16 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/yc-lockbox.svg)](https://pypi.org/project/yc-lockbox/)
 [![PyPi Package](https://img.shields.io/pypi/v/yc-lockbox.svg)](https://pypi.org/project/yc-lockbox/)
 [![Codecov](https://codecov.io/gh/akimrx/python-yc-lockbox/branch/master/graph/badge.svg)](https://app.codecov.io/gh/akimrx/python-yc-lockbox)
 [![Tests](https://github.com/akimrx/python-yc-lockbox/workflows/Tests/badge.svg)](https://github.com/akimrx/python-yc-lockbox)
 
 This library is a simple client for working with **[Yandex Lockbox](https://cloud.yandex.ru/en/docs/lockbox/)** over [REST API](https://cloud.yandex.ru/en/docs/lockbox/api-ref/), simplifying work with secrets and allowing you to work with them in the OOP paradigm.
 
+Supports two modes: synchronous and asynchronous.
+
 **[Full library documentation link](https://akimrx.github.io/python-yc-lockbox/)**
 
 **Supported Python versions**:
 
 * 3.10
 * 3.11
 * 3.12
@@ -47,46 +49,57 @@
 
 * [Pydantic V2](https://github.com/pydantic/pydantic)
 * [Crypthography](https://github.com/pyca/cryptography)
 * [PyJWT](https://github.com/jpadilla/pyjwt)
 * [Requests](https://github.com/psf/requests)
 
 
+**Extra dependencies:**
+
+* [aiohttp](https://github.com/aio-libs/aiohttp)
+
+
 **Currently, the following operations are not supported by the library:**
 
 * List secret access bindings
 * Set secret access bindings
 * Update secret access bindings
 * List secret operations
 
 
 **In the near future release:**
 
-- [ ] Async client implementation
+- [x] Tests
+- [x] Async client implementation
 - [ ] Implement access bindings methods and view operations
-- [ ] Tests
 - [ ] Ansible action and lookup plugins
 
 
 ## Install
 
-Installing with PIP:
+Installing via [pip](https://pypi.org/project/yc-lockbox/):
 
 ```
 pip install yc-lockbox
 ```
 
 Also, you can install from source with:
 
 ```
 git clone https://github.com/akimrx/python-yc-lockbox
 cd python-yc-lockbox 
 make install
 ```
 
+For async mode support use
+
+```
+pip install yc-lockbox[aio]
+```
+
 
 ## Usage
 
 
 * **Authenticate via your [OAuth token](https://oauth.yandex.com/authorize?response_type=token&client_id=1a6990aa636648e9b2ef855fa7bec2fb)**
 
 ```python
@@ -214,7 +227,54 @@
 
     for version in secret.list_versions(iterator=True):  # if iterator=False returns paginated list with ``next_page_token``
         if version.id != secret.current_version.id:
             version.schedule_version_destruction()
             version.cancel_version_destruction()
 
 ```
+
+## Async mode
+
+The client supports asynchronous mode using the aiohttp library. The signature of the methods does not differ from the synchronous implementation.
+
+
+Just import async client:
+
+```python
+
+from yc_lockbox import AsyncYandexLockboxClient
+
+lockbox = AsyncYandexLockboxClient("oauth_or_iam_token")
+```
+
+Alternative:
+
+```python
+
+from yc_lockbox import YandexLockboxFacade
+
+lockbox = YandexLockboxFacade("oauth_or_iam_token", enable_async=True).client
+```
+
+Example usage:
+
+```python
+secret: Secret = await lockbox.get_secret("e6qxxxxxxxxxx")
+payload = await secret.payload()
+print(payload.entries)  # list of SecretPayloadEntry objects
+
+# Direct access
+
+entry = payload["secret_entry_1"]  # or payload.get("secret_entry_1")
+
+print(entry.text_value)  # return MASKED value like ***********
+print(entry.reveal_text_value())  # similar to entry.text_value.get_secret_value()
+
+# Async iterators
+
+secret_versions = await secret.list_versions(iterator=True)
+
+async for version in secret_versions:
+    if version.id != secret.current_version.id:
+        await version.schedule_version_destruction()
+        await version.cancel_version_destruction()
+```
```

