# Comparing `tmp/fuzzbucket_client-0.8.1-py3-none-any.whl.zip` & `tmp/fuzzbucket_client-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 13041 bytes, number of entries: 10
--rw-r--r--  2.0 unx        0 b- defN 21-Sep-08 17:38 fuzzbucket_client/__init__.py
--rw-r--r--  2.0 unx    35828 b- defN 21-Sep-08 17:38 fuzzbucket_client/__main__.py
--rw-r--r--  2.0 unx      142 b- defN 21-Sep-08 17:40 fuzzbucket_client/__version__.py
--rw-r--r--  2.0 unx     1069 b- defN 21-Sep-08 17:40 fuzzbucket_client-0.8.1.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     5158 b- defN 21-Sep-08 17:40 fuzzbucket_client-0.8.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Sep-08 17:40 fuzzbucket_client-0.8.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       71 b- defN 21-Sep-08 17:40 fuzzbucket_client-0.8.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       18 b- defN 21-Sep-08 17:40 fuzzbucket_client-0.8.1.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 21-Sep-08 17:40 fuzzbucket_client-0.8.1.dist-info/zip-safe
-?rw-rw-r--  2.0 unx      898 b- defN 21-Sep-08 17:40 fuzzbucket_client-0.8.1.dist-info/RECORD
-10 files, 43277 bytes uncompressed, 11471 bytes compressed:  73.5%
+Zip file size: 13066 bytes, number of entries: 10
+-rw-r--r--  2.0 unx        0 b- defN 21-Sep-09 13:09 fuzzbucket_client/__init__.py
+-rw-r--r--  2.0 unx    36000 b- defN 21-Sep-09 13:09 fuzzbucket_client/__main__.py
+-rw-r--r--  2.0 unx      142 b- defN 21-Sep-09 13:11 fuzzbucket_client/__version__.py
+-rw-r--r--  2.0 unx     1069 b- defN 21-Sep-09 13:11 fuzzbucket_client-0.9.0.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     5225 b- defN 21-Sep-09 13:11 fuzzbucket_client-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-Sep-09 13:11 fuzzbucket_client-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       71 b- defN 21-Sep-09 13:11 fuzzbucket_client-0.9.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       18 b- defN 21-Sep-09 13:11 fuzzbucket_client-0.9.0.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 21-Sep-09 13:11 fuzzbucket_client-0.9.0.dist-info/zip-safe
+?rw-rw-r--  2.0 unx      898 b- defN 21-Sep-09 13:11 fuzzbucket_client-0.9.0.dist-info/RECORD
+10 files, 43516 bytes uncompressed, 11496 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -3,29 +3,29 @@
 
 Filename: fuzzbucket_client/__main__.py
 Comment: 
 
 Filename: fuzzbucket_client/__version__.py
 Comment: 
 
-Filename: fuzzbucket_client-0.8.1.dist-info/LICENSE.md
+Filename: fuzzbucket_client-0.9.0.dist-info/LICENSE.md
 Comment: 
 
-Filename: fuzzbucket_client-0.8.1.dist-info/METADATA
+Filename: fuzzbucket_client-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: fuzzbucket_client-0.8.1.dist-info/WHEEL
+Filename: fuzzbucket_client-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: fuzzbucket_client-0.8.1.dist-info/entry_points.txt
+Filename: fuzzbucket_client-0.9.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: fuzzbucket_client-0.8.1.dist-info/top_level.txt
+Filename: fuzzbucket_client-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fuzzbucket_client-0.8.1.dist-info/zip-safe
+Filename: fuzzbucket_client-0.9.0.dist-info/zip-safe
 Comment: 
 
-Filename: fuzzbucket_client-0.8.1.dist-info/RECORD
+Filename: fuzzbucket_client-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fuzzbucket_client/__main__.py

```diff
@@ -84,14 +84,20 @@
         default=log_level() == logging.DEBUG,
         help="enable debug logging",
     )
     subparsers = parser.add_subparsers(title="commands")
 
     parser_login = subparsers.add_parser("login", help="login via GitHub")
     parser_login.add_argument("user", help="GitHub username")
+    parser_login.add_argument(
+        "-n",
+        "--name",
+        default=None,
+        help="human-friendly name to give to credentials entry",
+    )
     parser_login.set_defaults(func=client.login)
     parser_login.epilog = textwrap.dedent(
         """
         NOTE: Use the exact letter casing expected by GitHub to
         avoid weirdness.
         """
     )
@@ -473,15 +479,15 @@
                 raw_secret = getpass.getpass("secret: ").strip()
                 if len(raw_secret) != 42:
                     print("Invalid secret provided. Please try again.")
                     continue
                 secret = raw_secret
             except KeyboardInterrupt:
                 return False
-        self._write_credentials(known_args.user, secret)
+        self._write_credentials(known_args.user, secret, name=known_args.name)
         print(f"Login successful user={known_args.user!r}")
         return True
 
     @_command
     def logout(self, *_):
         log.debug(f"starting logout for user={self._user!r}")
         req = self._build_request(_pjoin(self._url, "_logout"), method="POST")
@@ -539,19 +545,18 @@
         if known_args.name != "":
             payload["name"] = known_args.name
         if known_args.instance_tags:
             payload["instance_tags"] = {}
             for pair in known_args.instance_tags.split(","):
                 if ":" not in pair:
                     continue
-                parts = pair.strip().split(":", maxsplit=1)
-                if len(parts) != 2:
-                    log.warn(f"ignoring unexpected key-value pair {pair!r}")
-                    continue
-                key, value = [urllib.parse.unquote(str(s.strip())) for s in parts]
+                key, value = [
+                    urllib.parse.unquote(str(s.strip()))
+                    for s in pair.strip().split(":", maxsplit=1)
+                ]
                 log.debug(f"adding instance tag to request key={key!r} value={value!r}")
                 payload["instance_tags"][key] = value
         req = self._build_request(
             _pjoin(self._url, "box"),
             data=json.dumps(payload).encode("utf-8"),
             headers={"Content-Type": "application/json"},
             method="POST",
@@ -896,28 +901,30 @@
         with self._credentials_file.open() as infile:
             creds = configparser.ConfigParser()
             creds.read_file(infile)
             if self._credentials_section not in creds.sections():
                 return ""
             return creds.get(self._credentials_section, "credentials")
 
-    def _write_credentials(self, user, secret):
+    def _write_credentials(self, user, secret, name=None):
         if self._env.get("FUZZBUCKET_CREDENTIALS") is not None:
             log.debug(
                 "skipping writing credentials due to presence of FUZZBUCKET_CREDENTIALS"
             )
             return
 
         creds = configparser.ConfigParser()
         if self._credentials_file.exists():
             with self._credentials_file.open() as infile:
                 creds.read_file(infile)
         if self._credentials_section not in creds.sections():
             creds.add_section(self._credentials_section)
         creds.set(self._credentials_section, "credentials", f"{user}:{secret}")
+        if name is not None:
+            creds.set(self._credentials_section, "name", str(name))
         with self._credentials_file.open("w") as outfile:
             outfile.write(
                 "# WARNING: this file is generated "
                 + f"(last update {datetime.datetime.utcnow()})\n"
             )
             creds.write(outfile)
         self._cached_credentials = None
```

## fuzzbucket_client/__version__.py

```diff
@@ -1,5 +1,5 @@
 # coding: utf-8
 # file generated by setuptools_scm
 # don't change, don't track in version control
-version = '0.8.1'
-version_tuple = (0, 8, 1)
+version = '0.9.0'
+version_tuple = (0, 9, 0)
```

## Comparing `fuzzbucket_client-0.8.1.dist-info/LICENSE.md` & `fuzzbucket_client-0.9.0.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `fuzzbucket_client-0.8.1.dist-info/METADATA` & `fuzzbucket_client-0.9.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzbucket-client
-Version: 0.8.1
+Version: 0.9.0
 Summary: Command line client for fuzzbucket
 Home-page: https://github.com/rstudio/fuzzbucket
 Author: RStudio Connect Engineers
 Author-email: rsc-dev+fuzzbucket@rstudio.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: <4,>3.5
@@ -73,35 +73,36 @@
 as by including it in your shell configuration (`~/.bashrc`, `~/.zshrc`) or
 by using a tool like [autoenv](https://github.com/inishchith/autoenv).
 
 ## development
 
 Prerequisites for development are:
 
--    `make`
+-    `just`
 -    `yarn`
 -    `pipenv`
 
-Hopefully `make` is already available :grimacing:. The `yarn` tool
-may be installed via `brew` on macOS and [other ways,
-too](https://yarnpkg.com/getting-started/install). The `pipenv`
-tool may be installed via `pip`.
+The `just` tool may be installed via `brew` on macOS and [other
+ways, too](https://github.com/casey/just#installation). Similarly,
+the `yarn` tool may be installed via `brew` on macOS and [other
+ways, too](https://yarnpkg.com/getting-started/install). The
+`pipenv` tool may be installed via `pip`.
 
 Once these prerequisites are available, the default workflow is nearly
 identical to what is captured in the [github
 workflow](./.github/workflows/main.yml):
 
 ```bash
-make deps
+just deps
 
 # BEGIN editing, linting, testing loop {
 
 # edit edit edit
-make lint
-make test
+just lint
+just test
 
 # } END editing, linting, testing loop
 ```
 
 ## deployment
 
 Deploying the `fuzzbucket` API requires AWS credentials with rights to
@@ -148,25 +149,25 @@
 
 ```bash
 export FUZZBUCKET_CUSTOM_prod='custom-path.yml'
 ```
 
 ### cycle
 
-The `make deploy` target will run the necessary `serverless` command to create
+The `just deploy` target will run the necessary `serverless` command to create
 the whole shebang.
 
 ```bash
 # deploy to STAGE=dev in REGION=us-east-1
-make deploy
+just deploy
 ```
 
 ```bash
 # deploy to STAGE=prod in REGION=us-west-2
-make deploy STAGE=prod REGION=us-west-2
+just deploy prod us-west-2
 ```
 
 These commands are expected to be re-run as needed, such as after modifying the
 custom YAML described in the prerequisites section above.
 
 
 ## changelog
```

