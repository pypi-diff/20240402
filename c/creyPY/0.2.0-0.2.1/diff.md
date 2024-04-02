# Comparing `tmp/creyPY-0.2.0.tar.gz` & `tmp/creyPY-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "creyPY-0.2.0.tar", last modified: Tue Apr  2 09:42:00 2024, max compression
+gzip compressed data, was "creyPY-0.2.1.tar", last modified: Tue Apr  2 10:16:38 2024, max compression
```

## Comparing `creyPY-0.2.0.tar` & `creyPY-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:42:00.828273 creyPY-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-02 09:41:46.000000 creyPY-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-02 09:42:00.828273 creyPY-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 09:41:46.000000 creyPY-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:42:00.824273 creyPY-0.2.0/creyPY/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 09:41:46.000000 creyPY-0.2.0/creyPY/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:42:00.824273 creyPY-0.2.0/creyPY/const/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-02 09:41:46.000000 creyPY-0.2.0/creyPY/const/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-02 09:41:46.000000 creyPY-0.2.0/creyPY/const/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-04-02 09:41:46.000000 creyPY-0.2.0/creyPY/const/i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-02 09:41:46.000000 creyPY-0.2.0/creyPY/const/stripe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:42:00.824273 creyPY-0.2.0/creyPY/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-02 09:41:46.000000 creyPY-0.2.0/creyPY/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-02 09:41:46.000000 creyPY-0.2.0/creyPY/fastapi/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-02 09:41:46.000000 creyPY-0.2.0/creyPY/fastapi/crud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:42:00.824273 creyPY-0.2.0/creyPY/fastapi/models/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 09:41:46.000000 creyPY-0.2.0/creyPY/fastapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-02 09:41:46.000000 creyPY-0.2.0/creyPY/fastapi/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-02 09:41:46.000000 creyPY-0.2.0/creyPY/fastapi/pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:42:00.824273 creyPY-0.2.0/creyPY/fastapi/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 09:41:46.000000 creyPY-0.2.0/creyPY/fastapi/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-02 09:41:46.000000 creyPY-0.2.0/creyPY/fastapi/schemas/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-02 09:41:46.000000 creyPY-0.2.0/creyPY/fastapi/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:42:00.824273 creyPY-0.2.0/creyPY.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-02 09:42:00.000000 creyPY-0.2.0/creyPY.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-02 09:42:00.000000 creyPY-0.2.0/creyPY.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 09:42:00.000000 creyPY-0.2.0/creyPY.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-02 09:42:00.000000 creyPY-0.2.0/creyPY.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 09:42:00.000000 creyPY-0.2.0/creyPY.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 09:42:00.828273 creyPY-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-02 09:41:46.000000 creyPY-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:16:38.105191 creyPY-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-02 10:16:21.000000 creyPY-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-04-02 10:16:38.105191 creyPY-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-02 10:16:21.000000 creyPY-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:16:38.101191 creyPY-0.2.1/creyPY/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 10:16:21.000000 creyPY-0.2.1/creyPY/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:16:38.101191 creyPY-0.2.1/creyPY/const/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-02 10:16:21.000000 creyPY-0.2.1/creyPY/const/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-02 10:16:21.000000 creyPY-0.2.1/creyPY/const/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-04-02 10:16:21.000000 creyPY-0.2.1/creyPY/const/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-02 10:16:21.000000 creyPY-0.2.1/creyPY/const/stripe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:16:38.105191 creyPY-0.2.1/creyPY/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-02 10:16:21.000000 creyPY-0.2.1/creyPY/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-02 10:16:21.000000 creyPY-0.2.1/creyPY/fastapi/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-02 10:16:21.000000 creyPY-0.2.1/creyPY/fastapi/crud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:16:38.105191 creyPY-0.2.1/creyPY/fastapi/db/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 10:16:21.000000 creyPY-0.2.1/creyPY/fastapi/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-02 10:16:21.000000 creyPY-0.2.1/creyPY/fastapi/db/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:16:38.105191 creyPY-0.2.1/creyPY/fastapi/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 10:16:21.000000 creyPY-0.2.1/creyPY/fastapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-02 10:16:21.000000 creyPY-0.2.1/creyPY/fastapi/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-02 10:16:21.000000 creyPY-0.2.1/creyPY/fastapi/pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:16:38.105191 creyPY-0.2.1/creyPY/fastapi/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 10:16:21.000000 creyPY-0.2.1/creyPY/fastapi/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-02 10:16:21.000000 creyPY-0.2.1/creyPY/fastapi/schemas/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-02 10:16:21.000000 creyPY-0.2.1/creyPY/fastapi/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:16:38.105191 creyPY-0.2.1/creyPY.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-04-02 10:16:38.000000 creyPY-0.2.1/creyPY.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-02 10:16:38.000000 creyPY-0.2.1/creyPY.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 10:16:38.000000 creyPY-0.2.1/creyPY.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-02 10:16:38.000000 creyPY-0.2.1/creyPY.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 10:16:38.000000 creyPY-0.2.1/creyPY.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 10:16:38.105191 creyPY-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-02 10:16:21.000000 creyPY-0.2.1/setup.py
```

### Comparing `creyPY-0.2.0/LICENSE` & `creyPY-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `creyPY-0.2.0/creyPY/const/i18n.py` & `creyPY-0.2.1/creyPY/const/i18n.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import enum
 
 
+# Source: https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes
 class CountryEnum(str, enum.Enum):
     AF = "Afghanistan"
     AX = "land Islands"
     AL = "Albania"
     DZ = "Algeria"
     AS = "American Samoa"
     AD = "AndorrA"
@@ -244,14 +245,15 @@
     WF = "Wallis and Futuna"
     EH = "Western Sahara"
     YE = "Yemen"
     ZM = "Zambia"
     ZW = "Zimbabwe"
 
 
+# :: https://en.wikipedia.org/wiki/List_of_ISO_639_language_codes
 class LanguageEnum(str, enum.Enum):
     AA = "Afar"
     AB = "Abkhazian"
     AF = "Afrikaans"
     AK = "Akan"
     AM = "Amharic"
     AN = "Aragonese"
```

### Comparing `creyPY-0.2.0/creyPY/const/stripe.py` & `creyPY-0.2.1/creyPY/const/stripe.py`

 * *Files identical despite different names*

### Comparing `creyPY-0.2.0/creyPY/fastapi/app.py` & `creyPY-0.2.1/creyPY/fastapi/app.py`

 * *Files identical despite different names*

### Comparing `creyPY-0.2.0/creyPY/fastapi/crud.py` & `creyPY-0.2.1/creyPY/fastapi/crud.py`

 * *Files identical despite different names*

### Comparing `creyPY-0.2.0/creyPY/fastapi/models/base.py` & `creyPY-0.2.1/creyPY/fastapi/models/base.py`

 * *Files identical despite different names*

### Comparing `creyPY-0.2.0/creyPY/fastapi/pagination.py` & `creyPY-0.2.1/creyPY/fastapi/pagination.py`

 * *Files identical despite different names*

### Comparing `creyPY-0.2.0/creyPY/fastapi/testing.py` & `creyPY-0.2.1/creyPY/fastapi/testing.py`

 * *Files identical despite different names*

### Comparing `creyPY-0.2.0/creyPY.egg-info/SOURCES.txt` & `creyPY-0.2.1/creyPY.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,11 +12,13 @@
 creyPY/const/i18n.py
 creyPY/const/stripe.py
 creyPY/fastapi/__init__.py
 creyPY/fastapi/app.py
 creyPY/fastapi/crud.py
 creyPY/fastapi/pagination.py
 creyPY/fastapi/testing.py
+creyPY/fastapi/db/__init__.py
+creyPY/fastapi/db/session.py
 creyPY/fastapi/models/__init__.py
 creyPY/fastapi/models/base.py
 creyPY/fastapi/schemas/__init__.py
 creyPY/fastapi/schemas/base.py
```

### Comparing `creyPY-0.2.0/setup.py` & `creyPY-0.2.1/setup.py`

 * *Files identical despite different names*

