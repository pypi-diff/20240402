# Comparing `tmp/python_gettext_translations-1.0.1.tar.gz` & `tmp/python_gettext_translations-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_gettext_translations-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "python_gettext_translations-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `python_gettext_translations-1.0.1.tar` & `python_gettext_translations-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       16 2024-03-21 01:01:02.867021 python_gettext_translations-1.0.1/.gitignore
--rw-r--r--   0        0        0      767 2024-03-21 01:00:01.761261 python_gettext_translations-1.0.1/README.rst
--rw-r--r--   0        0        0      583 2024-03-21 01:12:29.971819 python_gettext_translations-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      131 2024-03-22 14:04:28.808854 python_gettext_translations-1.0.1/python_gettext_translations/__init__.py
--rw-r--r--   0        0        0     1385 2024-03-21 00:41:23.163048 python_gettext_translations-1.0.1/python_gettext_translations/storage.py
--rw-r--r--   0        0        0      511 2024-03-22 14:04:13.395485 python_gettext_translations-1.0.1/python_gettext_translations/translations.py
--rw-r--r--   0        0        0        0 2024-03-21 00:13:27.169114 python_gettext_translations-1.0.1/test/__init__.py
--rw-r--r--   0        0        0      594 2024-03-21 00:30:31.302966 python_gettext_translations-1.0.1/test/i18n/de_DE/messages.po
--rw-r--r--   0        0        0      495 2024-03-21 00:14:47.705907 python_gettext_translations-1.0.1/test/i18n/fr_FR/messages.po
--rw-r--r--   0        0        0        0 2024-03-21 00:42:38.419342 python_gettext_translations-1.0.1/test/i18n/ru_RU/.gitkeep
--rw-r--r--   0        0        0      317 2024-03-21 01:08:22.363791 python_gettext_translations-1.0.1/test/test_storage.py
--rw-r--r--   0        0        0      764 2024-03-21 01:08:35.630549 python_gettext_translations-1.0.1/test/test_translations.py
--rw-r--r--   0        0        0     1102 1970-01-01 00:00:00.000000 python_gettext_translations-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       16 2024-03-21 01:01:02.867021 python_gettext_translations-1.1.0/.gitignore
+-rw-r--r--   0        0        0      781 2024-04-02 16:36:00.903030 python_gettext_translations-1.1.0/README.rst
+-rw-r--r--   0        0        0      583 2024-03-21 01:12:29.971819 python_gettext_translations-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      131 2024-04-02 16:36:34.184973 python_gettext_translations-1.1.0/python_gettext_translations/__init__.py
+-rw-r--r--   0        0        0     1385 2024-03-21 00:41:23.163048 python_gettext_translations-1.1.0/python_gettext_translations/storage.py
+-rw-r--r--   0        0        0      518 2024-04-02 16:35:14.949989 python_gettext_translations-1.1.0/python_gettext_translations/translations.py
+-rw-r--r--   0        0        0        0 2024-03-21 00:13:27.169114 python_gettext_translations-1.1.0/test/__init__.py
+-rw-r--r--   0        0        0      594 2024-03-21 00:30:31.302966 python_gettext_translations-1.1.0/test/i18n/de_DE/messages.po
+-rw-r--r--   0        0        0      495 2024-03-21 00:14:47.705907 python_gettext_translations-1.1.0/test/i18n/fr_FR/messages.po
+-rw-r--r--   0        0        0        0 2024-03-21 00:42:38.419342 python_gettext_translations-1.1.0/test/i18n/ru_RU/.gitkeep
+-rw-r--r--   0        0        0      317 2024-03-21 01:08:22.363791 python_gettext_translations-1.1.0/test/test_storage.py
+-rw-r--r--   0        0        0      799 2024-04-02 16:35:14.955853 python_gettext_translations-1.1.0/test/test_translations.py
+-rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 python_gettext_translations-1.1.0/PKG-INFO
```

### Comparing `python_gettext_translations-1.0.1/README.rst` & `python_gettext_translations-1.1.0/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -12,16 +12,16 @@
     from translations import init_translations
     dir_path = os.path.dirname(os.path.realpath(__file__))
     init_translations(dir_path + "/i18n")
 
 3. Get translation string:
 .. code-block:: python
 
-    from translations import __
-    __("de_DE", "Hello, %user%", {"user": "Alexey"}) # Prints "Hello, Alexey"
+    from translations import translate
+    translate("de_DE", "Hello, %user%", {"user": "Alexey"}) # Prints "Hello, Alexey"
 
 New version release
 --------------------
 
 To release new version:
 1. Update sphinx_integral_theme/__init__.py with new __version__ and __version_info__
 2. Run the following command:
```

### Comparing `python_gettext_translations-1.0.1/pyproject.toml` & `python_gettext_translations-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python_gettext_translations-1.0.1/python_gettext_translations/storage.py` & `python_gettext_translations-1.1.0/python_gettext_translations/storage.py`

 * *Files identical despite different names*

### Comparing `python_gettext_translations-1.0.1/test/i18n/de_DE/messages.po` & `python_gettext_translations-1.1.0/test/i18n/de_DE/messages.po`

 * *Files identical despite different names*

### Comparing `python_gettext_translations-1.0.1/test/test_translations.py` & `python_gettext_translations-1.1.0/test/test_translations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import os
 
-from python_gettext_translations.translations import init_translations, __
+from python_gettext_translations.translations import init_translations, translate
 
 dir_path = os.path.dirname(os.path.realpath(__file__))
 
 def test_happy_pass():
     init_translations(dir_path + "/i18n")
-    assert __("de_DE", "Hello, %user%", {"user": "Alexey"}) == "Hallo, Alexey"
+    assert translate("de_DE", "Hello, %user%", {"user": "Alexey"}) == "Hallo, Alexey"
 
 def test_untranslated_string():
     init_translations(dir_path + "/i18n")
-    assert __("de_DE", "String is not translated in DE") == "String is not translated in DE"
+    assert translate("de_DE", "String is not translated in DE") == "String is not translated in DE"
 
 def test_fr_language():
     init_translations(dir_path + "/i18n")
-    assert __("fr_FR", "Slug is already in use") == "Slug est déjà utilisé"
+    assert translate("fr_FR", "Slug is already in use") == "Slug est déjà utilisé"
 
 def test_nonexisting_key():
     init_translations(dir_path + "/i18n")
-    assert __("fr_FR", "String is not translated in DE") == "String is not translated in DE"
+    assert translate("fr_FR", "String is not translated in DE") == "String is not translated in DE"
```

### Comparing `python_gettext_translations-1.0.1/PKG-INFO` & `python_gettext_translations-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gettext-translations
-Version: 1.0.1
+Version: 1.1.0
 Summary: Python gettext translations
 Keywords: translations,i18n,i18n_mrg
 Author-email: Alexey Zauzin <a.zauzin@thestage.ai>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Requires-Dist: importlib-metadata; python_version<"3.8"
 Requires-Dist: polib
@@ -23,16 +23,16 @@
     from translations import init_translations
     dir_path = os.path.dirname(os.path.realpath(__file__))
     init_translations(dir_path + "/i18n")
 
 3. Get translation string:
 .. code-block:: python
 
-    from translations import __
-    __("de_DE", "Hello, %user%", {"user": "Alexey"}) # Prints "Hello, Alexey"
+    from translations import translate
+    translate("de_DE", "Hello, %user%", {"user": "Alexey"}) # Prints "Hello, Alexey"
 
 New version release
 --------------------
 
 To release new version:
 1. Update sphinx_integral_theme/__init__.py with new __version__ and __version_info__
 2. Run the following command:
```

