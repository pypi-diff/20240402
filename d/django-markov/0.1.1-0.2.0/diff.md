# Comparing `tmp/django_markov-0.1.1.tar.gz` & `tmp/django_markov-0.2.0.tar.gz`

## Comparing `django_markov-0.1.1.tar` & `django_markov-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 django_markov-0.1.1/src/django_markov/__init__.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 django_markov-0.1.1/src/django_markov/admin.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 django_markov-0.1.1/src/django_markov/apps.py
--rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 django_markov-0.1.1/src/django_markov/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_markov-0.1.1/src/django_markov/py.typed
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 django_markov-0.1.1/src/django_markov/text_models.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 django_markov-0.1.1/src/django_markov/urls.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_markov-0.1.1/src/django_markov/views.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 django_markov-0.1.1/src/django_markov/migrations/0001_initial.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 django_markov-0.1.1/src/django_markov/migrations/0002_alter_markovtextmodel_created_and_more.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_markov-0.1.1/src/django_markov/migrations/__init__.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 django_markov-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 django_markov-0.1.1/tests/settings.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 django_markov-0.1.1/tests/test_models.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 django_markov-0.1.1/tests/urls.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 django_markov-0.1.1/.gitignore
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 django_markov-0.1.1/LICENSE
--rw-r--r--   0        0        0     5962 2020-02-02 00:00:00.000000 django_markov-0.1.1/README.md
--rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 django_markov-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6892 2020-02-02 00:00:00.000000 django_markov-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 django_markov-0.2.0/src/django_markov/__init__.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 django_markov-0.2.0/src/django_markov/admin.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 django_markov-0.2.0/src/django_markov/apps.py
+-rw-r--r--   0        0        0    11609 2020-02-02 00:00:00.000000 django_markov-0.2.0/src/django_markov/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_markov-0.2.0/src/django_markov/py.typed
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 django_markov-0.2.0/src/django_markov/text_models.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 django_markov-0.2.0/src/django_markov/urls.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_markov-0.2.0/src/django_markov/views.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 django_markov-0.2.0/src/django_markov/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 django_markov-0.2.0/src/django_markov/migrations/0002_alter_markovtextmodel_created_and_more.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 django_markov-0.2.0/src/django_markov/migrations/0003_markovtextmodel_compiled.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 django_markov-0.2.0/src/django_markov/migrations/0004_remove_markovtextmodel_compiled.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_markov-0.2.0/src/django_markov/migrations/__init__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 django_markov-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 django_markov-0.2.0/tests/settings.py
+-rw-r--r--   0        0        0     7387 2020-02-02 00:00:00.000000 django_markov-0.2.0/tests/test_models.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 django_markov-0.2.0/tests/urls.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 django_markov-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 django_markov-0.2.0/LICENSE
+-rw-r--r--   0        0        0     6638 2020-02-02 00:00:00.000000 django_markov-0.2.0/README.md
+-rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 django_markov-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7568 2020-02-02 00:00:00.000000 django_markov-0.2.0/PKG-INFO
```

### Comparing `django_markov-0.1.1/src/django_markov/text_models.py` & `django_markov-0.2.0/src/django_markov/text_models.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.1.1/src/django_markov/migrations/0001_initial.py` & `django_markov-0.2.0/src/django_markov/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.1.1/src/django_markov/migrations/0002_alter_markovtextmodel_created_and_more.py` & `django_markov-0.2.0/src/django_markov/migrations/0002_alter_markovtextmodel_created_and_more.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.1.1/tests/settings.py` & `django_markov-0.2.0/tests/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -185,7 +185,10 @@
 
 # EMAIL
 # ------------------------------------------------------------------------------
 # https://docs.djangoproject.com/en/dev/ref/settings/#email-backend
 EMAIL_BACKEND = "django.core.mail.backends.locmem.EmailBackend"
 
 MARKOV_CORPUS_MAX_CHAR_LIMIT = env("DJANGO_MARKOV_MAX_CHAR_LIMIT", cast=int, default=0)  # type: ignore
+MARKOV_STORE_COMPILED_MODELS = env.bool(
+    "DJANGO_MARKOV_STORE_COMPILED_MODELS", default=True
+)
```

### Comparing `django_markov-0.1.1/tests/urls.py` & `django_markov-0.2.0/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.1.1/LICENSE` & `django_markov-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_markov-0.1.1/README.md` & `django_markov-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 django-markov is a reusable Django app that enables you to create Markov text models, and store
 them in the database. Those models can then be used to generate Markov chain sentences.
 It relies on the excellent [markovify](https://github.com/jsvine/markovify) by [Jeremy Singer-Vine](https://github.com/jsvine)
 and [spacy](https://spacy.io).
 
 ![PyPI - Version](https://img.shields.io/pypi/v/django-markov)
 ![PyPI - Versions from Framework Classifiers](https://img.shields.io/pypi/frameworkversions/django/django-markov)
+[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Rye](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/rye/main/artwork/badge.json)](https://rye-up.com)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
-![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/andrlik/django-markov/ci.yml)
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/andrlik/django-markov/ci.yml?branch=main)
 [![Coverage Status](https://coveralls.io/repos/github/andrlik/django-markov/badge.svg?branch=main)](https://coveralls.io/github/andrlik/django-markov?branch=main)
 
 
 This project is extracted from [django-quotes](https://github.com/andrlik/django-quotes). Once I realized I needed it for another project, but without
 the quotes, I spent an afternoon splitting it out.
 
 ## Installation
@@ -50,14 +51,22 @@
 ]
 
 # Limit the total size of the corpus. This will result in
 # sentences that are less likely to be sensible, but will improve
 # performance when loading the compiled model from the database.
 # Use 0 for no limit, or specify a character limit.
 MARKOV_CORPUS_MAX_CHAR_LIMIT = 0
+
+# Compile text models by default when writing to database.
+# Compiled models are significantly more performant when
+# generating sentences, but they cannot be chained with other
+# model without parsing the entire corpus again.
+# What's best will depend on your use case. If you don't intend
+# to combine multiple models, you'll want this set to True.
+MARKOV_STORE_COMPILED_MODELS = True
 ```
 
 Then run migrations as usual.
 
 ```bash
 python manage.py migrate
 ```
@@ -102,44 +111,55 @@
 
 async def sentence(text_model: MarkovTextModel, char_limit: int) -> str | None:
     # If the model has no data it will return None instead of a str.
     return await text_model.agenerate_sentence(char_limit=char_limit)
 ```
 
 Every time a sentence is generated the `sentence_generated` signal will be emitted. You
-can use this for things like collecting stats, creating an ongoing log of output, etc.
+can use this for things like collecting stats, creating an ongoing log of output, etc. The
+signal will have the kwargs of:
+
+```python
+from django_markov.models import MarkovTextModel, sentence_generated
+
+text_model = MarkovTextModel.objects.create()
+
+sentence_generated.send(
+    sender=MarkovTextModel,
+    instance=text_model,
+    char_limit=500,
+    sentence="Life is stranger than a monkey riding a unicycle.",
+)
+```
 
 ## Contributing
 
 Pull requests and improvements are welcome! First, familiarize yourself with our
 [Code of Conduct](https://andrlik.github.io/django-markov/code_of_conduct/). You will need to agree to abide by this to have your contribution
 included.
 
-Django apps are often not fond of `src` layout packages.
-To avoid these complications, and to enable debug mode add the following environment variables
+To enable debug mode, add the following environment variable
 using `.envrc` for direnv, a `.env` file or similar.
 
 ```bash
-export DJANGO_SETTINGS_MODULE="tests.settings"
 export DJANGO_DEBUG="True"
-export PYTHONPATH="$PYTHONPATH:$(pwd)"
 ```
 
 We use [just](https://github.com/casey/just) and [Rye](https://rye-up) to manage our project.
 If you don't already have `just` installed, follow the directions on their project page.
 
 Then run our setup command.
 
 ```bash
 just bootstrap
 ```
 
 It will do the following for you:
 
-- Check if you've set the above environment variables.
+- Check if you've set the above environment variable.
 - Check if pre-commit is on your path.
 - Check if Rye is installed, and install it if it is not.
 - Install the pre-commit hooks into your repo.
 - Create your virtualenv with all requirements.
 - Run migrations
 
 Our Justfile can handle a lot of the admin tasks for you without having to worry about
```

### Comparing `django_markov-0.1.1/pyproject.toml` & `django_markov-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-markov"
-version = "0.1.1"
+version = "0.2.0"
 description = "django-markov is a reusable Django app that enables you to create Markov text models, and store them in the database. Those models can then be used to generate Markov chain sentences."
 authors = [
     { name = "Daniel Andrlik", email = "daniel@andrlik.org" }
 ]
 dependencies = [
     "django>=5.0.3",
     "markovify>=0.9.4",
@@ -51,14 +51,17 @@
     # This is so you can develop without relying on pip.
     "en-core-web-trf @ https://github.com/explosion/spacy-models/releases/download/en_core_web_trf-3.7.3/en_core_web_trf-3.7.3-py3-none-any.whl",
     "black>=24.3.0",
     "django-coverage>=1.2.4",
     "django-coverage-plugin>=3.1.0",
     "argon2-cffi>=23.1.0",
     "django-environ>=0.11.2",
+    "django-extensions>=3.2.3",
+    "pytest-mock>=3.14.0",
+    "faker>=24.4.0",
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/django_markov"]
@@ -159,14 +162,15 @@
   # Don't touch unused imports
   "F401",
 ]
 
 [tool.ruff.lint.per-file-ignores]
 "tests/*.py" = ["S101", "FBT001", "ARG001"]
 "tests/urls.py" = ["RUF005"]
+"tests/model_load_timings.py" = ["T201"]
 "conftest.py" = ["ARG001"]
 
 [tool.ruff.lint.isort]
 known-first-party = ["django_markov"]
 
 [tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "all"
@@ -204,15 +208,15 @@
   "--reuse-db"
 ]
 
 [tool.check-wheel-contents]
 ignore = ["W004"]
 
 [tool.bumpversion]
-current_version = "0.1.1"
+current_version = "0.2.0"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = false
 tag = true
```

### Comparing `django_markov-0.1.1/PKG-INFO` & `django_markov-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-markov
-Version: 0.1.1
+Version: 0.2.0
 Summary: django-markov is a reusable Django app that enables you to create Markov text models, and store them in the database. Those models can then be used to generate Markov chain sentences.
 Project-URL: Repository, https://github.com/andrlik/django-markov
 Project-URL: Documentation, https://andrlik.github.io/django-markov
 Project-URL: Homepage, https://andrlik.github.io/django-markov
 Author-email: Daniel Andrlik <daniel@andrlik.org>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
@@ -24,19 +24,20 @@
 django-markov is a reusable Django app that enables you to create Markov text models, and store
 them in the database. Those models can then be used to generate Markov chain sentences.
 It relies on the excellent [markovify](https://github.com/jsvine/markovify) by [Jeremy Singer-Vine](https://github.com/jsvine)
 and [spacy](https://spacy.io).
 
 ![PyPI - Version](https://img.shields.io/pypi/v/django-markov)
 ![PyPI - Versions from Framework Classifiers](https://img.shields.io/pypi/frameworkversions/django/django-markov)
+[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Rye](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/rye/main/artwork/badge.json)](https://rye-up.com)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
-![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/andrlik/django-markov/ci.yml)
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/andrlik/django-markov/ci.yml?branch=main)
 [![Coverage Status](https://coveralls.io/repos/github/andrlik/django-markov/badge.svg?branch=main)](https://coveralls.io/github/andrlik/django-markov?branch=main)
 
 
 This project is extracted from [django-quotes](https://github.com/andrlik/django-quotes). Once I realized I needed it for another project, but without
 the quotes, I spent an afternoon splitting it out.
 
 ## Installation
@@ -71,14 +72,22 @@
 ]
 
 # Limit the total size of the corpus. This will result in
 # sentences that are less likely to be sensible, but will improve
 # performance when loading the compiled model from the database.
 # Use 0 for no limit, or specify a character limit.
 MARKOV_CORPUS_MAX_CHAR_LIMIT = 0
+
+# Compile text models by default when writing to database.
+# Compiled models are significantly more performant when
+# generating sentences, but they cannot be chained with other
+# model without parsing the entire corpus again.
+# What's best will depend on your use case. If you don't intend
+# to combine multiple models, you'll want this set to True.
+MARKOV_STORE_COMPILED_MODELS = True
 ```
 
 Then run migrations as usual.
 
 ```bash
 python manage.py migrate
 ```
@@ -123,44 +132,55 @@
 
 async def sentence(text_model: MarkovTextModel, char_limit: int) -> str | None:
     # If the model has no data it will return None instead of a str.
     return await text_model.agenerate_sentence(char_limit=char_limit)
 ```
 
 Every time a sentence is generated the `sentence_generated` signal will be emitted. You
-can use this for things like collecting stats, creating an ongoing log of output, etc.
+can use this for things like collecting stats, creating an ongoing log of output, etc. The
+signal will have the kwargs of:
+
+```python
+from django_markov.models import MarkovTextModel, sentence_generated
+
+text_model = MarkovTextModel.objects.create()
+
+sentence_generated.send(
+    sender=MarkovTextModel,
+    instance=text_model,
+    char_limit=500,
+    sentence="Life is stranger than a monkey riding a unicycle.",
+)
+```
 
 ## Contributing
 
 Pull requests and improvements are welcome! First, familiarize yourself with our
 [Code of Conduct](https://andrlik.github.io/django-markov/code_of_conduct/). You will need to agree to abide by this to have your contribution
 included.
 
-Django apps are often not fond of `src` layout packages.
-To avoid these complications, and to enable debug mode add the following environment variables
+To enable debug mode, add the following environment variable
 using `.envrc` for direnv, a `.env` file or similar.
 
 ```bash
-export DJANGO_SETTINGS_MODULE="tests.settings"
 export DJANGO_DEBUG="True"
-export PYTHONPATH="$PYTHONPATH:$(pwd)"
 ```
 
 We use [just](https://github.com/casey/just) and [Rye](https://rye-up) to manage our project.
 If you don't already have `just` installed, follow the directions on their project page.
 
 Then run our setup command.
 
 ```bash
 just bootstrap
 ```
 
 It will do the following for you:
 
-- Check if you've set the above environment variables.
+- Check if you've set the above environment variable.
 - Check if pre-commit is on your path.
 - Check if Rye is installed, and install it if it is not.
 - Install the pre-commit hooks into your repo.
 - Create your virtualenv with all requirements.
 - Run migrations
 
 Our Justfile can handle a lot of the admin tasks for you without having to worry about
```

