# Comparing `tmp/AlpineHtmxWebViewTest-0.1.2-py3-none-any.whl.zip` & `tmp/AlpineHtmxWebViewTest-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7562 bytes, number of entries: 10
--rw-r--r--  2.0 unx     3522 b- defN 24-Mar-17 19:07 BuildBinary.py
--rw-r--r--  2.0 unx     2542 b- defN 24-Mar-17 19:07 AlpineHtmxWebViewTest/EntryPoint.py
--rw-r--r--  2.0 unx      836 b- defN 24-Mar-17 19:07 AlpineHtmxWebViewTest/Math.py
--rw-r--r--  2.0 unx      599 b- defN 24-Mar-17 19:07 AlpineHtmxWebViewTest/__init__.py
--rw-r--r--  2.0 unx     1092 b- defN 24-Mar-17 19:08 AlpineHtmxWebViewTest-0.1.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     6342 b- defN 24-Mar-17 19:08 AlpineHtmxWebViewTest-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-17 19:08 AlpineHtmxWebViewTest-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       79 b- defN 24-Mar-17 19:08 AlpineHtmxWebViewTest-0.1.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       34 b- defN 24-Mar-17 19:08 AlpineHtmxWebViewTest-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      906 b- defN 24-Mar-17 19:08 AlpineHtmxWebViewTest-0.1.2.dist-info/RECORD
-10 files, 16044 bytes uncompressed, 5984 bytes compressed:  62.7%
+Zip file size: 8097 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     3522 b- defN 24-Mar-22 16:30 BuildBinary.py
+-rw-r--r--  2.0 unx     2630 b- defN 24-Mar-22 16:30 AlpineHtmxWebViewTest/EntryPoint.py
+-rw-r--r--  2.0 unx     1739 b- defN 24-Mar-22 16:30 AlpineHtmxWebViewTest/Server.py
+-rw-r--r--  2.0 unx      560 b- defN 24-Mar-22 16:31 AlpineHtmxWebViewTest/__init__.py
+-rw-r--r--  2.0 unx     1092 b- defN 24-Mar-22 16:31 AlpineHtmxWebViewTest-0.1.6.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     6405 b- defN 24-Mar-22 16:31 AlpineHtmxWebViewTest-0.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-22 16:31 AlpineHtmxWebViewTest-0.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       79 b- defN 24-Mar-22 16:31 AlpineHtmxWebViewTest-0.1.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       34 b- defN 24-Mar-22 16:31 AlpineHtmxWebViewTest-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      909 b- defN 24-Mar-22 16:31 AlpineHtmxWebViewTest-0.1.6.dist-info/RECORD
+10 files, 17062 bytes uncompressed, 6515 bytes compressed:  61.8%
```

## zipnote {}

```diff
@@ -1,31 +1,31 @@
 Filename: BuildBinary.py
 Comment: 
 
 Filename: AlpineHtmxWebViewTest/EntryPoint.py
 Comment: 
 
-Filename: AlpineHtmxWebViewTest/Math.py
+Filename: AlpineHtmxWebViewTest/Server.py
 Comment: 
 
 Filename: AlpineHtmxWebViewTest/__init__.py
 Comment: 
 
-Filename: AlpineHtmxWebViewTest-0.1.2.dist-info/LICENSE.txt
+Filename: AlpineHtmxWebViewTest-0.1.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: AlpineHtmxWebViewTest-0.1.2.dist-info/METADATA
+Filename: AlpineHtmxWebViewTest-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: AlpineHtmxWebViewTest-0.1.2.dist-info/WHEEL
+Filename: AlpineHtmxWebViewTest-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: AlpineHtmxWebViewTest-0.1.2.dist-info/entry_points.txt
+Filename: AlpineHtmxWebViewTest-0.1.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: AlpineHtmxWebViewTest-0.1.2.dist-info/top_level.txt
+Filename: AlpineHtmxWebViewTest-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: AlpineHtmxWebViewTest-0.1.2.dist-info/RECORD
+Filename: AlpineHtmxWebViewTest-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## AlpineHtmxWebViewTest/EntryPoint.py

```diff
@@ -4,19 +4,24 @@
 # |  Distributed under the MIT License.
 # |
 # ----------------------------------------------------------------------
 """This file serves as an example of how to create scripts that can be invoked from the command line once the package is installed."""
 
 import sys
 
+from typing import Annotated
+
 import typer
+import webview
 
-from typer.core import TyperGroup  # type: ignore [import-untyped]
+from dbrownell_Common.Streams.DoneManager import DoneManager, Flags as DoneManagerFlags
+from typer.core import TyperGroup
 
-from AlpineHtmxWebViewTest import Math, __version__
+from AlpineHtmxWebViewTest import __version__
+from AlpineHtmxWebViewTest.Server import app as server
 
 
 # ----------------------------------------------------------------------
 class NaturalOrderGrouper(TyperGroup):
     # pylint: disable=missing-class-docstring
     # ----------------------------------------------------------------------
     def list_commands(self, *args, **kwargs):  # pylint: disable=unused-argument
@@ -30,63 +35,51 @@
     no_args_is_help=True,
     pretty_exceptions_show_locals=False,
     pretty_exceptions_enable=False,
 )
 
 
 # ----------------------------------------------------------------------
-@app.command("Add")
-def Add(
-    x: int,
-    y: int,
-) -> None:
-    """Adds 2 values."""
-
-    sys.stdout.write(str(Math.Add(x, y)))
-
-
-# ----------------------------------------------------------------------
-@app.command("Sub")
-def Sub(
-    x: int,
-    y: int,
-) -> None:
-    """Subtracts 2 values."""
-
-    sys.stdout.write(str(Math.Sub(x, y)))
-
-
-# ----------------------------------------------------------------------
-@app.command("Mult")
-def Mult(
-    x: int,
-    y: int,
+@app.command("EntryPoint", no_args_is_help=False)
+def EntryPoint(
+    version: Annotated[
+        bool,
+        typer.Option(
+            "--version",
+            help="Displays version info and exists.",
+        ),
+    ] = False,
+    verbose: Annotated[
+        bool,
+        typer.Option(
+            "--verbose",
+            help="Write verbose information to the terminal.",
+        ),
+    ] = False,
+    debug: Annotated[
+        bool,
+        typer.Option(
+            "--debug",
+            help="Write debug information to the terminal.",
+        ),
+    ] = False,
 ) -> None:
-    """Multiplies 2 values."""
-
-    sys.stdout.write(str(Math.Mult(x, y)))
-
-
-# ----------------------------------------------------------------------
-@app.command("Div")
-def Div(
-    x: int,
-    y: int,
-) -> None:
-    """Divides 1 value by another."""
-
-    sys.stdout.write(str(Math.Div(x, y)))
-
-
-# ----------------------------------------------------------------------
-@app.command("Version")
-def Version() -> None:
-    """Prints the version of the package."""
-
-    sys.stdout.write(__version__)
+    if version:
+        sys.stdout.write(f"AlpineHtmxWebViewTest {__version__}")
+        return
+
+    with DoneManager.CreateCommandLine(
+        flags=DoneManagerFlags.Create(verbose=verbose, debug=debug),
+    ) as dm:
+        webview.create_window("AlpineHtmxWebViewTest", server)
+
+        webview.start(
+            # debug=True,
+            ssl=True,
+        )
 
 
 # ----------------------------------------------------------------------
 # ----------------------------------------------------------------------
 # ----------------------------------------------------------------------
 if __name__ == "__main__":
-    app()  # pragma: no cover
+    app()
```

## AlpineHtmxWebViewTest/__init__.py

```diff
@@ -5,10 +5,8 @@
 # |
 # ----------------------------------------------------------------------
 # pylint: disable=missing-module-docstring,invalid-name
 
 # Note that this value will be overwritten by calls to `python ../../Build.py update_version` based
 # on changes observed in the git repository. The default value below will be used until the value
 # here is explicitly updated as part of a commit.
-__version__ = "0.1.2"
-
-from .Math import Add, Sub, Mult, Div
+__version__ = "0.1.6"
```

## Comparing `AlpineHtmxWebViewTest-0.1.2.dist-info/LICENSE.txt` & `AlpineHtmxWebViewTest-0.1.6.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `AlpineHtmxWebViewTest-0.1.2.dist-info/METADATA` & `AlpineHtmxWebViewTest-0.1.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlpineHtmxWebViewTest
-Version: 0.1.2
+Version: 0.1.6
 Summary: Test repo for a solution that uses Alpine.js, HTMX, and pywebview.
 Author-email: David Brownell <db@DavidBrownell.com>
 License: MIT
 Project-URL: Homepage, https://github.com/davidbrownell/AlpineHtmxWebViewTest
 Project-URL: Documentation, https://github.com/davidbrownell/AlpineHtmxWebViewTest
 Project-URL: Repository, https://github.com/davidbrownell/AlpineHtmxWebViewTest
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,16 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: bleach ==6.*
+Requires-Dist: cryptography ==42.*
 Requires-Dist: dbrownell-Common
 Requires-Dist: flask ==3.*
 Requires-Dist: pywebview ==5.*
 Requires-Dist: typer ~=0.9
 Provides-Extra: dev
 Requires-Dist: dbrownell-DevTools ; extra == 'dev'
 Provides-Extra: package
```

## Comparing `AlpineHtmxWebViewTest-0.1.2.dist-info/RECORD` & `AlpineHtmxWebViewTest-0.1.6.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BuildBinary.py,sha256=l_zn8PmmUo0uOMxy3pBfCnmNUVqA9GwvicToCYQO3l4,3522
-AlpineHtmxWebViewTest/EntryPoint.py,sha256=KPUIOVyMw-ZYP-HMLs8Sn9BYXEMjlUst4GfT0zISbfI,2542
-AlpineHtmxWebViewTest/Math.py,sha256=MtgI9Z0NRqGDttTofzM2UPlD3u4Lm91pxKX5Dl65nIQ,836
-AlpineHtmxWebViewTest/__init__.py,sha256=XmD_e3u4lNWd5njJegLG7wKXzEUivTZpU9CQhboj_PM,599
-AlpineHtmxWebViewTest-0.1.2.dist-info/LICENSE.txt,sha256=P0fqGEJwVh6ADlvhWsPNxwWII2O0VaoyMKUcjDqsOOM,1092
-AlpineHtmxWebViewTest-0.1.2.dist-info/METADATA,sha256=ql9HkKmqswt0VYgrTuj5wU8_p1lIUmXzhSRmwQnFz6U,6342
-AlpineHtmxWebViewTest-0.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-AlpineHtmxWebViewTest-0.1.2.dist-info/entry_points.txt,sha256=7Xt24fXdUn35R29ZbTuzJ4whWXbRoaVkjh1yO5JUMm4,79
-AlpineHtmxWebViewTest-0.1.2.dist-info/top_level.txt,sha256=BuQTEp1oQjppDXSdkYBbyIbdSf5P5ttv696j2Ppy0H0,34
-AlpineHtmxWebViewTest-0.1.2.dist-info/RECORD,,
+AlpineHtmxWebViewTest/EntryPoint.py,sha256=wGHEK-RqOXMD34q2muKk18pKKp5ksnWOOujKuvWixkc,2630
+AlpineHtmxWebViewTest/Server.py,sha256=CB-32OPpG6EQWoK9JVvnvyXleBZ-uiixUdIH4I1ug8Q,1739
+AlpineHtmxWebViewTest/__init__.py,sha256=YZACjJ27tINWYl8IOZ3Od3-fIGdIKmdAs1Oko2PGgHM,560
+AlpineHtmxWebViewTest-0.1.6.dist-info/LICENSE.txt,sha256=P0fqGEJwVh6ADlvhWsPNxwWII2O0VaoyMKUcjDqsOOM,1092
+AlpineHtmxWebViewTest-0.1.6.dist-info/METADATA,sha256=ALv5TS1OWCkenykq2HbaY98xsvA5_S-bAhZBM2bmjzM,6405
+AlpineHtmxWebViewTest-0.1.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+AlpineHtmxWebViewTest-0.1.6.dist-info/entry_points.txt,sha256=7Xt24fXdUn35R29ZbTuzJ4whWXbRoaVkjh1yO5JUMm4,79
+AlpineHtmxWebViewTest-0.1.6.dist-info/top_level.txt,sha256=BuQTEp1oQjppDXSdkYBbyIbdSf5P5ttv696j2Ppy0H0,34
+AlpineHtmxWebViewTest-0.1.6.dist-info/RECORD,,
```

