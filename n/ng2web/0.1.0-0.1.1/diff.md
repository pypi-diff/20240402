# Comparing `tmp/ng2web-0.1.0.tar.gz` & `tmp/ng2web-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ng2web-0.1.0.tar", last modified: Sun Mar 31 13:17:58 2024, max compression
+gzip compressed data, was "ng2web-0.1.1.tar", last modified: Tue Apr  2 07:08:02 2024, max compression
```

## Comparing `ng2web-0.1.0.tar` & `ng2web-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-03-31 13:17:58.177549 ng2web-0.1.0/
--rw-r--r--   0 davep      (501) staff       (20)    35141 2024-03-31 13:04:55.000000 ng2web-0.1.0/LICENSE
--rw-r--r--   0 davep      (501) staff       (20)     2016 2024-03-31 13:17:58.177376 ng2web-0.1.0/PKG-INFO
--rw-r--r--   0 davep      (501) staff       (20)      758 2024-03-31 13:04:55.000000 ng2web-0.1.0/README.md
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-03-31 13:17:58.175365 ng2web-0.1.0/ng2web/
--rw-r--r--   0 davep      (501) staff       (20)      399 2024-03-31 13:16:54.000000 ng2web-0.1.0/ng2web/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)      313 2024-03-31 13:04:55.000000 ng2web-0.1.0/ng2web/__main__.py
--rw-r--r--   0 davep      (501) staff       (20)    12458 2024-03-31 13:16:36.000000 ng2web-0.1.0/ng2web/ng2web.py
--rw-r--r--   0 davep      (501) staff       (20)        0 2024-03-31 13:04:55.000000 ng2web-0.1.0/ng2web/py.typed
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-03-31 13:17:58.176820 ng2web-0.1.0/ng2web/templates/
--rw-r--r--   0 davep      (501) staff       (20)      317 2024-03-31 13:04:55.000000 ng2web-0.1.0/ng2web/templates/about.html
--rw-r--r--   0 davep      (501) staff       (20)     2912 2024-03-31 13:04:55.000000 ng2web-0.1.0/ng2web/templates/base.css
--rw-r--r--   0 davep      (501) staff       (20)     1617 2024-03-31 13:04:55.000000 ng2web-0.1.0/ng2web/templates/base.html
--rw-r--r--   0 davep      (501) staff       (20)      592 2024-03-31 13:04:55.000000 ng2web-0.1.0/ng2web/templates/entry.html
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-03-31 13:17:58.176940 ng2web-0.1.0/ng2web/templates/inc/
--rw-r--r--   0 davep      (501) staff       (20)      193 2024-03-31 13:04:55.000000 ng2web-0.1.0/ng2web/templates/inc/nav-link.html
--rw-r--r--   0 davep      (501) staff       (20)      394 2024-03-31 13:04:55.000000 ng2web-0.1.0/ng2web/templates/long.html
--rw-r--r--   0 davep      (501) staff       (20)       85 2024-03-31 13:04:55.000000 ng2web-0.1.0/ng2web/templates/short.html
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-03-31 13:17:58.177201 ng2web-0.1.0/ng2web.egg-info/
--rw-r--r--   0 davep      (501) staff       (20)     2016 2024-03-31 13:17:58.000000 ng2web-0.1.0/ng2web.egg-info/PKG-INFO
--rw-r--r--   0 davep      (501) staff       (20)      496 2024-03-31 13:17:58.000000 ng2web-0.1.0/ng2web.egg-info/SOURCES.txt
--rw-r--r--   0 davep      (501) staff       (20)        1 2024-03-31 13:17:58.000000 ng2web-0.1.0/ng2web.egg-info/dependency_links.txt
--rw-r--r--   0 davep      (501) staff       (20)       46 2024-03-31 13:17:58.000000 ng2web-0.1.0/ng2web.egg-info/entry_points.txt
--rw-r--r--   0 davep      (501) staff       (20)       12 2024-03-31 13:17:58.000000 ng2web-0.1.0/ng2web.egg-info/requires.txt
--rw-r--r--   0 davep      (501) staff       (20)       13 2024-03-31 13:17:58.000000 ng2web-0.1.0/ng2web.egg-info/top_level.txt
--rw-r--r--   0 davep      (501) staff       (20)       38 2024-03-31 13:17:58.177585 ng2web-0.1.0/setup.cfg
--rw-r--r--   0 davep      (501) staff       (20)     3094 2024-03-31 13:04:55.000000 ng2web-0.1.0/setup.py
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-03-31 13:17:58.177057 ng2web-0.1.0/tests/
--rw-r--r--   0 davep      (501) staff       (20)       52 2024-03-31 13:04:55.000000 ng2web-0.1.0/tests/__init__.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-02 07:08:02.874926 ng2web-0.1.1/
+-rw-r--r--   0 davep      (501) staff       (20)    35141 2024-03-31 13:04:55.000000 ng2web-0.1.1/LICENSE
+-rw-r--r--   0 davep      (501) staff       (20)     2016 2024-04-02 07:08:02.874746 ng2web-0.1.1/PKG-INFO
+-rw-r--r--   0 davep      (501) staff       (20)      758 2024-03-31 13:04:55.000000 ng2web-0.1.1/README.md
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-02 07:08:02.872898 ng2web-0.1.1/ng2web/
+-rw-r--r--   0 davep      (501) staff       (20)      399 2024-04-02 07:07:09.000000 ng2web-0.1.1/ng2web/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)      313 2024-03-31 13:04:55.000000 ng2web-0.1.1/ng2web/__main__.py
+-rw-r--r--   0 davep      (501) staff       (20)    11983 2024-03-31 13:33:17.000000 ng2web-0.1.1/ng2web/ng2web.py
+-rw-r--r--   0 davep      (501) staff       (20)        0 2024-03-31 13:04:55.000000 ng2web-0.1.1/ng2web/py.typed
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-02 07:08:02.874201 ng2web-0.1.1/ng2web/templates/
+-rw-r--r--   0 davep      (501) staff       (20)      317 2024-03-31 13:04:55.000000 ng2web-0.1.1/ng2web/templates/about.html
+-rw-r--r--   0 davep      (501) staff       (20)     2912 2024-03-31 13:04:55.000000 ng2web-0.1.1/ng2web/templates/base.css
+-rw-r--r--   0 davep      (501) staff       (20)     1617 2024-03-31 13:04:55.000000 ng2web-0.1.1/ng2web/templates/base.html
+-rw-r--r--   0 davep      (501) staff       (20)      592 2024-03-31 13:04:55.000000 ng2web-0.1.1/ng2web/templates/entry.html
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-02 07:08:02.874336 ng2web-0.1.1/ng2web/templates/inc/
+-rw-r--r--   0 davep      (501) staff       (20)      193 2024-03-31 13:04:55.000000 ng2web-0.1.1/ng2web/templates/inc/nav-link.html
+-rw-r--r--   0 davep      (501) staff       (20)      394 2024-03-31 13:04:55.000000 ng2web-0.1.1/ng2web/templates/long.html
+-rw-r--r--   0 davep      (501) staff       (20)       85 2024-03-31 13:04:55.000000 ng2web-0.1.1/ng2web/templates/short.html
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-02 07:08:02.874581 ng2web-0.1.1/ng2web.egg-info/
+-rw-r--r--   0 davep      (501) staff       (20)     2016 2024-04-02 07:08:02.000000 ng2web-0.1.1/ng2web.egg-info/PKG-INFO
+-rw-r--r--   0 davep      (501) staff       (20)      496 2024-04-02 07:08:02.000000 ng2web-0.1.1/ng2web.egg-info/SOURCES.txt
+-rw-r--r--   0 davep      (501) staff       (20)        1 2024-04-02 07:08:02.000000 ng2web-0.1.1/ng2web.egg-info/dependency_links.txt
+-rw-r--r--   0 davep      (501) staff       (20)       46 2024-04-02 07:08:02.000000 ng2web-0.1.1/ng2web.egg-info/entry_points.txt
+-rw-r--r--   0 davep      (501) staff       (20)       12 2024-04-02 07:08:02.000000 ng2web-0.1.1/ng2web.egg-info/requires.txt
+-rw-r--r--   0 davep      (501) staff       (20)       13 2024-04-02 07:08:02.000000 ng2web-0.1.1/ng2web.egg-info/top_level.txt
+-rw-r--r--   0 davep      (501) staff       (20)       38 2024-04-02 07:08:02.874963 ng2web-0.1.1/setup.cfg
+-rw-r--r--   0 davep      (501) staff       (20)     3094 2024-03-31 13:04:55.000000 ng2web-0.1.1/setup.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-02 07:08:02.874443 ng2web-0.1.1/tests/
+-rw-r--r--   0 davep      (501) staff       (20)       52 2024-03-31 13:04:55.000000 ng2web-0.1.1/tests/__init__.py
```

### Comparing `ng2web-0.1.0/LICENSE` & `ng2web-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ng2web-0.1.0/PKG-INFO` & `ng2web-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ng2web
-Version: 0.1.0
+Version: 0.1.1
 Summary: ng2web -- Norton Guide to HTML conversion tool.
 Home-page: https://github.com/davep/ng2web
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `ng2web-0.1.0/README.md` & `ng2web-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ng2web-0.1.0/ng2web/ng2web.py` & `ng2web-0.1.1/ng2web/ng2web.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,60 +23,60 @@
 
 
 ##############################################################################
 def log(msg: str) -> None:
     """Simple logging function.
 
     Args:
-        msg (str): The message to log.
+        msg: The message to log.
 
     At some point soon I'll possibly switch to proper logging, but just for
     now...
     """
     print(msg)
 
 
 ##############################################################################
 def prefix(text: str, guide: NortonGuide) -> str:
     """Prefix the given text with the guide's namespace.
 
     Args:
-        text (str): The text to prefix.
-        guide (NortonGuide): The guide we're working with.
+        text: The text to prefix.
+        guide: The guide we're working with.
 
     Returns:
-        str: The prefixed text.
+        The prefixed text.
     """
     return f"{guide.path.stem}-{text}"
 
 
 ##############################################################################
 def output(args: argparse.Namespace, file_name: Path | str) -> Path:
     """Expand a file's name so that it's within the output location.
 
     Args:
-        args (argparse.Namespace): The command line arguments.
-        file_name (Path | str): The file's name.
+        args: The command line arguments.
+        file_name: The file's name.
 
     Returns:
-        Path: The full path to the file, within the output location.
+        The full path to the file, within the output location.
 
     Note:
        This function will expand any user information within the specified
        output path and also resolve the result.
     """
     return Path(args.output).expanduser().resolve() / Path(file_name)
 
 
 ##############################################################################
 def get_args() -> argparse.Namespace:
     """Get the arguments passed by the user.
 
     Returns:
-        argparse.Namespace: The parsed arguments.
+        The parsed arguments.
     """
 
     # Version information, used in a couple of paces.
     version = f"v{__version__} (ngdb v{ngdb_ver}; Jinja2 v{jinja_version})"
 
     # Create the argument parser object.
     parser = argparse.ArgumentParser(
@@ -110,59 +110,59 @@
 
 
 ##############################################################################
 def about(guide: NortonGuide, args: argparse.Namespace) -> Path:
     """Get the name of the about page for the guide.
 
     Args:
-        guide (NortonGuide): The guide to generate the about name for.
-        args (argparse.Namespace): The command line arguments.
+        guide: The guide to generate the about name for.
+        args: The command line arguments.
 
     Returns:
-        Path: The path to the about file for the guide.
+        The path to the about file for the guide.
     """
     return output(args, prefix("about.html", guide))
 
 
 ##############################################################################
 def write_about(guide: NortonGuide, args: argparse.Namespace, env: Environment) -> None:
     """Write the about page for the guide.
 
     Args:
-        guide (NortonGuide): The guide to generate the about name for.
-        args (argparse.Namespace): The command line arguments.
-        env (Environment): The template environment.
+        guide: The guide to generate the about name for.
+        args: The command line arguments.
+        env: The template environment.
     """
     log(f"Writing about into {about( guide, args )}")
     with about(guide, args).open("w") as target:
         target.write(env.get_template("about.html").render())
 
 
 ##############################################################################
 def css(guide: NortonGuide, args: argparse.Namespace) -> Path:
     """Get the name of the stylesheet for the guide.
 
     Args:
-        guide (NortonGuide): The guide to generate the css name for.
-        args (argparse.Namespace): The command line arguments.
+        guide: The guide to generate the css name for.
+        args: The command line arguments.
 
     Returns:
-        Path: The path to the stylesheet for the guide.
+        The path to the stylesheet for the guide.
     """
     return output(args, prefix("style.css", guide))
 
 
 ##############################################################################
 def write_css(guide: NortonGuide, args: argparse.Namespace, env: Environment) -> None:
     """Write the stylesheet for the guide.
 
     Args:
-        guide (NortonGuide): The guide to generate the stylesheet for.
-        args (argparse.Namespace): The command line arguments.
-        env (Environment): The template environment.
+        guide: The guide to generate the stylesheet for.
+        args: The command line arguments.
+        env: The template environment.
     """
     log(f"Writing stylesheet into {css( guide, args )}")
     with css(guide, args).open("w") as target:
         target.write(
             env.get_template("base.css").render(
                 colours=enumerate(
                     (
@@ -191,20 +191,20 @@
 ##############################################################################
 def entry_file(
     guide: NortonGuide, args: argparse.Namespace, location: int | Entry
 ) -> Path:
     """Get the name of an entry in the guide.
 
     Args:
-        guide (NortonGuide): The guide to generate the entry file name for.
-        args (argparse.Namespace): The command line arguments.
-        location (int | Entry): The location of the entry.
+        guid: The guide to generate the entry file name for.
+        args: The command line arguments.
+        location: The location of the entry.
 
     Returns:
-        Path: The path to the entry file name for the guide.
+        The path to the entry file name for the guide.
     """
     return output(
         args,
         prefix(
             f"{ location if isinstance( location, int ) else location.offset }.html",
             guide,
         ),
@@ -214,18 +214,18 @@
 ##############################################################################
 def write_entry(
     entry: Entry, guide: NortonGuide, args: argparse.Namespace, env: Environment
 ) -> None:
     """Write the an entry from the guide.
 
     Args:
-        entry (Entry): The entry to write.
-        guide (NortonGuide): The guide the entry came from.
-        args (argparse.Namespace): The command line arguments.
-        env (Environment): The template environment.
+        entry: The entry to write.
+        guide: The guide the entry came from.
+        args: The command line arguments.
+        env: The template environment.
     """
     log(
         f"Writing {entry.__class__.__name__.lower()} entry to {entry_file( guide, args, entry )}"
     )
     with entry_file(guide, args, entry).open("w") as target:
         target.write(
             env.get_template(f"{entry.__class__.__name__.lower()}.html").render(
@@ -251,46 +251,46 @@
 class ToHTML(MarkupText):
     """Class to convert some Norton Guide source into HTML"""
 
     def open_markup(self, cls: str) -> str:
         """Open markup for the given class.
 
         Args:
-            cls (str): The class of thing to open the markup for.
+            cls: The class of thing to open the markup for.
 
         Returns:
-            str: The opening markup text.
+            The opening markup text.
         """
         return f'<span class="{cls}">'
 
     def close_markup(self, cls: str) -> str:
         """Close markup for the given class.
 
         Args:
-            cls (str): The class of thing to close the markup for.
+            cls: The class of thing to close the markup for.
 
         Returns:
-            str: The closing markup text.
+            The closing markup text.
         """
         del cls
         return "</span>"
 
     def text(self, text: str) -> None:
         """Handle the given text.
 
         Args:
-            text (str): The text to handle.
+            text: The text to handle.
         """
         super().text(str(escape(make_dos_like(text))))
 
     def colour(self, colour: int) -> None:
         """Handle the given colour value.
 
         Args:
-            colour (int): The colour value to handle.
+            colour: The colour value to handle.
         """
         self.begin_markup(f"fg{ colour & 0xF} bg{ colour >> 4}")
 
     def bold(self) -> None:
         """Handle being asked to go to bold mode."""
         self.begin_markup("ngb")
 
@@ -316,19 +316,19 @@
 
 
 ##############################################################################
 def page_title(guide: NortonGuide, entry: Entry | None = None) -> str:
     """Generate a title appropriate for the current page.
 
     Args:
-        guide (NortonGuide): The guide that the entry came from.
-        entry (ngdb.Entry | None, optional): The entry to get the title for.
+        guide: The guide that the entry came from.
+        entry: The entry to get the title for.
 
     Returns:
-        str: A title for the current page.
+        A title for the current page.
     """
 
     # Start with the guide title.
     title = [guide.title]
 
     # If there's a parent menu...
     if entry and entry.parent.has_menu:
@@ -343,15 +343,15 @@
 
 
 ##############################################################################
 def to_html(args: argparse.Namespace) -> None:
     """Convert a Norton Guide into HTML.
 
     Args:
-        args (argparse.Namespace): The command line arguments.
+        args: The command line arguments.
     """
 
     # Open the guide. Note that we turn it into a Path, and just to be kind
     # to folk, we attempt to expand any sort of ~ inside it first.
     with NortonGuide(Path(args.guide).expanduser().resolve()) as guide:
 
         # Log some basics.
@@ -360,27 +360,27 @@
 
         # Bootstrap the template stuff.
         env = Environment(
             loader=PackageLoader(Path(__file__).stem), autoescape=select_autoescape()
         )
 
         # Set up the global variables for template expansion.
-        env.globals = dict(
-            generator=f"ng2web v{__version__} (ngdb v{ngdb_ver})",
-            guide=guide,
-            about_url=about(guide, args).name,
-            stylesheet=css(guide, args).name,
-        )
+        env.globals = {
+            "generator": f"ng2web v{__version__} (ngdb v{ngdb_ver})",
+            "guide": guide,
+            "about_url": about(guide, args).name,
+            "stylesheet": css(guide, args).name,
+        }
 
         # Set up the filters for the guide templates.
-        env.filters = dict(
-            urlify=lambda option: entry_file(guide, args, option.offset).name,
-            toHTML=lambda src: Markup(ToHTML(src)),
-            title=lambda entry: page_title(guide, entry),
-        )
+        env.filters = {
+            "urlify": lambda option: entry_file(guide, args, option.offset).name,
+            "toHTML": lambda src: Markup(ToHTML(src)),
+            "title": lambda entry: page_title(guide, entry),
+        }
 
         # Write the stylesheet.
         write_css(guide, args, env)
 
         # Write the about page.
         write_about(guide, args, env)
```

### Comparing `ng2web-0.1.0/ng2web/templates/base.css` & `ng2web-0.1.1/ng2web/templates/base.css`

 * *Files identical despite different names*

### Comparing `ng2web-0.1.0/ng2web/templates/base.html` & `ng2web-0.1.1/ng2web/templates/base.html`

 * *Files identical despite different names*

### Comparing `ng2web-0.1.0/ng2web/templates/entry.html` & `ng2web-0.1.1/ng2web/templates/entry.html`

 * *Files identical despite different names*

### Comparing `ng2web-0.1.0/ng2web.egg-info/PKG-INFO` & `ng2web-0.1.1/ng2web.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ng2web
-Version: 0.1.0
+Version: 0.1.1
 Summary: ng2web -- Norton Guide to HTML conversion tool.
 Home-page: https://github.com/davep/ng2web
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `ng2web-0.1.0/setup.py` & `ng2web-0.1.1/setup.py`

 * *Files identical despite different names*

