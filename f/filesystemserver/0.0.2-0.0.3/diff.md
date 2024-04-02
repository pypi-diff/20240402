# Comparing `tmp/filesystemserver-0.0.2-py3-none-any.whl.zip` & `tmp/filesystemserver-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,14 @@
-Zip file size: 8619 bytes, number of entries: 10
+Zip file size: 11936 bytes, number of entries: 12
 -rw-r--r--  2.0 unx       82 b- defN 20-Feb-02 00:00 filesystemserver/__init__.py
--rw-r--r--  2.0 unx    10465 b- defN 20-Feb-02 00:00 filesystemserver/filesystemserver.py
--rw-r--r--  2.0 unx     1077 b- defN 20-Feb-02 00:00 filesystemserver/data/plugin/fss/fss.js
--rw-r--r--  2.0 unx     1736 b- defN 20-Feb-02 00:00 filesystemserver/data/plugin/fss/browser/app.js
--rw-r--r--  2.0 unx      814 b- defN 20-Feb-02 00:00 filesystemserver/data/plugin/fss/browser/index.html
-?rw-r--r--  2.0 unx     2318 b- defN 20-Feb-02 00:00 filesystemserver-0.0.2.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 filesystemserver-0.0.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx       46 b- defN 20-Feb-02 00:00 filesystemserver-0.0.2.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1058 b- defN 20-Feb-02 00:00 filesystemserver-0.0.2.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      927 b- defN 20-Feb-02 00:00 filesystemserver-0.0.2.dist-info/RECORD
-10 files, 18610 bytes uncompressed, 7003 bytes compressed:  62.4%
+-rw-r--r--  2.0 unx    11327 b- defN 20-Feb-02 00:00 filesystemserver/filesystemserver.py
+-rw-r--r--  2.0 unx     2941 b- defN 20-Feb-02 00:00 filesystemserver/data/plugin/fss/favicon.png
+-rw-r--r--  2.0 unx     1542 b- defN 20-Feb-02 00:00 filesystemserver/data/plugin/fss/fss.js
+-rw-r--r--  2.0 unx     1811 b- defN 20-Feb-02 00:00 filesystemserver/data/plugin/fss/browser/app.js
+-rw-r--r--  2.0 unx      353 b- defN 20-Feb-02 00:00 filesystemserver/data/plugin/fss/browser/index.html
+-rw-r--r--  2.0 unx      472 b- defN 20-Feb-02 00:00 filesystemserver/data/plugin/fss/browser/style.css
+?rw-r--r--  2.0 unx     2757 b- defN 20-Feb-02 00:00 filesystemserver-0.0.3.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 filesystemserver-0.0.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx       46 b- defN 20-Feb-02 00:00 filesystemserver-0.0.3.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1058 b- defN 20-Feb-02 00:00 filesystemserver-0.0.3.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1134 b- defN 20-Feb-02 00:00 filesystemserver-0.0.3.dist-info/RECORD
+12 files, 23610 bytes uncompressed, 9980 bytes compressed:  57.7%
```

## zipnote {}

```diff
@@ -1,31 +1,37 @@
 Filename: filesystemserver/__init__.py
 Comment: 
 
 Filename: filesystemserver/filesystemserver.py
 Comment: 
 
+Filename: filesystemserver/data/plugin/fss/favicon.png
+Comment: 
+
 Filename: filesystemserver/data/plugin/fss/fss.js
 Comment: 
 
 Filename: filesystemserver/data/plugin/fss/browser/app.js
 Comment: 
 
 Filename: filesystemserver/data/plugin/fss/browser/index.html
 Comment: 
 
-Filename: filesystemserver-0.0.2.dist-info/METADATA
+Filename: filesystemserver/data/plugin/fss/browser/style.css
+Comment: 
+
+Filename: filesystemserver-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: filesystemserver-0.0.2.dist-info/WHEEL
+Filename: filesystemserver-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: filesystemserver-0.0.2.dist-info/entry_points.txt
+Filename: filesystemserver-0.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: filesystemserver-0.0.2.dist-info/licenses/LICENSE
+Filename: filesystemserver-0.0.3.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: filesystemserver-0.0.2.dist-info/RECORD
+Filename: filesystemserver-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filesystemserver/__init__.py

```diff
@@ -1,3 +1,3 @@
 from .filesystemserver import install, update, serve, main
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
```

## filesystemserver/filesystemserver.py

```diff
@@ -27,20 +27,25 @@
     return url, plugin_dir
 
 
 def installed_plugins(plugin_dir):
     index = "index.html"
     prefix_len = len(plugin_dir) + 1
     postfix_len = len(index) + 1
-    return sorted(
-        [
-            m[prefix_len:-postfix_len]
-            for m in glob.glob(f"{plugin_dir}/**/{index}", recursive=True)
-        ]
-    )
+    plugins = []
+    for m in glob.glob(f"{plugin_dir}/**/{index}", recursive=True):
+        directory = m[prefix_len:-postfix_len]
+        plugin = {"name": directory}
+        config_path = os.path.join(plugin_dir, directory, "fss.toml")
+        if os.path.exists(config_path):
+            with open(config_path, "rb") as fd:
+                plugin.update(toml.load(fd))
+        plugin["directory"] = directory
+        plugins.append(plugin)
+    return sorted(plugins, key=lambda m: m["name"])
 
 
 def git(*args, cwd=None, help_message=""):
     assert cwd is not None
     try:
         subprocess.run(["git", "-C", cwd, *args], check=True)
     except FileNotFoundError:
@@ -67,15 +72,15 @@
 
 
 def update(args):
     plugins = (
         args.plugins if len(args.plugins) > 0 else installed_plugins(args.plugin_dir)
     )
     for plugin in plugins:
-        repo, plugin_dir = resolve_git_repo(plugin)
+        repo, plugin_dir = resolve_git_repo(plugin["directory"])
         git(
             "pull",
             cwd=os.path.join(args.plugin_dir, plugin_dir),
             help_message="Perhaps the plugin isn't already installed, did you mean to run `install`?",
         )
         print("Succesfully updated:", plugin_dir)
 
@@ -108,14 +113,19 @@
             return self.send_file(f, fsize, "application/json")
 
         def send_file_at_path(self, path, revalidate=False):
             if not os.path.exists(path):
                 return self.send_error(
                     http.server.HTTPStatus.NOT_FOUND, f"File not found {path}"
                 )
+            if os.path.isdir(path):
+                return self.send_error(
+                    http.server.HTTPStatus.BAD_REQUEST,
+                    f"File attempting to open is directory {path}",
+                )
             ctype, encoding = mimetypes.guess_type(path)
             if ctype is None:
                 ctype = "application/octet-stream"
             f = open(path, "rb")
             fs = os.fstat(f.fileno())
             return self.send_file(
                 f,
@@ -201,15 +211,17 @@
             if req.query:
                 f = self.query_handler(req.query)
                 if f is not None:
                     return f
 
             if plugin_path == "/":
                 PluginRequestHandler.cwd = "/"
-                return self.redirect("fss/browser/")
+                return self.redirect(args.default_plugin + "/")
+            elif not req.query:
+                return self.redirect(plugin_path + f"?cwd={PluginRequestHandler.cwd}")
             else:
                 return self.plugin_handler(plugin_path)
 
         def do_GET(self):
             f = self.do_HEAD()
             if f:
                 try:
@@ -231,15 +243,15 @@
     return get_default_fss_subpath("config.toml")
 
 
 def get_default_config():
     return {
         "address": "localhost",
         "port": 8080,
-        "default_plugin": None,
+        "default_plugin": "fss/browser",
     }
 
 
 def load_config(config_path, create=False):
     config = get_default_config()
     if os.path.exists(config_path):
         with open(config_path, "rb") as fd:
@@ -325,14 +337,19 @@
     )
     serve_parser.add_argument(
         "-d",
         "--directory",
         default=".",
         help="Root directory to serve",
     )
+    serve_parser.add_argument(
+        "--default-plugin",
+        default=None,
+        help="Default plugin to launch with, default (fss/browser)",
+    )
 
     args = setup_defaults_and_environment(parser.parse_args())
     exit_code = args.func(args)
     if exit_code is not None:
         sys.exit(exit_code)
```

## filesystemserver/data/plugin/fss/fss.js

### js-beautify {}

```diff
@@ -1,41 +1,57 @@
-class ServerError extends Error {
-    constructor(message) {
-        super(message);
-        this.name = "ServerError";
+export let fss = (() => {
+    class FSSError extends Error {
+        constructor(message) {
+            super(message);
+            this.name = "FSSError";
+        }
     }
-}
 
-const fetch_json = (url) => fetch(url).then(response => {
-    if (response.ok) return response.json();
-    throw new ServerError(response.statusText);
-});
-
-const fetch_text = (url) => fetch(url).then(response => {
-    if (response.ok) return response.text();
-    throw new ServerError(response.statusText);
-});
-
-const error_handler = (error) => {
-    console.log(error);
-    document.body.innerHTML =
-        `<div style="font-family: ui-monospace, courier new, monospace">
-      <h1>${error}</h1>
-      <blockquote><pre>${error.stack}</pre></blockquote>
-    </div>`;
-};
-
-const fss = {
-    query: (callback, queries = ["cwd", "list", "plugins"]) => {
-        query = queries.map(q => `query=${q}`).join("&");
-        fetch_json(`?${query}`)
+    const response_as_json = (r) => r.json();
+    const response_as_text = (r) => r.text();
+
+    const fetch_as = (url, as_fn) => fetch(url).then(response => {
+        if (response.ok) return as_fn(response);
+        throw new FSSError(response.statusText);
+    });
+    const fetch_json = (url) => fetch_as(url, response_as_json);
+    const fetch_text = (url) => fetch_as(url, response_as_text);
+
+    const error_handler = (error) => {
+        console.log(error);
+        document.body.innerHTML =
+            `<div style="font-family: ui-monospace, courier new, monospace">
+        <h1>${error}</h1>
+        <blockquote><pre>${error.stack}</pre></blockquote>
+      </div>`;
+    };
+
+    const query = (callback, queries = ["cwd", "list", "plugins"]) => {
+        const query_str = queries.map(q => `query=${q}`).join("&");
+        fetch_json(`?${query_str}`)
             .then(callback)
             .catch(error_handler);
-    },
+    };
 
-    download: (url, callback) => {
-        const fetch_fn = url.endsWith(".json") ? fetch_json : fetch_text;
-        fetch_fn(`?download=${url}`)
+    const download = (url, callback, as_fn = undefined) => {
+        if (as_fn === undefined) {
+            as_fn = url.endsWith(".json") ? response_as_json : response_as_text;
+        }
+        fetch_as(`?download=${url}`, as_fn)
             .then(callback)
             .catch(error_handler);
-    },
-}
+    };
+
+    const with_data = (callback, as_fn = undefined) => {
+        query(q => {
+            download(q["list"].root, callback, as_fn);
+        }, queries = ["list"]);
+    };
+
+    return {
+        query: query,
+        download: download,
+        with_data: with_data,
+    };
+})();
+
+export default fss;
```

## filesystemserver/data/plugin/fss/browser/app.js

### js-beautify {}

```diff
@@ -1,7 +1,11 @@
+import fss from "/fss/fss.js";
+
+fss.query(app_main);
+
 function app_main(data) {
     console.log(data);
     const dirlist = data["list"];
     const plugins = data["plugins"];
     const container = document.getElementById("container");
     const root = (dirlist.root == "/") ? dirlist.root : dirlist.root + "/";
     const [_, h1] = dirlist.root.split("/").reduce((a, c) => {
@@ -17,15 +21,15 @@
 
     const plugin_container = document.getElementById("plugin_container");
     const collection = container.getElementsByClassName("nav");
     for (let e of collection) {
         e.addEventListener("mouseover", (i) => {
             const rect = i.target.getBoundingClientRect();
             const plugin_list = plugins.length > 0 ?
-                plugins.map(p => `<li><a href="/${p}?cwd=${root}${i.target.id === "" ? "" : dirlist.paths.at(i.target.id)}">${p}</a></li>`).join("") :
+                plugins.map(p => `<li><a href="/${p["directory"]}?cwd=${root}${i.target.id === "" ? "" : dirlist.paths.at(i.target.id)}">${p["name"]}</a></li>`).join("") :
                 "<em>No plugins installed</em>";
             plugin_container.style.display = "block";
             plugin_container.style.left = rect.right + "px";
             plugin_container.style.top = (rect.top - 5) + "px";
             plugin_container.innerHTML = `<ul style="list-style-type: none; padding: 5px; margin: 0px;">${plugin_list}</ul>`;
         });
     }
```

## filesystemserver/data/plugin/fss/browser/index.html

```diff
@@ -1,54 +1,14 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta charset="UTF-8">
-    <title>FSS Browser</title>
-    <style>
-span.nav {
-  -webkit-user-select: none;
-  -ms-user-select: none;
-  user-select: none;
-  cursor: default;
-  color: LightGray;
-}
-
-span.nav:hover { color: black; }
-
-h1 {
-  margin-left: 20px;
-  position: sticky;
-  top: 0;
-  background-color: white;
-}
-
-a {
-  text-decoration: none;
-  color: #1560bd;
-}
-
-a:hover {
-  color: #2c3968;
-}
-
-a:visited {
-  color: #1560bd;
-}
-
-#plugin_container {
-  display: none;
-  position: fixed;
-  list-style-type: none;
-  background-color: white;
-}
-    </style>
-    <script src="/fss/fss.js"></script>
-    <script src="app.js"></script>
-    <script>
-    fss.query(app_main);
-    </script>
+    <title>fss</title>
+    <link rel="icon" type="image/png" sizes="16x16" href="/fss/favicon.png">
+    <link rel="stylesheet" href="style.css">
+    <script src="app.js" type="module"></script>
 </head>
 <body>
 <div id="container"></div>
 <div id="plugin_container"></div>
 </body>
 </html>
```

## Comparing `filesystemserver-0.0.2.dist-info/METADATA` & `filesystemserver-0.0.3.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: filesystemserver
-Version: 0.0.2
+Version: 0.0.3
 Summary: File System Server
 Project-URL: Homepage, https://github.com/nicholashaydensmith/filesystemserver
 Project-URL: Issues, https://github.com/nicholashaydensmith/filesystemserver/issues
 Author-email: Nicholas Smith <thesmithdynasty@gmail.com>
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -54,18 +54,33 @@
 
 # Update all installed plugins
 fss update
 ```
 
 ## `fss` Configuration
 
+`fss` is configured via toml `~/.config/fss/config.toml` and has the following options:
+```toml
+address = "localhost"
+port = 8080
+default_plugin = "fss/browser"
+```
+
 ## Developing a Plugin
 
+The simplest possible plugin is just a git project with an `index.html` file.  Plugins are installed into `~/.config/fss/plugin`.
+
 ### `index.html`
 
+### JavaScript API
+
 ### `fss.toml`
 
+### Examples
+- https://github.com/nicholashaydensmith/gallery.fss
+- https://github.com/nicholashaydensmith/highlight.fss
+
 ## Development
 
 `filesystemserver` itself strives to be as small and simple as possible, leaving all features and extensibility to plugins.
 
 It also strives to have as few dependencies as possible, currently its only dependency requirement is for python pre 3.11 package `tomli`.
```

## Comparing `filesystemserver-0.0.2.dist-info/licenses/LICENSE` & `filesystemserver-0.0.3.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

