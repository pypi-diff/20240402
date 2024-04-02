# Comparing `tmp/authx_extra-1.0.0.tar.gz` & `tmp/authx_extra-1.1.0.tar.gz`

## Comparing `authx_extra-1.0.0.tar` & `authx_extra-1.1.0.tar`

### file list

```diff
@@ -1,35 +1,44 @@
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 authx_extra-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 authx_extra-1.0.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 authx_extra-1.0.0/.github/dependabot.yaml
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 authx_extra-1.0.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 authx_extra-1.0.0/.github/workflows/release.yml
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 authx_extra-1.0.0/authx_extra/__init__.py
--rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 authx_extra-1.0.0/authx_extra/cache.py
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 authx_extra-1.0.0/authx_extra/metrics.py
--rw-r--r--   0        0        0     6960 2020-02-02 00:00:00.000000 authx_extra-1.0.0/authx_extra/oauth2.py
--rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 authx_extra-1.0.0/authx_extra/profiler.py
--rw-r--r--   0        0        0     8873 2020-02-02 00:00:00.000000 authx_extra-1.0.0/authx_extra/session.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx_extra-1.0.0/authx_extra/addons/__init__.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 authx_extra-1.0.0/authx_extra/addons/expiry.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 authx_extra-1.0.0/authx_extra/addons/keys.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx_extra-1.0.0/authx_extra/extra/__init__.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 authx_extra-1.0.0/authx_extra/extra/_cache.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 authx_extra-1.0.0/scripts/clean.sh
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 authx_extra-1.0.0/scripts/docker.sh
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 authx_extra-1.0.0/scripts/format.sh
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 authx_extra-1.0.0/scripts/lint.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx_extra-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     6438 2020-02-02 00:00:00.000000 authx_extra-1.0.0/tests/test_cache.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 authx_extra-1.0.0/tests/test_keys.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 authx_extra-1.0.0/tests/test_method_cache.py
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 authx_extra-1.0.0/tests/test_metrics.py
--rw-r--r--   0        0        0    15068 2020-02-02 00:00:00.000000 authx_extra-1.0.0/tests/test_oauth2.py
--rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 authx_extra-1.0.0/tests/test_profiler.py
--rw-r--r--   0        0        0     7306 2020-02-02 00:00:00.000000 authx_extra-1.0.0/tests/test_session_middleware.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 authx_extra-1.0.0/tests/test_skip_session_header_check_dict.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 authx_extra-1.0.0/tests/test_skip_session_header_check_list.py
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 authx_extra-1.0.0/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 authx_extra-1.0.0/LICENSE
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 authx_extra-1.0.0/README.md
--rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 authx_extra-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 authx_extra-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 authx_extra-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 authx_extra-1.1.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 authx_extra-1.1.0/.github/dependabot.yaml
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 authx_extra-1.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 authx_extra-1.1.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 authx_extra-1.1.0/authx_extra/__init__.py
+-rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 authx_extra-1.1.0/authx_extra/cache.py
+-rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 authx_extra-1.1.0/authx_extra/metrics.py
+-rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 authx_extra-1.1.0/authx_extra/oauth2.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 authx_extra-1.1.0/authx_extra/profiler.py
+-rw-r--r--   0        0        0     9282 2020-02-02 00:00:00.000000 authx_extra-1.1.0/authx_extra/session.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx_extra-1.1.0/authx_extra/addons/__init__.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 authx_extra-1.1.0/authx_extra/addons/expiry.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 authx_extra-1.1.0/authx_extra/addons/keys.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx_extra-1.1.0/authx_extra/extra/__init__.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 authx_extra-1.1.0/authx_extra/extra/_cache.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 authx_extra-1.1.0/requirements/all.txt
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 authx_extra-1.1.0/requirements/linting.in
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 authx_extra-1.1.0/requirements/linting.txt
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 authx_extra-1.1.0/requirements/optional.in
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 authx_extra-1.1.0/requirements/optional.txt
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 authx_extra-1.1.0/requirements/pyproject.txt
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 authx_extra-1.1.0/requirements/testing.in
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 authx_extra-1.1.0/requirements/testing.txt
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 authx_extra-1.1.0/scripts/clean.sh
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 authx_extra-1.1.0/scripts/docker.sh
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 authx_extra-1.1.0/scripts/format.sh
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 authx_extra-1.1.0/scripts/lint.sh
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 authx_extra-1.1.0/scripts/requirements.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx_extra-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     6560 2020-02-02 00:00:00.000000 authx_extra-1.1.0/tests/test_cache.py
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 authx_extra-1.1.0/tests/test_keys.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 authx_extra-1.1.0/tests/test_method_cache.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 authx_extra-1.1.0/tests/test_metrics.py
+-rw-r--r--   0        0        0    15238 2020-02-02 00:00:00.000000 authx_extra-1.1.0/tests/test_oauth2.py
+-rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 authx_extra-1.1.0/tests/test_profiler.py
+-rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 authx_extra-1.1.0/tests/test_session_middleware.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 authx_extra-1.1.0/tests/test_skip_session_header_check_dict.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 authx_extra-1.1.0/tests/test_skip_session_header_check_list.py
+-rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 authx_extra-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 authx_extra-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 authx_extra-1.1.0/README.md
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 authx_extra-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 authx_extra-1.1.0/PKG-INFO
```

### Comparing `authx_extra-1.0.0/.github/workflows/ci.yml` & `authx_extra-1.1.0/.github/workflows/ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -16,19 +16,26 @@
 
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
-      - name: Install Dependencies
-        run: pip install -e .[lint,cache,profiler,oauth2,metrics]
-      - uses: pre-commit/action@v3.0.0
+      - name: setup uv
+        uses: yezz123/setup-uv@v4
         with:
-          extra_args: --all-files --verbose
+          uv-version: "0.1.27"
+          uv-venv: ".venv"
+
+      - name: Install Dependencies
+        run: uv pip install -r requirements/pyproject.txt && uv pip install -r requirements/linting.txt
+
+      - name: Run Pre-commit
+        run: bash scripts/format.sh
+
   test:
     name: test on python ${{ matrix.python-version }}
     runs-on: ubuntu-latest
     services:
       redis:
         image: redis
         ports:
@@ -46,25 +53,31 @@
 
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
+      - name: setup uv
+        uses: yezz123/setup-uv@v4
+        with:
+          uv-version: "0.1.27"
+          uv-venv: ".venv"
       - name: Install Dependencies
-        run: pip install -e .[test,cache,profiler,oauth2,metrics]
-      - name: Freeze dependencies
-        run: pip freeze
-      - name: Test
+        run: uv pip install -r requirements/pyproject.txt && uv pip install -r requirements/optional.txt && uv pip install -r requirements/testing.txt
+      - name: Test Suite
+        run: pytest --cov=authx_extra --cov-report=xml
         env:
           ENV: test
           REDIS_URL: "redis://0.0.0.0:6379"
-        run: pytest --cov=authx_extra --cov=tests --cov-report=html -xv --color=yes --disable-warnings --cov-fail-under=80
       - name: Upload coverage
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
+        with:
+          token: ${{ secrets.CODECOV_TOKEN }}
+          file: ./coverage.xml
 
   # https://github.com/marketplace/actions/alls-green#why used for branch protection checks
   check:
     if: always()
     needs: [lint, test]
     runs-on: ubuntu-latest
     steps:
```

### Comparing `authx_extra-1.0.0/.github/workflows/release.yml` & `authx_extra-1.1.0/.github/workflows/release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,14 @@
       - name: check GITHUB_REF matches package version
         uses: samuelcolvin/check-python-version@v4.1
         with:
           version_file_path: authx_extra/__init__.py
       - name: Build distribution
         run: python -m build
       - name: Publish
-        uses: pypa/gh-action-pypi-publish@v1.8.11
+        uses: pypa/gh-action-pypi-publish@v1.8.14
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
       - name: Dump GitHub context
         env:
           GITHUB_CONTEXT: ${{ toJson(github) }}
         run: echo "$GITHUB_CONTEXT"
```

### Comparing `authx_extra-1.0.0/authx_extra/cache.py` & `authx_extra-1.1.0/authx_extra/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,16 +97,20 @@
 
     def wrapper(func: Callable):
         @wraps(func)
         async def inner(*args, **kwargs):
             try:
                 # extracts the `id` attribute from the `obj_attr` parameter passed to the `@cache` method
                 _obj = kwargs.get(f"{obj}")
-                _key = await HTTPKeys.generate_key(key=key, config=HTTPCache, obj=_obj, obj_attr=obj_attr)
-                _cache = HTTPCacheBackend(redis=HTTPCache.redis_client, namespace=namespace)
+                _key = await HTTPKeys.generate_key(
+                    key=key, config=HTTPCache, obj=_obj, obj_attr=obj_attr
+                )
+                _cache = HTTPCacheBackend(
+                    redis=HTTPCache.redis_client, namespace=namespace
+                )
                 _request = kwargs.get("request")
                 _response = kwargs.get("response")
 
                 # check cache and return if value is present
                 ttl, response = await _cache.get(key=_key)
                 if response:
                     if _request and _response:
@@ -114,15 +118,19 @@
                         _response.headers["Cache-Hit"] = "true"
                     return response
 
                 # if not a cache-hit populate current response.
                 _computed_response = await func(*args, **kwargs)
 
                 # if http request store the response body data
-                _cacheable_response = _computed_response.body if kwargs.get("request", None) else _computed_response
+                _cacheable_response = (
+                    _computed_response.body
+                    if kwargs.get("request", None)
+                    else _computed_response
+                )
 
                 await _cache.set(
                     key=_key,
                     value=_cacheable_response,
                     ttl_in_seconds=ttl_in_seconds,
                     ttl_func=ttl_func,
                     end_of_day=expire_end_of_day,
@@ -155,16 +163,20 @@
 
     def wrapper(func: Callable):
         @wraps(func)
         async def inner(*args, **kwargs):
             try:
                 # extracts the `id` attribute from the `obj_attr` giparameter passed to the `@cache` method
                 _obj = kwargs.get(f"{obj}")
-                _keys = await HTTPKeys.generate_keys(keys=keys, config=HTTPCache, obj=_obj, obj_attr=obj_attr)
-                _cache = HTTPCacheBackend(redis=HTTPCache.redis_client, namespace=namespace)
+                _keys = await HTTPKeys.generate_keys(
+                    keys=keys, config=HTTPCache, obj=_obj, obj_attr=obj_attr
+                )
+                _cache = HTTPCacheBackend(
+                    redis=HTTPCache.redis_client, namespace=namespace
+                )
                 await _cache.invalidate_all(keys=_keys)
                 _computed_response = await func(*args, **kwargs)
                 return _computed_response
             except Exception as e:
                 log_error(msg=f"Cache Error: {e}", e=e, method="cache")
                 return await func(*args, **kwargs)
```

### Comparing `authx_extra-1.0.0/authx_extra/metrics.py` & `authx_extra-1.1.0/authx_extra/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,17 @@
         "Total HTTP requests",
         ("method", "path", "status"),
         registry=get_registry(),
     )
 
 
 @functools.lru_cache()
-def request_time(prefix: str, buckets: typing.Tuple[float, ...]) -> prometheus_client.Histogram:
+def request_time(
+    prefix: str, buckets: typing.Tuple[float, ...]
+) -> prometheus_client.Histogram:
     """Return request time metric for the app prefix (cached/singleton)."""
     return prometheus_client.Histogram(
         f"{prefix}request_duration_seconds",
         "HTTP request duration in seconds",
         ("method", "path", "status"),
         buckets=buckets,
         registry=get_registry(),
```

### Comparing `authx_extra-1.0.0/authx_extra/oauth2.py` & `authx_extra-1.1.0/authx_extra/oauth2.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,17 @@
     if not isinstance(url_or_keys, str) or not url_or_keys.startswith("https://"):
         return url_or_keys
     logger.info("Getting jwk from %s...", url_or_keys)
     with urllib.request.urlopen(url_or_keys) as f:
         return json.loads(f.read().decode())
 
 
-def _validate_provider(provider_name: str, provider: typing.Dict[str, typing.Any]) -> None:
+def _validate_provider(
+    provider_name: str, provider: typing.Dict[str, typing.Any]
+) -> None:
     mandatory_keys = {"issuer", "keys", "audience"}
     if not mandatory_keys.issubset(set(provider)):
         raise ValueError(
             f'Each provider must contain the following keys: {mandatory_keys}. Provider "{provider_name}" is missing {mandatory_keys - set(provider)}.'
         )
 
     keys = provider["keys"]
@@ -39,31 +41,37 @@
 class MiddlewareOauth2:
     def __init__(
         self,
         app: ASGIApp,
         providers: typing.Dict[str, typing.Dict[str, typing.Any]],
         public_paths: typing.Optional[typing.Set[str]] = None,
         get_keys: typing.Optional[typing.Callable[[typing.Any], typing.Any]] = None,
-        key_refresh_minutes: typing.Optional[typing.Union[int, typing.Dict[str, int]]] = None,
+        key_refresh_minutes: typing.Optional[
+            typing.Union[int, typing.Dict[str, int]]
+        ] = None,
     ) -> None:
         self._app = app
         for provider in providers:
             _validate_provider(provider, providers[provider])
         self._providers = providers
         self._get_keys = get_keys or _get_keys
         self._public_paths = public_paths or set()
 
         if key_refresh_minutes is None:
             self._timeout = {provider: None for provider in providers}
         elif isinstance(key_refresh_minutes, dict):
             self._timeout = {
-                provider: datetime.timedelta(minutes=key_refresh_minutes[provider]) for provider in providers
+                provider: datetime.timedelta(minutes=key_refresh_minutes[provider])
+                for provider in providers
             }
         else:
-            self._timeout = {provider: datetime.timedelta(minutes=key_refresh_minutes) for provider in providers}
+            self._timeout = {
+                provider: datetime.timedelta(minutes=key_refresh_minutes)
+                for provider in providers
+            }
 
         # cached attribute and respective timeout
         self._last_retrieval: typing.Dict[str, datetime.datetime] = {}
         self._keys: typing.Dict[str, typing.Any] = {}
 
     def _provider_claims(self, provider: str, token: str) -> typing.Any:
         issuer = self._providers[provider]["issuer"]
@@ -119,22 +127,26 @@
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         request = HTTPConnection(scope)
 
         if request.url.path in self._public_paths:
             return await self._app(scope, receive, send)
 
         # check for authorization header and token on it.
-        if "authorization" in request.headers and request.headers["authorization"].startswith("Bearer "):
+        if "authorization" in request.headers and request.headers[
+            "authorization"
+        ].startswith("Bearer "):
             token = request.headers["authorization"][len("Bearer ") :]
             try:
                 provider, claims = self.claims(token)
                 scope["oauth2-claims"] = claims
                 scope["oauth2-provider"] = provider
             except InvalidToken as e:
-                return await self._prepare_error_response(e.errors, 401, scope, receive, send)
+                return await self._prepare_error_response(
+                    e.errors, 401, scope, receive, send
+                )
         elif "authorization" in request.headers:
             logger.debug('No "Bearer" in authorization header')
             return await self._prepare_error_response(
                 'The "authorization" header must start with "Bearer "',
                 400,
                 scope,
                 receive,
@@ -156,15 +168,18 @@
         if self._keys.get(provider, None) is None:
             # we do not even have the key (first time) => should refresh
             return True
         elif self._timeout[provider] is None:
             # we have a key and no timeout => do not refresh
             return False
         # have the key and have timeout => check if we passed the timeout
-        return self._last_retrieval[provider] + self._timeout[provider] < datetime.datetime.utcnow()
+        return (
+            self._last_retrieval[provider] + self._timeout[provider]
+            < datetime.datetime.utcnow()
+        )
 
     def _refresh_keys(self, provider: str) -> None:
         self._keys[provider] = self._get_keys(self._providers[provider]["keys"])
         self._last_retrieval[provider] = datetime.datetime.utcnow()
 
     def _provider_keys(self, provider: str) -> typing.Any:
         if self._should_refresh(provider):
```

### Comparing `authx_extra-1.0.0/authx_extra/profiler.py` & `authx_extra-1.1.0/authx_extra/profiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,31 +59,40 @@
         try:
             await self.app(scope, receive, wrapped_send)
         finally:
             if scope["type"] == "http":
                 self._profiler.stop()
                 end = time.perf_counter()
                 if self._print_each_request:
-                    print(f"Method: {method}, " f"Path: {path}, " f"Duration: {end - begin}, " f"Status: {status_code}")
+                    print(
+                        f"Method: {method}, "
+                        f"Path: {path}, "
+                        f"Duration: {end - begin}, "
+                        f"Status: {status_code}"
+                    )
                     print(self._profiler.output_text(**self._profiler_kwargs))
 
     async def get_result(self):
         if self._output_type == "text":
             print(self._profiler.output_text(**self._profiler_kwargs))
 
         elif self._output_type == "html":
             html_name = self._profiler_kwargs.get("html_file_name")
             if html_name is None:
                 html_name = "authx_profiling_results.html"
 
-            html_code = renderers.HTMLRenderer().render(session=self._profiler.last_session)
+            html_code = renderers.HTMLRenderer().render(
+                session=self._profiler.last_session
+            )
             with codecs.open(html_name, "w", "utf-8") as f:
                 f.write(html_code)
 
         elif self._output_type == "json":
             json_name = self._profiler_kwargs.get("json_file_name")
             if json_name is None:
                 json_name = "authx_profiling_results.json"
 
-            json_code = renderers.JSONRenderer().render(session=self._profiler.last_session)
+            json_code = renderers.JSONRenderer().render(
+                session=self._profiler.last_session
+            )
             with codecs.open(json_name, "w", "utf-8") as f:
                 f.write(json_code)
```

### Comparing `authx_extra-1.0.0/authx_extra/session.py` & `authx_extra-1.1.0/authx_extra/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,19 +93,23 @@
         cookie[self.session_cookie_name] = signed_session_id
 
         self.logger.debug(
             f"[session_id:'{session_id}'] Creating new Cookie object... cookie[{self.session_cookie_name}]"
         )
 
         if self.http_only:
-            self.logger.debug(f"[session_id:'{session_id}'] cookie[{self.session_cookie_name}]['httponly'] enabled")
+            self.logger.debug(
+                f"[session_id:'{session_id}'] cookie[{self.session_cookie_name}]['httponly'] enabled"
+            )
             cookie[self.session_cookie_name]["httponly"] = True
 
         if self.secure:
-            self.logger.debug(f"[session_id:'{session_id}'] cookie[{self.session_cookie_name}]['secure'] enabled")
+            self.logger.debug(
+                f"[session_id:'{session_id}'] cookie[{self.session_cookie_name}]['secure'] enabled"
+            )
             cookie[self.session_cookie_name]["secure"] = True
 
         if self.max_age > 0:
             self.logger.debug(
                 f"[session_id:'{session_id}'] cookie[{self.session_cookie_name}]['maxage']={self.max_age} enabled"
             )
             cookie[self.session_cookie_name]["max-age"] = self.max_age
@@ -134,27 +138,35 @@
         header_names = []
 
         for header in skip_header:
             header_name = header.get("header_name")
             header_value = header.get("header_value")
             header_names.append(header_name)
 
-            self.logger.debug(f"Use skip_header option. skip_header:'{header_name}':'{header_value}'")
+            self.logger.debug(
+                f"Use skip_header option. skip_header:'{header_name}':'{header_value}'"
+            )
             request_header_value = request.headers.get(header_name)
             self.logger.debug(
                 f"Use skip_header option. Checking request header: '{header_name}':'{request_header_value}'"
             )
-            if (header_value == "*" and request_header_value is not None) or request_header_value == header_value:
+            if (
+                header_value == "*" and request_header_value is not None
+            ) or request_header_value == header_value:
                 self.logger.debug("Use skip_header option. skip_header matched!")
                 return True
 
-        self.logger.debug(f"Use skip_header option. skip_headers:{header_names} not matched in request headers.")
+        self.logger.debug(
+            f"Use skip_header option. skip_headers:{header_names} not matched in request headers."
+        )
         return False
 
-    async def dispatch(self, request: Request, call_next: RequestResponseEndpoint) -> Response:
+    async def dispatch(
+        self, request: Request, call_next: RequestResponseEndpoint
+    ) -> Response:
         """
         Dispatch the request, handling session management.
 
         Args:
             request (Request): The incoming request.
             call_next (RequestResponseEndpoint): The next request handler.
 
@@ -179,35 +191,43 @@
                 session_id = decoded_dict.get(self.session_cookie_name)
                 session_store = self.session_store.get_store(session_id)
 
                 if session_store is None:
                     self.logger.info(
                         f"[session_id:'{session_id}'] Session cookie available. But no store for this sessionId found. Maybe store had cleaned."
                     )
-                    cookie = await self.create_new_session_id_and_store(request, cause="valid_cookie_but_no_store")
+                    cookie = await self.create_new_session_id_and_store(
+                        request, cause="valid_cookie_but_no_store"
+                    )
                 else:
                     self.logger.info(
                         f"[session_id:'{session_id}'] Session cookie and Store is available! set session_mgr to reqeust.state.{self.session_object}"
                     )
 
                     setattr(
                         request.state,
                         self.session_object,
                         SessionIntegration(
                             store=session_store,
                             session_id=session_id,
-                            session_save=lambda: self.session_store.save_store(session_id),
+                            session_save=lambda: self.session_store.save_store(
+                                session_id
+                            ),
                         ),
                     )
 
                     session_store["__cause__"] = "success"
 
             else:
-                self.logger.info(f"Session cookies available but verification failed! err:{err}")
-                cookie = await self.create_new_session_id_and_store(request, cause=f"renew after {err}")
+                self.logger.info(
+                    f"Session cookies available but verification failed! err:{err}"
+                )
+                cookie = await self.create_new_session_id_and_store(
+                    request, cause=f"renew after {err}"
+                )
 
         response = await call_next(request)
 
         if cookie is not None:
             cookie_val = cookie.output(header="").strip()
             self.logger.info("Set response header 'Set-Cookie' to signed cookie value")
             response.headers["Set-Cookie"] = cookie_val
@@ -223,21 +243,27 @@
             cause (str): The cause of creating a new session ID.
 
         Returns:
             SimpleCookie: The signed session cookie.
         """
         session_id = str(uuid.uuid4())
         session_store = self.session_store.create_store(session_id)
-        self.logger.debug(f"[session_id:'{session_id}'(NEW)] New session_id and store for session_id created.")
+        self.logger.debug(
+            f"[session_id:'{session_id}'(NEW)] New session_id and store for session_id created."
+        )
 
         if cause is not None:
             session_store["__cause__"] = cause
 
         fast_session_obj = SessionIntegration(
-            store=session_store, session_id=session_id, session_save=lambda: self.session_store.save_store(session_id)
+            store=session_store,
+            session_id=session_id,
+            session_save=lambda: self.session_store.save_store(session_id),
+        )
+        self.logger.info(
+            f"[session_id:'{session_id}'(NEW)] Set session_mgr to request.state.{self.session_object} "
         )
-        self.logger.info(f"[session_id:'{session_id}'(NEW)] Set session_mgr to request.state.{self.session_object} ")
         setattr(request.state, self.session_object, fast_session_obj)
 
         self.session_store.gc()
 
         return self.create_session_cookie(session_id)
```

### Comparing `authx_extra-1.0.0/authx_extra/addons/expiry.py` & `authx_extra-1.1.0/authx_extra/addons/expiry.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.0.0/authx_extra/addons/keys.py` & `authx_extra-1.1.0/authx_extra/addons/keys.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 
 from authx_extra.extra._cache import HTTPCache
 
 
 class HTTPKeys:
     @staticmethod
     async def generate_key(
-        key: str, config: HTTPCache, obj: Optional[Any] = None, obj_attr: Optional[str] = None
+        key: str,
+        config: HTTPCache,
+        obj: Optional[Any] = None,
+        obj_attr: Optional[str] = None,
     ) -> str:
         """Converts a raw key passed by the user to a key with an parameter passed by the user and associates a namespace"""
 
         _key = (
             key.format(
                 getattr(obj, obj_attr),
             )
@@ -18,16 +21,24 @@
             else key
         )
 
         return await HTTPKeys.generate_namespaced_key(key=_key, config=config)
 
     @staticmethod
     async def generate_keys(
-        keys: List[str], config: HTTPCache, obj: Optional[Any] = None, obj_attr: Optional[str] = None
+        keys: List[str],
+        config: HTTPCache,
+        obj: Optional[Any] = None,
+        obj_attr: Optional[str] = None,
     ) -> List[str]:
         """Converts a list of raw keys passed by the user to a list of namespaced keys with an optional parameter if passed"""
-        return [await HTTPKeys.generate_key(key=k, config=config, obj=obj, obj_attr=obj_attr) for k in keys]
+        return [
+            await HTTPKeys.generate_key(
+                key=k, config=config, obj=obj, obj_attr=obj_attr
+            )
+            for k in keys
+        ]
 
     @staticmethod
     async def generate_namespaced_key(key: str, config: HTTPCache) -> str:
         """Adds a namespace to the key"""
         return f"{config.namespace}:{key}".replace(" ", "")
```

### Comparing `authx_extra-1.0.0/authx_extra/extra/_cache.py` & `authx_extra-1.1.0/authx_extra/extra/_cache.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.0.0/scripts/clean.sh` & `authx_extra-1.1.0/scripts/clean.sh`

 * *Files identical despite different names*

### Comparing `authx_extra-1.0.0/scripts/docker.sh` & `authx_extra-1.1.0/scripts/docker.sh`

 * *Files identical despite different names*

### Comparing `authx_extra-1.0.0/tests/test_cache.py` & `authx_extra-1.1.0/tests/test_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,48 +27,60 @@
 async def home(request: Request, response: Response):
     return JSONResponse({"page": "home", "datetime": str(datetime.utcnow())})
 
 
 @app.get("/b/logged-in")
 @cache(key="b.logged_in.{}", obj="user", obj_attr="id")
 async def logged_in(request: Request, response: Response, user=user):
-    return JSONResponse({"page": "home", "user": user.id, "datetime": str(datetime.utcnow())})
+    return JSONResponse(
+        {"page": "home", "user": user.id, "datetime": str(datetime.utcnow())}
+    )
 
 
 async def my_ttl_callable():
     return 3600
 
 
 @app.get("/b/ttl_callable")
 @cache(key="b.ttl_callable_expiry", ttl_func=my_ttl_callable)
 async def path_with_ttl_callable(request: Request, response: Response):
-    return JSONResponse({"page": "path_with_ttl_callable", "datetime": str(datetime.utcnow())})
+    return JSONResponse(
+        {"page": "path_with_ttl_callable", "datetime": str(datetime.utcnow())}
+    )
 
 
 @app.post("/b/logged-in")
-@invalidate_cache(key="b.logged_in.{}", obj="user", obj_attr="id", namespace="test_namespace")
+@invalidate_cache(
+    key="b.logged_in.{}", obj="user", obj_attr="id", namespace="test_namespace"
+)
 async def post_logged_in(request: Request, response: Response, user=user):
-    return JSONResponse({"page": "home", "user": user.id, "datetime": str(datetime.utcnow())})
+    return JSONResponse(
+        {"page": "home", "user": user.id, "datetime": str(datetime.utcnow())}
+    )
 
 
 @app.get("/b/profile")
 @cache(key="b.profile.{}", obj="user", obj_attr="id")
 async def logged_in(request: Request, response: Response, user=user):
-    return JSONResponse({"page": "profile", "user": user.id, "datetime": str(datetime.utcnow())})
+    return JSONResponse(
+        {"page": "profile", "user": user.id, "datetime": str(datetime.utcnow())}
+    )
 
 
 @app.post("/b/invalidate_multiple")
 @invalidate_cache(
     keys=["b.logged_in.{}", "b.profile.{}"],
     obj="user",
     obj_attr="id",
     namespace="test_namespace",
 )
 async def invalidate_multiple(request: Request, response: Response, user=user):
-    return JSONResponse({"page": "invalidate_multiple", "datetime": str(datetime.utcnow())})
+    return JSONResponse(
+        {"page": "invalidate_multiple", "datetime": str(datetime.utcnow())}
+    )
 
 
 def test_invalidate_multiple():
     client = TestClient(app)
     redis_client.flushdb()
     response = extracted_result(client, "/b/logged-in")
     response2 = extracted_result(client, "/b/profile")
@@ -142,15 +154,20 @@
         "/b/ttl_callable",
         headers={
             "Content-Type": "application/json",
             "X-Product-Id": "0fb6a4d4-ae65-4f18-be44-edb9ace6b5bb",
         },
     )
     assert response.headers["Cache-hit"] == "true"
-    assert pytest.approx(redis_client.ttl("test_namespace:b.ttl_callable_expiry"), rel=1e-3) == 3600
+    assert (
+        pytest.approx(
+            redis_client.ttl("test_namespace:b.ttl_callable_expiry"), rel=1e-3
+        )
+        == 3600
+    )
 
 
 def test_home_cached_with_current_user():
     client = TestClient(app)
     redis_client.flushdb()
 
     response = client.get(
```

### Comparing `authx_extra-1.0.0/tests/test_keys.py` & `authx_extra-1.1.0/tests/test_keys.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,17 @@
         class User:
             id: str = "112358"
 
         user = User()
 
         namespace = "test_namespace"
         HTTPCache.init(redis_url=REDIS_URL, namespace=namespace)
-        namespaced_key = await HTTPKeys.generate_key(key="hello.{}", config=HTTPCache, obj=user, obj_attr="id")
+        namespaced_key = await HTTPKeys.generate_key(
+            key="hello.{}", config=HTTPCache, obj=user, obj_attr="id"
+        )
         assert namespaced_key == f"{namespace}:hello.112358"
 
     @pytest.mark.asyncio
     async def test_generate_keys_with_attr(self):
         redis_client.flushdb()
 
         class User:
```

### Comparing `authx_extra-1.0.0/tests/test_method_cache.py` & `authx_extra-1.1.0/tests/test_method_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,8 +48,13 @@
 
     @pytest.mark.asyncio
     async def test_ttl_callable(self):
         redis_client.flushdb()
         HTTPCache.init(redis_url=REDIS_URL, namespace="test_namespace")
         await cache_me_with_ttl_callable(x=22, invoke_count=0)
         await cache_me_with_ttl_callable(x=22, invoke_count=0)
-        assert pytest.approx(redis_client.ttl("test_namespace:cache.me.ttl_callable"), rel=1e-3) == 3600
+        assert (
+            pytest.approx(
+                redis_client.ttl("test_namespace:cache.me.ttl_callable"), rel=1e-3
+            )
+            == 3600
+        )
```

### Comparing `authx_extra-1.0.0/tests/test_metrics.py` & `authx_extra-1.1.0/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.0.0/tests/test_oauth2.py` & `authx_extra-1.1.0/tests/test_oauth2.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,17 @@
         app, key, audience, issuer = case_1()
 
         client = TestClient(app)
         token = jose.jwt.encode(good_claims(audience, issuer), key)
 
         with self.assertLogs("authx_extra.oauth2", level="DEBUG") as cm:
             response = client.get("/", headers={"authorization": f"Bearer {token}"})
-            self.assertEqual(cm.output, [log_message1, "DEBUG:authx_extra.oauth2:Token decoded."])
+            self.assertEqual(
+                cm.output, [log_message1, "DEBUG:authx_extra.oauth2:Token decoded."]
+            )
 
         self.assertEqual(response.status_code, 404)
 
     def test_keys_as_dict(self):
         key = "not-secret"
         keys = {"keys": [key]}
         app, audience, issuer = case_2(keys)
@@ -210,15 +212,17 @@
         self.assertEqual(storage["scope"]["oauth2-provider"], "custom")
 
     def test_ignore_at_hash(self):
         """Explicitly test that we ignore the ``at_hash`` of the jwt."""
         app, key, audience, issuer = case_1()
 
         client = TestClient(app)
-        token = jose.jwt.encode(good_claims(audience, issuer), key, access_token="test_access_token")
+        token = jose.jwt.encode(
+            good_claims(audience, issuer), key, access_token="test_access_token"
+        )
         response = client.get("/", headers={"authorization": f"Bearer {token}"})
 
         self.assertEqual(response.status_code, 404)
 
     def test_wrong_key(self):
         app, _, audience, issuer = case_1()
 
@@ -227,15 +231,17 @@
         with self.assertLogs("authx_extra.oauth2", level="DEBUG") as cm:
             response = client.get("/", headers={"authorization": f"Bearer {token}"})
             self.assertEqual(len(cm.output), 2)
             self.assertEqual(cm.output[0], log_message1)
             self.assertTrue("Signature verification failed" in cm.output[1])
 
         self.assertEqual(response.status_code, 401)
-        self.assertEqual(response.json(), {"message": {"custom": "Signature verification failed."}})
+        self.assertEqual(
+            response.json(), {"message": {"custom": "Signature verification failed."}}
+        )
 
     def test_expired(self):
         app, key, audience, issuer = case_1()
 
         client = TestClient(app)
         token = jose.jwt.encode(
             {
@@ -320,15 +326,17 @@
         with self.assertLogs("authx_extra.oauth2", level="DEBUG") as cm:
             response = client.get("/", headers={"authorization": f"Bearer {token}"})
             self.assertEqual(len(cm.output), 2)
             self.assertEqual(cm.output[0], log_message1)
             self.assertTrue("Signature verification failed" in cm.output[1])
 
         self.assertEqual(response.status_code, 401)
-        self.assertEqual(response.json(), {"message": {"custom": "Signature verification failed."}})
+        self.assertEqual(
+            response.json(), {"message": {"custom": "Signature verification failed."}}
+        )
 
     def test_public_path(self):
         app, key, audience, issuer = case_1(public_paths={"/"})
 
         client = TestClient(app)
         response = client.get("/")
 
@@ -394,15 +402,17 @@
         response = client.get("/", headers={"authorization": f"Bearer {token}"})
         response = client.get("/", headers={"authorization": f"Bearer {token}"})
 
         self.assertEqual(response.status_code, 404)
         self.assertEqual(len(calls_get_keys), 1)
 
     def test_key_refresh_dict(self):
-        app, key, audience, issuer, calls_get_keys = case_3(key_refresh_minutes={"custom": 0})
+        app, key, audience, issuer, calls_get_keys = case_3(
+            key_refresh_minutes={"custom": 0}
+        )
 
         client = TestClient(app)
         token = jose.jwt.encode(good_claims(audience, issuer), key)
         response = client.get("/", headers={"authorization": f"Bearer {token}"})
         response = client.get("/", headers={"authorization": f"Bearer {token}"})
 
         self.assertEqual(response.status_code, 404)
@@ -416,15 +426,17 @@
             await websocket.accept()
             await websocket.send_text("Hello, world!")
             await websocket.close()
 
         client = TestClient(app)
         token = jose.jwt.encode(good_claims(audience, issuer), key)
 
-        with client.websocket_connect("/ws", headers={"authorization": f"Bearer {token}"}) as websocket:
+        with client.websocket_connect(
+            "/ws", headers={"authorization": f"Bearer {token}"}
+        ) as websocket:
             data = websocket.receive_text()
             self.assertEqual(data, "Hello, world!")
 
     def test_websocket_not_ok(self):
         app, key, audience, issuer = case_1()
 
         @app.websocket_route("/ws")
@@ -434,9 +446,11 @@
             await websocket.close()
 
         client = TestClient(app)
         invalid_key = f"{key}a"
         token = jose.jwt.encode(good_claims(audience, issuer), invalid_key)
 
         with self.assertRaises(WebSocketDisconnect):
-            with client.websocket_connect("/ws", headers={"authorization": f"Bearer {token}"}):
+            with client.websocket_connect(
+                "/ws", headers={"authorization": f"Bearer {token}"}
+            ):
                 pass
```

### Comparing `authx_extra-1.0.0/tests/test_profiler.py` & `authx_extra-1.1.0/tests/test_profiler.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.0.0/tests/test_session_middleware.py` & `authx_extra-1.1.0/tests/test_session_middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,15 +218,17 @@
     assert "HttpOnly" not in response.headers["Set-Cookie"]
 
 
 @pytest.mark.asyncio
 async def test_dispatch_should_skip_session_management_with_skip_header():
     app = Mock(return_value=Response("OK"))
     middleware = SessionMiddleware(
-        app=app, secret_key="test", skip_session_header={"header_name": "X-ApiTest-Skip", "header_value": "skip"}
+        app=app,
+        secret_key="test",
+        skip_session_header={"header_name": "X-ApiTest-Skip", "header_value": "skip"},
     )
 
     headers = [(b"x-apitest-skip", b"skip")]
     request = Request(scope={"type": "http", "headers": headers}, receive=None)
 
     class MockResponse:
         def __init__(self):
@@ -242,15 +244,20 @@
     assert not hasattr(request.state, "session")
 
 
 @pytest.mark.asyncio
 async def test_dispatch_should_not_skip_session_management_without_skip_heade1r():
     app = Mock(return_value=Response("OK"))
     middleware = SessionMiddleware(
-        app=app, secret_key="test", skip_session_header={"header_name": "X-FastSession-Skip", "header_value": "skip"}
+        app=app,
+        secret_key="test",
+        skip_session_header={
+            "header_name": "X-FastSession-Skip",
+            "header_value": "skip",
+        },
     )
 
     headers = [(b"ignore", b"ignore")]
     request = Request(scope={"type": "http", "headers": headers}, receive=None)
 
     class MockResponse:
         def __init__(self):
```

### Comparing `authx_extra-1.0.0/tests/test_skip_session_header_check_dict.py` & `authx_extra-1.1.0/tests/test_skip_session_header_check_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 from authx_extra.session import SessionMiddleware
 
 
 @pytest.fixture
 def middleware():
     return SessionMiddleware(
-        app=None, secret_key="test", skip_session_header={"header_name": "X-TESTAPI-Skip", "header_value": "skip"}
+        app=None,
+        secret_key="test",
+        skip_session_header={"header_name": "X-TESTAPI-Skip", "header_value": "skip"},
     )
 
 
 def test_skip_session_header_check_dict_with_skip_header(middleware):
     request = Mock()
     request.headers = {"X-TESTAPI-Skip": "skip"}
 
@@ -22,12 +24,14 @@
 def test_skip_session_header_check_dict_without_skip_header(middleware):
     request = Mock()
     request.headers = {"X-Other-Header": "value"}
 
     assert middleware.skip_session_header_check(request) is False
 
 
-def test_skip_session_header_check_dict_with_skip_header_and_different_value(middleware):
+def test_skip_session_header_check_dict_with_skip_header_and_different_value(
+    middleware,
+):
     request = Mock()
     request.headers = {"X-TESTAPI-Skip": "other"}
 
     assert middleware.skip_session_header_check(request) is False
```

### Comparing `authx_extra-1.0.0/tests/test_skip_session_header_check_list.py` & `authx_extra-1.1.0/tests/test_skip_session_header_check_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,17 @@
 
 def request1(argument, middleware):
     request = Mock()
     request.headers = {argument: "skip"}
     assert middleware.skip_session_header_check(request) is True
 
 
-def test_skip_session_header_check_list_with_multiple_headers_and_different_values(middleware):
+def test_skip_session_header_check_list_with_multiple_headers_and_different_values(
+    middleware,
+):
     request2("X-APITEST-Skip", middleware)
     request2("X-Another-Skip-Header", middleware)
 
 
 def request2(argument, middleware):
     request = Mock()
     request.headers = {argument: "other"}
```

### Comparing `authx_extra-1.0.0/.gitignore` & `authx_extra-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `authx_extra-1.0.0/LICENSE` & `authx_extra-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `authx_extra-1.0.0/README.md` & `authx_extra-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `authx_extra-1.0.0/pyproject.toml` & `authx_extra-1.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     "Topic :: Internet :: WWW/HTTP :: Session",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Internet",
     "Typing :: Typed",
 ]
 
 dependencies = [
-    "authx==1.0.0b0",
+    "authx==1.0.0",
 ]
 
 dynamic = ["version"]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
@@ -58,82 +58,60 @@
 Documentation = "https://authx.yezz.me/installation/#extra-dependencies"
 Funding = 'https://github.com/sponsors/yezz123'
 
 [project.optional-dependencies]
 profiler = [
     "pyinstrument>=4.1.1,<4.7.0",
 ]
-oauth2 = [
-    "python-jose>=3.3.0,<4.0.0",
-]
 metrics = [
     "prometheus-client>=0.16.0,<1.0.0",
 ]
 cache = [
-    "python-dateutil>=2.8,<3.0.0",
-    "redis>=4.3.3,<5.0.2",
-    "pytz>=2023.3,<2024.0",
-]
-lint = [
-    "pre-commit==3.6.0",
-    "mypy==1.8.0",
-]
-test = [
-    "pytest",
-    "pytest-asyncio",
-    "pytest-cov",
-    "httpx",
-    "requests",
-    "SQLAlchemy",
-    "itsdangerous",
-    "websockets",
-    "uvicorn",
-    "uvloop",
-    "freezegun"
+    "redis>=4.3.3,<5.0.4",
 ]
 
 [tool.hatch.version]
 path = "authx_extra/__init__.py"
 
 
-[tool.ruff]
-line-length = 120
+[tool.ruff.lint]
 mccabe = { max-complexity = 14 }
 select = [
     "E",  # pycodestyle errors
     "W",  # pycodestyle warnings
     "F",  # pyflakes
     "I",  # isort
     "C",  # flake8-comprehensions
     "B",  # flake8-bugbear
 ]
 ignore = [
     "E501"  # line too long, handled by black
 ]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
 "tests/test_cache.py" = ["F841", "F811"]
 "session.py" = ["B008"]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-third-party = ["pydantic", "typing_extensions", "sqlalchemy"]
 
-[tool.ruff.pyupgrade]
+[tool.ruff.lint.pyupgrade]
 keep-runtime-typing = true
 
 [tool.coverage.run]
 source = ["authx_extra", "tests"]
 branch = true
 context = '${CONTEXT}'
 
 [tool.coverage.paths]
 source = [
-    "authx_extra/",
-    "tests/",
+    'authx_extra/',
+    '/Users/runner/work/authx_extra/authx_extra/authx_extra/',
+    'D:\a\authx_extra\authx_extra\authx_extra',
 ]
 
 [tool.coverage.report]
 precision = 2
 exclude_lines = [
     'pragma: no cover',
     'raise NotImplementedError',
```

