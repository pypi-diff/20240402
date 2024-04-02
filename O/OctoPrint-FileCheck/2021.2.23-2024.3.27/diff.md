# Comparing `tmp/OctoPrint-FileCheck-2021.2.23.tar.gz` & `tmp/OctoPrint-FileCheck-2024.3.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/OctoPrint-FileCheck-2021.2.23.tar", last modified: Tue Feb 23 13:20:00 2021, max compression
+gzip compressed data, was "dist/OctoPrint-FileCheck-2024.3.27.tar", last modified: Tue Apr  2 07:50:11 2024, max compression
```

## Comparing `OctoPrint-FileCheck-2021.2.23.tar` & `OctoPrint-FileCheck-2024.3.27.tar`

### file list

```diff
@@ -1,25 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-23 13:20:00.000000 OctoPrint-FileCheck-2021.2.23/
--rw-r--r--   0 runner    (1001) docker     (121)    34520 2021-02-23 13:19:56.000000 OctoPrint-FileCheck-2021.2.23/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      171 2021-02-23 13:19:56.000000 OctoPrint-FileCheck-2021.2.23/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-23 13:20:00.000000 OctoPrint-FileCheck-2021.2.23/OctoPrint_FileCheck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1501 2021-02-23 13:20:00.000000 OctoPrint-FileCheck-2021.2.23/OctoPrint_FileCheck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      550 2021-02-23 13:20:00.000000 OctoPrint-FileCheck-2021.2.23/OctoPrint_FileCheck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-23 13:20:00.000000 OctoPrint-FileCheck-2021.2.23/OctoPrint_FileCheck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       54 2021-02-23 13:20:00.000000 OctoPrint-FileCheck-2021.2.23/OctoPrint_FileCheck.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-23 13:20:00.000000 OctoPrint-FileCheck-2021.2.23/OctoPrint_FileCheck.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-02-23 13:20:00.000000 OctoPrint-FileCheck-2021.2.23/OctoPrint_FileCheck.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-02-23 13:20:00.000000 OctoPrint-FileCheck-2021.2.23/OctoPrint_FileCheck.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1501 2021-02-23 13:20:00.000000 OctoPrint-FileCheck-2021.2.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      979 2021-02-23 13:19:56.000000 OctoPrint-FileCheck-2021.2.23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-23 13:20:00.000000 OctoPrint-FileCheck-2021.2.23/octoprint_file_check/
--rw-r--r--   0 runner    (1001) docker     (121)     5146 2021-02-23 13:19:56.000000 OctoPrint-FileCheck-2021.2.23/octoprint_file_check/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-23 13:20:00.000000 OctoPrint-FileCheck-2021.2.23/octoprint_file_check/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-23 13:20:00.000000 OctoPrint-FileCheck-2021.2.23/octoprint_file_check/static/js/
--rw-r--r--   0 runner    (1001) docker     (121)     1729 2021-02-23 13:19:56.000000 OctoPrint-FileCheck-2021.2.23/octoprint_file_check/static/js/file_check.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-23 13:20:00.000000 OctoPrint-FileCheck-2021.2.23/octoprint_file_check/translations/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-23 13:20:00.000000 OctoPrint-FileCheck-2021.2.23/octoprint_file_check/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-23 13:20:00.000000 OctoPrint-FileCheck-2021.2.23/octoprint_file_check/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1895 2021-02-23 13:19:56.000000 OctoPrint-FileCheck-2021.2.23/octoprint_file_check/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     2443 2021-02-23 13:19:56.000000 OctoPrint-FileCheck-2021.2.23/octoprint_file_check/translations/de/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (121)      374 2021-02-23 13:20:00.000000 OctoPrint-FileCheck-2021.2.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    25612 2021-02-23 13:19:56.000000 OctoPrint-FileCheck-2021.2.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:50:11.000000 OctoPrint-FileCheck-2024.3.27/
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-02 07:50:08.000000 OctoPrint-FileCheck-2024.3.27/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-02 07:50:08.000000 OctoPrint-FileCheck-2024.3.27/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:50:11.000000 OctoPrint-FileCheck-2024.3.27/OctoPrint_FileCheck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-02 07:50:11.000000 OctoPrint-FileCheck-2024.3.27/OctoPrint_FileCheck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-02 07:50:11.000000 OctoPrint-FileCheck-2024.3.27/OctoPrint_FileCheck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 07:50:11.000000 OctoPrint-FileCheck-2024.3.27/OctoPrint_FileCheck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-02 07:50:11.000000 OctoPrint-FileCheck-2024.3.27/OctoPrint_FileCheck.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 07:50:11.000000 OctoPrint-FileCheck-2024.3.27/OctoPrint_FileCheck.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 07:50:11.000000 OctoPrint-FileCheck-2024.3.27/OctoPrint_FileCheck.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-02 07:50:11.000000 OctoPrint-FileCheck-2024.3.27/OctoPrint_FileCheck.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-02 07:50:11.000000 OctoPrint-FileCheck-2024.3.27/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-02 07:50:08.000000 OctoPrint-FileCheck-2024.3.27/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:50:11.000000 OctoPrint-FileCheck-2024.3.27/octoprint_file_check/
+-rw-r--r--   0 runner    (1001) docker     (127)    15204 2024-04-02 07:50:08.000000 OctoPrint-FileCheck-2024.3.27/octoprint_file_check/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:50:11.000000 OctoPrint-FileCheck-2024.3.27/octoprint_file_check/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:50:11.000000 OctoPrint-FileCheck-2024.3.27/octoprint_file_check/static/clientjs/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-02 07:50:08.000000 OctoPrint-FileCheck-2024.3.27/octoprint_file_check/static/clientjs/file_check.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:50:11.000000 OctoPrint-FileCheck-2024.3.27/octoprint_file_check/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    13537 2024-04-02 07:50:08.000000 OctoPrint-FileCheck-2024.3.27/octoprint_file_check/static/js/file_check.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:50:11.000000 OctoPrint-FileCheck-2024.3.27/octoprint_file_check/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-02 07:50:08.000000 OctoPrint-FileCheck-2024.3.27/octoprint_file_check/templates/file_check_settings.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 07:50:08.000000 OctoPrint-FileCheck-2024.3.27/octoprint_file_check/templates/file_check_wizard_fullcheck.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:50:11.000000 OctoPrint-FileCheck-2024.3.27/octoprint_file_check/templates/snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-02 07:50:08.000000 OctoPrint-FileCheck-2024.3.27/octoprint_file_check/templates/snippets/fileCheckButton.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:50:11.000000 OctoPrint-FileCheck-2024.3.27/octoprint_file_check/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:50:11.000000 OctoPrint-FileCheck-2024.3.27/octoprint_file_check/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:50:11.000000 OctoPrint-FileCheck-2024.3.27/octoprint_file_check/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     7035 2024-04-02 07:50:08.000000 OctoPrint-FileCheck-2024.3.27/octoprint_file_check/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12378 2024-04-02 07:50:08.000000 OctoPrint-FileCheck-2024.3.27/octoprint_file_check/translations/de/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-02 07:50:08.000000 OctoPrint-FileCheck-2024.3.27/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-02 07:50:11.000000 OctoPrint-FileCheck-2024.3.27/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    25312 2024-04-02 07:50:08.000000 OctoPrint-FileCheck-2024.3.27/setup.py
```

### Comparing `OctoPrint-FileCheck-2021.2.23/LICENSE` & `OctoPrint-FileCheck-2024.3.27/LICENSE`

 * *Files identical despite different names*

### Comparing `OctoPrint-FileCheck-2021.2.23/OctoPrint_FileCheck.egg-info/PKG-INFO` & `OctoPrint-FileCheck-2024.3.27/OctoPrint_FileCheck.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 Metadata-Version: 2.1
 Name: OctoPrint-FileCheck
-Version: 2021.2.23
+Version: 2024.3.27
 Summary: Checks for common issues in uploaded files
 Home-page: https://github.com/OctoPrint/OctoPrint-FileCheck
 Author: Gina Häußge
 Author-email: gina@octoprint.org
 License: AGPLv3
 Description: # File Check
         
         The File Check plugin tries to detect common issues in uploaded files that are known to cause
         issues while printing and which in the past have caused support requests on OctoPrint's Community
-        Forums.
+        Forums, as well as leaked sensitive data such as API keys.
         
         ![Screenshot](https://raw.githubusercontent.com/OctoPrint/OctoPrint-FileCheck/master/extras/screenshot.png)
         
         It currently detects and warns about the following issues:
         
           * Outdated placeholder `{travel_speed}` left in the GCODE generated by the slicer. See
             [here](https://faq.octoprint.org/file-check-travel-speed) for details on this.
+          * API keys leaked by the slicer into the GCODE. See
+            [here](https://faq.octoprint.org/file-check-leaked-api-key) for details on this.
+        
+        Since version 2024.3.27 it also supports checking selected files as well as all uploaded files for issues on
+        the press of a button (if `grep` is available), not just freshly uploaded files.
         
         ## Setup
         
         The plugin is part of the core dependencies of OctoPrint 1.4.1+ and will be installed automatically alongside it.
         
-        In case you want to manually install it into an older version for whatever reason, install via the bundled
+        In case you want to manually install it for whatever reason, install via the bundled
         [Plugin Manager](https://docs.octoprint.org/en/master/bundledplugins/pluginmanager.html)
         or manually using this URL:
         
             https://github.com/OctoPrint/OctoPrint-FileCheck/archive/master.zip
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `OctoPrint-FileCheck-2021.2.23/PKG-INFO` & `OctoPrint-FileCheck-2024.3.27/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 Metadata-Version: 2.1
 Name: OctoPrint-FileCheck
-Version: 2021.2.23
+Version: 2024.3.27
 Summary: Checks for common issues in uploaded files
 Home-page: https://github.com/OctoPrint/OctoPrint-FileCheck
 Author: Gina Häußge
 Author-email: gina@octoprint.org
 License: AGPLv3
 Description: # File Check
         
         The File Check plugin tries to detect common issues in uploaded files that are known to cause
         issues while printing and which in the past have caused support requests on OctoPrint's Community
-        Forums.
+        Forums, as well as leaked sensitive data such as API keys.
         
         ![Screenshot](https://raw.githubusercontent.com/OctoPrint/OctoPrint-FileCheck/master/extras/screenshot.png)
         
         It currently detects and warns about the following issues:
         
           * Outdated placeholder `{travel_speed}` left in the GCODE generated by the slicer. See
             [here](https://faq.octoprint.org/file-check-travel-speed) for details on this.
+          * API keys leaked by the slicer into the GCODE. See
+            [here](https://faq.octoprint.org/file-check-leaked-api-key) for details on this.
+        
+        Since version 2024.3.27 it also supports checking selected files as well as all uploaded files for issues on
+        the press of a button (if `grep` is available), not just freshly uploaded files.
         
         ## Setup
         
         The plugin is part of the core dependencies of OctoPrint 1.4.1+ and will be installed automatically alongside it.
         
-        In case you want to manually install it into an older version for whatever reason, install via the bundled
+        In case you want to manually install it for whatever reason, install via the bundled
         [Plugin Manager](https://docs.octoprint.org/en/master/bundledplugins/pluginmanager.html)
         or manually using this URL:
         
             https://github.com/OctoPrint/OctoPrint-FileCheck/archive/master.zip
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `OctoPrint-FileCheck-2021.2.23/README.md` & `OctoPrint-FileCheck-2024.3.27/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 # File Check
 
 The File Check plugin tries to detect common issues in uploaded files that are known to cause
 issues while printing and which in the past have caused support requests on OctoPrint's Community
-Forums.
+Forums, as well as leaked sensitive data such as API keys.
 
 ![Screenshot](https://raw.githubusercontent.com/OctoPrint/OctoPrint-FileCheck/master/extras/screenshot.png)
 
 It currently detects and warns about the following issues:
 
   * Outdated placeholder `{travel_speed}` left in the GCODE generated by the slicer. See
     [here](https://faq.octoprint.org/file-check-travel-speed) for details on this.
+  * API keys leaked by the slicer into the GCODE. See
+    [here](https://faq.octoprint.org/file-check-leaked-api-key) for details on this.
+
+Since version 2024.3.27 it also supports checking selected files as well as all uploaded files for issues on
+the press of a button (if `grep` is available), not just freshly uploaded files.
 
 ## Setup
 
 The plugin is part of the core dependencies of OctoPrint 1.4.1+ and will be installed automatically alongside it.
 
-In case you want to manually install it into an older version for whatever reason, install via the bundled
+In case you want to manually install it for whatever reason, install via the bundled
 [Plugin Manager](https://docs.octoprint.org/en/master/bundledplugins/pluginmanager.html)
 or manually using this URL:
 
     https://github.com/OctoPrint/OctoPrint-FileCheck/archive/master.zip
```

### Comparing `OctoPrint-FileCheck-2021.2.23/setup.py` & `OctoPrint-FileCheck-2024.3.27/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-# -*- coding: utf-8 -*-
-
 ########################################################################################################################
 ### Do not forget to adjust the following variables to your own plugin.
 
 # The plugin's identifier, has to be unique
 plugin_identifier = "file_check"
 
 # The plugin's python package, should be "octoprint_<plugin identifier>", has to be unique
 plugin_package = "octoprint_file_check"
 
 # The plugin's human readable name. Can be overwritten within OctoPrint's internal data via __plugin_name__ in the
 # plugin module
 plugin_name = "OctoPrint-FileCheck"
 
 # The plugin's version. Can be overwritten within OctoPrint's internal data via __plugin_version__ in the plugin module
-plugin_version = "2021.2.23"
+plugin_version = "2024.3.27"
 
 # The plugin's description. Can be overwritten within OctoPrint's internal data via __plugin_description__ in the plugin
 # module
 plugin_description = """Checks for common issues in uploaded files"""
 
 # The plugin's author. Can be overwritten within OctoPrint's internal data via __plugin_author__ in the plugin module
 plugin_author = "Gina Häußge"
@@ -459,17 +457,15 @@
             if not os.path.isdir(target_path):
                 raise RuntimeError(
                     "target path " + target_path + " exists and is not a directory"
                 )
             shutil.rmtree(target_path)
 
         print(
-            "Copying translations for locale {locale} from {source_path} to {target_path}...".format(
-                **locals()
-            )
+            f"Copying translations for locale {locale} from {source_path} to {target_path}..."
         )
         shutil.copytree(source_path, target_path)
 
 
 class PackTranslation(Command):
     description = "creates language packs for translations"
     user_options = [
@@ -529,41 +525,41 @@
             self.target,
             "{prefix}{locale}_{date}.zip".format(
                 prefix=self.__class__.pack_name_prefix,
                 locale=locale,
                 date=now.strftime("%Y%m%d%H%M%S"),
             ),
         )
-        print("Packing translation to {zip_path}".format(**locals()))
+        print(f"Packing translation to {zip_path}")
 
         def add_recursively(zip, path, prefix):
             if not os.path.isdir(path):
                 return
 
             for entry in os.listdir(path):
                 entry_path = os.path.join(path, entry)
                 new_prefix = prefix + "/" + entry
                 if os.path.isdir(entry_path):
                     add_recursively(zip, entry_path, new_prefix)
                 elif os.path.isfile(entry_path):
-                    print("Adding {entry_path} as {new_prefix}".format(**locals()))
+                    print(f"Adding {entry_path} as {new_prefix}")
                     zip.write(entry_path, new_prefix)
 
-        meta_str = "last_update: {date}\n".format(date=now.isoformat())
+        meta_str = f"last_update: {now.isoformat()}\n"
         if self.author:
-            meta_str += "author: {author}\n".format(author=self.author)
+            meta_str += f"author: {self.author}\n"
 
         zip_locale_root = self.__class__.pack_path_prefix + locale
 
         import zipfile
 
         with zipfile.ZipFile(zip_path, "w") as zip:
             add_recursively(zip, locale_dir, zip_locale_root)
 
-            print("Adding meta.yaml as {zip_locale_root}/meta.yaml".format(**locals()))
+            print(f"Adding meta.yaml as {zip_locale_root}/meta.yaml")
             zip.writestr(zip_locale_root + "/meta.yaml", meta_str)
 
 
 def get_babel_commandclasses(
     pot_file=None,
     mapping_file="babel.cfg",
     input_dirs=".",
@@ -626,15 +622,15 @@
     eggs=None,
     package=None,
     dependency_links=None,
 ):
     import pkg_resources
 
     if package is None:
-        package = "octoprint_{identifier}".format(**locals())
+        package = f"octoprint_{identifier}"
 
     if additional_data is None:
         additional_data = list()
 
     if additional_packages is None:
         additional_packages = list()
 
@@ -682,32 +678,32 @@
     pot_file = os.path.join(translation_dir, "messages.pot")
     bundled_dir = os.path.join(source_folder, package, "translations")
     cmdclass.update(
         get_babel_commandclasses(
             pot_file=pot_file,
             output_dir=translation_dir,
             bundled_dir=bundled_dir,
-            pack_name_prefix="{name}-i18n-".format(**locals()),
-            pack_path_prefix="_plugins/{identifier}/".format(**locals()),
+            pack_name_prefix=f"{name}-i18n-",
+            pack_path_prefix=f"_plugins/{identifier}/",
         )
     )
 
     from setuptools import find_packages
 
     packages = set(
         [package]
         + list(
             filter(
-                lambda x: x.startswith("{package}.".format(package=package)),
+                lambda x: x.startswith(f"{package}."),
                 find_packages(where=source_folder, exclude=ignored_packages),
             )
         )
         + additional_packages
     )
-    print("Found packages: {packages!r}".format(**locals()))
+    print(f"Found packages: {packages!r}")
 
     return dict(
         name=name,
         version=version,
         description=description,
         author=author,
         author_email=mail,
@@ -729,17 +725,15 @@
         # this plugin is not zip_safe.
         zip_safe=False,
         install_requires=requires,
         extras_require=extra_requires,
         dependency_links=dependency_links,
         # Hook the plugin into the "octoprint.plugin" entry point, mapping the plugin_identifier to the plugin_package.
         # That way OctoPrint will be able to find the plugin and load it.
-        entry_points={
-            "octoprint.plugin": ["{identifier} = {package}".format(**locals())]
-        },
+        entry_points={"octoprint.plugin": [f"{identifier} = {package}"]},
     )
 
 
 def read_file_contents(path):
     import codecs
 
     with codecs.open(path, encoding="utf-8") as f:
```

