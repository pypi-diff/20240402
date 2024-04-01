# Comparing `tmp/ugrc-palletjack-4.3.0.tar.gz` & `tmp/ugrc-palletjack-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ugrc-palletjack-4.3.0.tar", last modified: Wed Dec  6 18:32:58 2023, max compression
+gzip compressed data, was "ugrc-palletjack-4.3.1.tar", last modified: Mon Apr  1 22:56:40 2024, max compression
```

## Comparing `ugrc-palletjack-4.3.0.tar` & `ugrc-palletjack-4.3.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 18:32:58.512842 ugrc-palletjack-4.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-12-06 18:32:55.000000 ugrc-palletjack-4.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2023-12-06 18:32:58.512842 ugrc-palletjack-4.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2023-12-06 18:32:55.000000 ugrc-palletjack-4.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      542 2023-12-06 18:32:58.512842 ugrc-palletjack-4.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2023-12-06 18:32:55.000000 ugrc-palletjack-4.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 18:32:58.508842 ugrc-palletjack-4.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 18:32:58.512842 ugrc-palletjack-4.3.0/src/palletjack/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2023-12-06 18:32:55.000000 ugrc-palletjack-4.3.0/src/palletjack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2023-12-06 18:32:55.000000 ugrc-palletjack-4.3.0/src/palletjack/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    45151 2023-12-06 18:32:55.000000 ugrc-palletjack-4.3.0/src/palletjack/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)    38327 2023-12-06 18:32:55.000000 ugrc-palletjack-4.3.0/src/palletjack/load.py
--rw-r--r--   0 runner    (1001) docker     (127)    11372 2023-12-06 18:32:55.000000 ugrc-palletjack-4.3.0/src/palletjack/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)    40397 2023-12-06 18:32:55.000000 ugrc-palletjack-4.3.0/src/palletjack/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2023-12-06 18:32:55.000000 ugrc-palletjack-4.3.0/src/palletjack/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 18:32:58.512842 ugrc-palletjack-4.3.0/src/ugrc_palletjack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2023-12-06 18:32:58.000000 ugrc-palletjack-4.3.0/src/ugrc_palletjack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      513 2023-12-06 18:32:58.000000 ugrc-palletjack-4.3.0/src/ugrc_palletjack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-06 18:32:58.000000 ugrc-palletjack-4.3.0/src/ugrc_palletjack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-12-06 18:32:58.000000 ugrc-palletjack-4.3.0/src/ugrc_palletjack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      392 2023-12-06 18:32:58.000000 ugrc-palletjack-4.3.0/src/ugrc_palletjack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-06 18:32:58.000000 ugrc-palletjack-4.3.0/src/ugrc_palletjack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-06 18:32:58.000000 ugrc-palletjack-4.3.0/src/ugrc_palletjack.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:56:40.130240 ugrc-palletjack-4.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-01 22:56:37.000000 ugrc-palletjack-4.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-04-01 22:56:40.130240 ugrc-palletjack-4.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-01 22:56:37.000000 ugrc-palletjack-4.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-01 22:56:37.000000 ugrc-palletjack-4.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 22:56:40.130240 ugrc-palletjack-4.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-01 22:56:37.000000 ugrc-palletjack-4.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:56:40.126240 ugrc-palletjack-4.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:56:40.126240 ugrc-palletjack-4.3.1/src/palletjack/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-01 22:56:37.000000 ugrc-palletjack-4.3.1/src/palletjack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-01 22:56:37.000000 ugrc-palletjack-4.3.1/src/palletjack/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45152 2024-04-01 22:56:37.000000 ugrc-palletjack-4.3.1/src/palletjack/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38332 2024-04-01 22:56:37.000000 ugrc-palletjack-4.3.1/src/palletjack/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11331 2024-04-01 22:56:37.000000 ugrc-palletjack-4.3.1/src/palletjack/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40269 2024-04-01 22:56:37.000000 ugrc-palletjack-4.3.1/src/palletjack/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-01 22:56:37.000000 ugrc-palletjack-4.3.1/src/palletjack/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:56:40.130240 ugrc-palletjack-4.3.1/src/ugrc_palletjack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-04-01 22:56:40.000000 ugrc-palletjack-4.3.1/src/ugrc_palletjack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-01 22:56:40.000000 ugrc-palletjack-4.3.1/src/ugrc_palletjack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 22:56:40.000000 ugrc-palletjack-4.3.1/src/ugrc_palletjack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 22:56:40.000000 ugrc-palletjack-4.3.1/src/ugrc_palletjack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-01 22:56:40.000000 ugrc-palletjack-4.3.1/src/ugrc_palletjack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-01 22:56:40.000000 ugrc-palletjack-4.3.1/src/ugrc_palletjack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 22:56:40.000000 ugrc-palletjack-4.3.1/src/ugrc_palletjack.egg-info/zip-safe
```

### Comparing `ugrc-palletjack-4.3.0/LICENSE` & `ugrc-palletjack-4.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ugrc-palletjack-4.3.0/PKG-INFO` & `ugrc-palletjack-4.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: ugrc-palletjack
-Version: 4.3.0
+Version: 4.3.1
 Summary: Updating AGOL feature services with data from external tables.
 Home-page: https://github.com/agrc/palletjack
 Author: Jake Adams, UGRC
 Author-email: jdadams@utah.gov
-License: UNKNOWN
 Project-URL: Issue Tracker, https://github.com/agrc/palletjack/issues
 Keywords: gis
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
@@ -95,9 +93,7 @@
 The github pages are served from the `gh-pages` branch. After you make edits to the code and update the docstrings, rebase this branch onto the updated `main` branch. To prevent github pages from trying to generate a site from the contents of `docs/palletjack` with jekyll, add a `.nojekyll` file to `docs/palletjack`.
 
 To generate the docs, run `pdoc --html -o docs\ c:\palletjack\repo\src\palletjack --force`. The code's docstrings should be Google-style docstrings with proper indentation to ensure the argument lists, etc are parsed and displayed correctly.
 
 `docs/README.md` is included at the top package level by adding the line `.. include:: ../../docs/README.md` in `__init__.py`'s docstring. This tells pdoc to insert that markdown into the HTML generated for that docstring, and the include directive can be used for more in-depth documentation anywhere else as well. Note that `pdoc` tries to create links for anything surrounded by backticks, which are also used for code blocks. You may need to manually edit the HTML to remove the links if they change the content of your code blocks (such as in the example import statement).
 
 Once the contents of `docs/palletjack` look correct, force push the `gh-pages` branch to github. This will trigger the action to republish the site. The docs are then accessible at [agrc.github.io/palletjack/palletjack/index.html].
-
-
```

### Comparing `ugrc-palletjack-4.3.0/README.md` & `ugrc-palletjack-4.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ugrc-palletjack-4.3.0/setup.py` & `ugrc-palletjack-4.3.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,67 +5,67 @@
 A module that installs palletjack as a module
 """
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 version = {}
-with open('src/palletjack/version.py', encoding='utf-8') as fp:
+with open("src/palletjack/version.py", encoding="utf-8") as fp:
     exec(fp.read(), version)
 
 setup(
-    name='ugrc-palletjack',
-    version=version['__version__'],
-    description='Updating AGOL feature services with data from external tables.',
-    long_description=(Path(__file__).parent / 'README.md').read_text(),
-    long_description_content_type='text/markdown',
-    author='Jake Adams, UGRC',
-    author_email='jdadams@utah.gov',
-    url='https://github.com/agrc/palletjack',
-    packages=find_packages('src'),
-    package_dir={'': 'src'},
+    name="ugrc-palletjack",
+    version=version["__version__"],
+    description="Updating AGOL feature services with data from external tables.",
+    long_description=(Path(__file__).parent / "README.md").read_text(),
+    long_description_content_type="text/markdown",
+    author="Jake Adams, UGRC",
+    author_email="jdadams@utah.gov",
+    url="https://github.com/agrc/palletjack",
+    packages=find_packages("src"),
+    package_dir={"": "src"},
     include_package_data=True,
     zip_safe=True,
     classifiers=[
         # complete classifier list: http://pypi.python.org/pypi?%3Aaction=list_classifiers
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Topic :: Utilities',
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Topic :: Utilities",
     ],
     project_urls={
-        'Issue Tracker': 'https://github.com/agrc/palletjack/issues',
+        "Issue Tracker": "https://github.com/agrc/palletjack/issues",
     },
-    keywords=['gis'],
+    keywords=["gis"],
     install_requires=[
-        'arcgis==2.2.*',
-        'geopandas==0.14.*',
-        'pg8000>=1.29,<1.31',
-        'psycopg2-binary==2.9.*',
-        'pygsheets==2.0.*',
-        'pyogrio>=0.6,<0.8',
-        'pysftp==0.2.9',
-        'SQLAlchemy>=1.4,<2.1',
+        "arcgis>=2.2,<2.3",
+        "geopandas==0.14.*",
+        "pg8000>=1.29,<1.32",
+        "psycopg2-binary==2.9.*",
+        "pygsheets==2.0.*",
+        "pyogrio>=0.6,<0.8",
+        "pysftp==0.2.9",
+        "SQLAlchemy>=1.4,<2.1",
     ],
     extras_require={
-        'tests': [
-            'pdoc3==0.10.*',
-            'pylint-quotes==0.2.*',
-            'pylint>=2.15,<3.1',
-            'pytest-cov>=4.0,<4.2',
-            'pytest-instafail>=0.4,<0.6',
-            'pytest-isort==3.1.*',
-            'pytest-mock>=3.10,<3.13',
-            'pytest-pylint>=0.20,<0.22',
-            'pytest-watch==4.2.*',
-            'pytest==7.*',
-            'requests-mock==1.*',
-            'yapf>=0.32,<0.41',
+        "tests": [
+            "pdoc3==0.10.*",
+            "pytest-cov>=3,<6",
+            "pytest-instafail~=0.4",
+            "pytest-mock>=3.10,<3.15",
+            "pytest-ruff==0.*",
+            "pytest-watch~=4.2",
+            "pytest>=6,<9",
+            "black>=23.3,<24.4",
+            "requests-mock==1.*",
+            "ruff==0.0.*",
         ]
     },
     setup_requires=[
-        'pytest-runner',
+        "pytest-runner",
     ],
-    entry_points={'console_scripts': [
-        'palletjack = palletjack.example:process',
-    ]},
+    entry_points={
+        "console_scripts": [
+            "palletjack = palletjack.example:process",
+        ]
+    },
 )
```

### Comparing `ugrc-palletjack-4.3.0/src/palletjack/__init__.py` & `ugrc-palletjack-4.3.1/src/palletjack/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """A library for extracting tabular/spatial data from many different sources, transforming it to meet ArcGIS Online hosted feature service requirements, and loading it into existing feature services.
 
 .. include:: ../../docs/README.md
 """
+
 import locale
 
-from . import extract, load, transform, utils
-from .errors import IntFieldAsFloatError, TimezoneAwareDatetimeError
+from . import extract, load, transform, utils  # noqa: F401
+from .errors import IntFieldAsFloatError, TimezoneAwareDatetimeError  # noqa: F401
 
 #: If the locale is not set explicitly, set it to the system default for text to number conversions
 if not locale.getlocale(locale.LC_NUMERIC)[0]:
     locale.setlocale(locale.LC_NUMERIC, locale.getlocale())
```

### Comparing `ugrc-palletjack-4.3.0/src/palletjack/extract.py` & `ugrc-palletjack-4.3.1/src/palletjack/extract.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,35 +58,35 @@
             worksheet (int or str): Zero-based index of the worksheet or the worksheet title
             by_title (bool, optional): Search for worksheet by title instead of index. Defaults to False.
 
         Returns:
             pd.DataFrame: The specified worksheet as a data frame.
         """
 
-        self._class_logger.debug('Loading sheet ID %s', sheet_id)
+        self._class_logger.debug("Loading sheet ID %s", sheet_id)
         sheet = self.gsheets_client.open_by_key(sheet_id)
 
         if by_title:
-            self._class_logger.debug('Loading worksheet by title %s', worksheet)
+            self._class_logger.debug("Loading worksheet by title %s", worksheet)
             return sheet.worksheet_by_title(worksheet).get_as_df()
         else:
-            self._class_logger.debug('Loading worksheet by index %s', worksheet)
-            return sheet.worksheet('index', worksheet).get_as_df()
+            self._class_logger.debug("Loading worksheet by index %s", worksheet)
+            return sheet.worksheet("index", worksheet).get_as_df()
 
     def load_all_worksheets_into_dataframes(self, sheet_id):
         """Load all worksheets into a dictionary of dataframes. Keys are the worksheet.
 
         Args:
             sheet_id (str): The ID of the sheet (long alpha-numeric unique ID)
 
         Returns:
             dict: {'worksheet_name': Worksheet as a dataframe}
         """
 
-        self._class_logger.debug('Loading sheet ID %s', sheet_id)
+        self._class_logger.debug("Loading sheet ID %s", sheet_id)
         sheet = self.gsheets_client.open_by_key(sheet_id)
 
         worksheet_dfs = {worksheet.title: worksheet.get_as_df() for worksheet in sheet.worksheets()}
 
         return worksheet_dfs
 
     def combine_worksheets_into_single_dataframe(self, worksheet_dfs):
@@ -105,19 +105,19 @@
                 came from. The row index is the original row numbers and is probably not unique.
         """
 
         dataframes = list(worksheet_dfs.values())
 
         #: Make sure all the dataframes have the same columns
         if not all([set(dataframes[0].columns) == set(df.columns) for df in dataframes]):
-            raise ValueError('Columns do not match; cannot create multi-index dataframe')
+            raise ValueError("Columns do not match; cannot create multi-index dataframe")
 
-        self._class_logger.debug('Concatting worksheet dataframes %s into a single dataframe', worksheet_dfs.keys())
-        concatted_df = pd.concat(dataframes, keys=worksheet_dfs.keys(), names=['worksheet', 'row'])
-        return concatted_df.reset_index(level='worksheet')
+        self._class_logger.debug("Concatting worksheet dataframes %s into a single dataframe", worksheet_dfs.keys())
+        concatted_df = pd.concat(dataframes, keys=worksheet_dfs.keys(), names=["worksheet", "row"])
+        return concatted_df.reset_index(level="worksheet")
 
 
 class GoogleDriveDownloader:
     """Provides methods to download any non-html file (ie, Content-Type != text/html) Google Drive file from it's
     sharing link (of the form `https://drive.google.com/file/d/big_long_id/etc`). The files may be publicly shared or shared with a service account.
 
     This class has two similar sets of methods. The `*_using_api` methods authenticate to the Google API using either a
@@ -127,37 +127,37 @@
 
     def __init__(self, out_dir):
         """
         Args:
             out_dir (str or Path): Directory to save downloaded files. Can be reassigned later to change the directory.
         """
         self._class_logger = logging.getLogger(__name__).getChild(self.__class__.__name__)
-        self._class_logger.debug('Initializing GoogleDriveDownloader')
-        self._class_logger.debug('Output directory: %s', out_dir)
+        self._class_logger.debug("Initializing GoogleDriveDownloader")
+        self._class_logger.debug("Output directory: %s", out_dir)
         self.out_dir = Path(out_dir)
-        regex_pattern = '(\/|=)([-\w]{25,})'  # pylint:disable=anomalous-backslash-in-string
-        self._class_logger.debug('Regex pattern: %s', regex_pattern)
+        regex_pattern = "(\/|=)([-\w]{25,})"  # pylint:disable=anomalous-backslash-in-string
+        self._class_logger.debug("Regex pattern: %s", regex_pattern)
         self.regex = re.compile(regex_pattern)
 
     @staticmethod
     def _save_response_content(response, destination, chunk_size=32768):
         """Download streaming response content in chunks
 
         Args:
             response (requests.response): The response object from the requests .get call
             destination (Path): File path to write to
             chunk_size (int, optional): Download the file in chunks of this size. Defaults to 32768.
         """
 
-        with destination.open(mode='wb') as out_file:
+        with destination.open(mode="wb") as out_file:
             for chunk in response.iter_content(chunk_size):
                 if chunk:  # filter out keep-alive new chunks
                     out_file.write(chunk)
 
-    def _get_http_response(self, file_id, base_url='https://docs.google.com/uc?export=download'):
+    def _get_http_response(self, file_id, base_url="https://docs.google.com/uc?export=download"):
         """Performs the HTTP GET request and checks the response
 
         Args:
             file_id (str): The Google-created unique id for the file
             base_url (str, optional): The base URL for the GET call. Defaults to 'https://docs.google.com/uc?
                 export=download'.
 
@@ -165,19 +165,19 @@
             RuntimeError: If Content-Type is text/html, we can't get the file, either because it doesn't exist or isn't
                 publicly shared.
 
         Returns:
             request.response: The requests response object.
         """
 
-        response = requests.get(base_url, params={'id': file_id}, stream=True)
+        response = requests.get(base_url, params={"id": file_id}, stream=True)
 
-        if 'text/html' in response.headers['Content-Type']:
+        if "text/html" in response.headers["Content-Type"]:
             self._class_logger.error(response.headers)
-            raise RuntimeError(f'Cannot access {file_id} (is it publicly shared?). Response header in log.')
+            raise RuntimeError(f"Cannot access {file_id} (is it publicly shared?). Response header in log.")
 
         return response
 
     @staticmethod
     def _get_filename_from_response(response):
         """Get the filename from the response header
 
@@ -187,22 +187,24 @@
         Raises:
             ValueError: If it can't find the filename in the header
 
         Returns:
             str: Filename as defined in the header
         """
 
-        content = response.headers['Content-Disposition']
-        all_filenames = re.findall('filename\*?=([^;]+)', content, flags=re.IGNORECASE)  # pylint:disable=anomalous-backslash-in-string
+        content = response.headers["Content-Disposition"]
+        all_filenames = re.findall(
+            "filename\*?=([^;]+)", content, flags=re.IGNORECASE
+        )  # pylint:disable=anomalous-backslash-in-string
         if all_filenames:
             #: Remove spurious whitespace and "s
             return all_filenames[0].strip().strip('"')
 
         #: If we don't return a filename, raise an error instead
-        raise ValueError('filename not found in response header')
+        raise ValueError("filename not found in response header")
 
     def _get_file_id_from_sharing_link(self, sharing_link):
         """Use regex to parse out the unique Google id from the sharing link
 
         Args:
             sharing_link (str): The public sharing link to the file
 
@@ -216,18 +218,18 @@
 
         match = self.regex.search(sharing_link)
         if match:
             try:
                 return match.group(2)
             #: Not sure how this would happen (can't even figure out a test), but leaving in for safety.
             except IndexError as err:
-                raise IndexError(f'Regex could not extract the file id from sharing link {sharing_link}') from err
-        raise RuntimeError(f'Regex could not match sharing link {sharing_link}')
+                raise IndexError(f"Regex could not extract the file id from sharing link {sharing_link}") from err
+        raise RuntimeError(f"Regex could not match sharing link {sharing_link}")
 
-    def download_file_from_google_drive(self, sharing_link, join_id, pause=0.):
+    def download_file_from_google_drive(self, sharing_link, join_id, pause=0.0):
         """Download a publicly-shared image from Google Drive using it's sharing link
 
         Uses an anonymous HTTP request with support for sleeping between downloads to try to get around Google's
         blocking (I haven't found a good value yet).
 
         Logs a warning if the URL doesn't match the proper pattern or it can't extract the unique id from the sharing
         URL. Will also log a warning if the header's Content-Type is text/html, which usually indicates the HTTP
@@ -239,31 +241,31 @@
             pause (flt, optional): Pause the specified number of seconds before downloading. Defaults to 0.
 
         Returns:
             Path: Path of downloaded file or None if download fails/is not possible
         """
 
         if pause:
-            self._class_logger.debug('Sleeping for %s', pause)
+            self._class_logger.debug("Sleeping for %s", pause)
         sleep(pause)
         if not sharing_link:
-            self._class_logger.debug('Row %s has no attachment info', join_id)
+            self._class_logger.debug("Row %s has no attachment info", join_id)
             return None
-        self._class_logger.debug('Row %s: downloading shared file %s', join_id, sharing_link)
+        self._class_logger.debug("Row %s: downloading shared file %s", join_id, sharing_link)
         try:
             file_id = self._get_file_id_from_sharing_link(sharing_link)
-            self._class_logger.debug('Row %s: extracted file id %s', join_id, file_id)
+            self._class_logger.debug("Row %s: extracted file id %s", join_id, file_id)
             response = self._get_http_response(file_id)
             filename = self._get_filename_from_response(response)
             out_file_path = self.out_dir / filename
-            self._class_logger.debug('Row %s: writing to %s', join_id, out_file_path)
+            self._class_logger.debug("Row %s: writing to %s", join_id, out_file_path)
             self._save_response_content(response, out_file_path)
             return out_file_path
         except Exception as err:
-            self._class_logger.warning('Row %s: Couldn\'t download %s', join_id, sharing_link)
+            self._class_logger.warning("Row %s: Couldn't download %s", join_id, sharing_link)
             self._class_logger.warning(err)
             return None
 
     def _get_request_and_filename_from_drive_api(self, client, file_id):
         """Get the request object and filename from a Google drive file_id. Will try to determine extension if missing.
 
         Args:
@@ -272,23 +274,23 @@
 
         Returns:
             (googleapiclient.http.HttpRequest, str): Result of the .get_media() call, name of the file
         """
 
         get_media_request = client.drive.service.files().get_media(fileId=file_id)  # pylint:disable=no-member
         metadata = client.drive.service.files().get(fileId=file_id).execute()  # pylint:disable=no-member
-        filename = metadata['name']
+        filename = metadata["name"]
         if not Path(filename).suffix:
             try:
-                filename = filename + mimetypes.guess_extension(metadata['mimeType'])
+                filename = filename + mimetypes.guess_extension(metadata["mimeType"])
             except KeyError:
-                self._class_logger.warning('%s: No MIME type in drive info, file extension not set', file_id)
+                self._class_logger.warning("%s: No MIME type in drive info, file extension not set", file_id)
             except TypeError:
                 self._class_logger.warning(
-                    '%s: Unable to determine file extension from MIME type, file extension not set', file_id
+                    "%s: Unable to determine file extension from MIME type, file extension not set", file_id
                 )
 
         return get_media_request, filename
 
     def _save_get_media_content(self, request, out_file_path):
         """Save the binary data referenced from a .get_media() call to out_file_path
 
@@ -301,15 +303,15 @@
         downloader = MediaIoBaseDownload(in_memory, request)
         done = False
         while not done:
             _, done = downloader.next_chunk()
         out_file_path.write_bytes(in_memory.getbuffer())
 
     def download_file_from_google_drive_using_api(self, gsheets_client, sharing_link, join_id):
-        """ Download a file using the Google API via pygsheets authentication.
+        """Download a file using the Google API via pygsheets authentication.
 
         Requires a pygsheets client object that handles authentication.
 
         Logs a warning if the URL doesn't match the proper pattern or it can't extract the unique id from the sharing
         URL. Will also log a warning if the header's Content-Type is text/html, which usually indicates the HTTP
         response was an error message instead of the file.
 
@@ -318,29 +320,29 @@
             sharing_link (str): Sharing link to the file to be downloaded
             join_id (str or int): Unique key for the row (used for reporting)
 
         Returns:
             Path: Path of downloaded file or None if download fails/is not possible
         """
         if not sharing_link:
-            self._class_logger.debug('Row %s has no attachment info', join_id)
+            self._class_logger.debug("Row %s has no attachment info", join_id)
             return None
-        self._class_logger.debug('Row %s: downloading file %s', join_id, sharing_link)
+        self._class_logger.debug("Row %s: downloading file %s", join_id, sharing_link)
         try:
             file_id = self._get_file_id_from_sharing_link(sharing_link)
-            self._class_logger.debug('Row %s: extracted file id %s', join_id, file_id)
+            self._class_logger.debug("Row %s: extracted file id %s", join_id, file_id)
             get_media_request, filename = utils.retry(
                 self._get_request_and_filename_from_drive_api, gsheets_client, file_id
             )
             out_file_path = self.out_dir / filename
-            self._class_logger.debug('Row %s: writing to %s', join_id, out_file_path)
+            self._class_logger.debug("Row %s: writing to %s", join_id, out_file_path)
             utils.retry(self._save_get_media_content, get_media_request, out_file_path)
             return out_file_path
         except Exception as err:
-            self._class_logger.warning('Row %s: Couldn\'t download %s', join_id, sharing_link)
+            self._class_logger.warning("Row %s: Couldn't download %s", join_id, sharing_link)
             self._class_logger.warning(err)
             return None
 
     def download_attachments_from_dataframe(self, dataframe, sharing_link_column, join_id_column, output_path_column):
         """Download the attachments linked in a dataframe column, creating a new column with the resulting path
 
         Args:
@@ -378,22 +380,21 @@
             pd.DataFrame: Input dataframe with output path info
         """
 
         client = utils.authorize_pygsheets(credentials)
 
         dataframe[output_path_column] = dataframe.apply(
             lambda x: self.download_file_from_google_drive_using_api(client, x[sharing_link_column], x[join_id_column]),
-            axis=1
+            axis=1,
         )
         return dataframe
 
 
 class SFTPLoader:
-    """Loads data from an SFTP share into a pandas DataFrame
-    """
+    """Loads data from an SFTP share into a pandas DataFrame"""
 
     def __init__(self, host, username, password, knownhosts_file, download_dir):
         """
         Args:
             host (str): The SFTP host to connect to
             username (str): SFTP username
             password (str): SFTP password
@@ -404,38 +405,38 @@
         self.host = host
         self.username = username
         self.password = password
         self.knownhosts_file = knownhosts_file
         self.download_dir = download_dir
         self._class_logger = logging.getLogger(__name__).getChild(self.__class__.__name__)
 
-    def download_sftp_folder_contents(self, sftp_folder='upload'):
+    def download_sftp_folder_contents(self, sftp_folder="upload"):
         """Download all files in sftp_folder to the SFTPLoader's download_dir
 
         Args:
             sftp_folder (str, optional): Path of remote folder, relative to sftp home directory. Defaults to 'upload'.
         """
 
-        self._class_logger.info('Downloading files from `%s:%s` to `%s`', self.host, sftp_folder, self.download_dir)
+        self._class_logger.info("Downloading files from `%s:%s` to `%s`", self.host, sftp_folder, self.download_dir)
         starting_file_count = len(list(self.download_dir.iterdir()))
-        self._class_logger.debug('SFTP Username: %s', self.username)
+        self._class_logger.debug("SFTP Username: %s", self.username)
         connection_opts = pysftp.CnOpts(knownhosts=self.knownhosts_file)
         with pysftp.Connection(
             self.host, username=self.username, password=self.password, cnopts=connection_opts
         ) as sftp:
             try:
                 sftp.get_d(sftp_folder, self.download_dir, preserve_mtime=True)
             except FileNotFoundError as error:
-                raise FileNotFoundError(f'Folder `{sftp_folder}` not found on SFTP server') from error
+                raise FileNotFoundError(f"Folder `{sftp_folder}` not found on SFTP server") from error
         downloaded_file_count = len(list(self.download_dir.iterdir())) - starting_file_count
         if not downloaded_file_count:
-            raise ValueError('No files downloaded')
+            raise ValueError("No files downloaded")
         return downloaded_file_count
 
-    def download_sftp_single_file(self, filename, sftp_folder='upload'):
+    def download_sftp_single_file(self, filename, sftp_folder="upload"):
         """Download filename into SFTPLoader's download_dir
 
         Args:
             filename (str): Filename to download; used as output filename as well.
             sftp_folder (str, optional): Path of remote folder, relative to sftp home directory. Defaults to 'upload'.
 
         Raises:
@@ -443,51 +444,51 @@
 
         Returns:
             Path: Downloaded file's path
         """
 
         outfile = Path(self.download_dir, filename)
 
-        self._class_logger.info('Downloading %s from `%s:%s` to `%s`', filename, self.host, sftp_folder, outfile)
-        self._class_logger.debug('SFTP Username: %s', self.username)
+        self._class_logger.info("Downloading %s from `%s:%s` to `%s`", filename, self.host, sftp_folder, outfile)
+        self._class_logger.debug("SFTP Username: %s", self.username)
         connection_opts = pysftp.CnOpts(knownhosts=self.knownhosts_file)
         try:
             with pysftp.Connection(
                 self.host,
                 username=self.username,
                 password=self.password,
                 cnopts=connection_opts,
                 default_path=sftp_folder,
             ) as sftp:
                 sftp.get(filename, localpath=outfile, preserve_mtime=True)
         except FileNotFoundError as error:
-            raise FileNotFoundError(f'File `{filename}` or folder `{sftp_folder}`` not found on SFTP server') from error
+            raise FileNotFoundError(f"File `{filename}` or folder `{sftp_folder}`` not found on SFTP server") from error
 
         return outfile
 
     def read_csv_into_dataframe(self, filename, column_types=None):
         """Read filename into a dataframe with optional column names and types
 
         Args:
             filename (str): Name of file in the SFTPLoader's download_dir
             column_types (dict, optional): Column names and their dtypes(np.float64, str, etc). Defaults to None.
 
         Returns:
             pd.DataFrame: CSV as a pandas dataframe
         """
 
-        self._class_logger.info('Reading `%s` into dataframe', filename)
+        self._class_logger.info("Reading `%s` into dataframe", filename)
         filepath = Path(self.download_dir, filename)
         column_names = None
         if column_types:
             column_names = list(column_types.keys())
         dataframe = pd.read_csv(filepath, names=column_names, dtype=column_types)
-        self._class_logger.debug('Dataframe shape: %s', dataframe.shape)
+        self._class_logger.debug("Dataframe shape: %s", dataframe.shape)
         if len(dataframe.index) == 0:
-            self._class_logger.warning('Dataframe contains no rows. Shape: %s', dataframe.shape)
+            self._class_logger.warning("Dataframe contains no rows. Shape: %s", dataframe.shape)
         return dataframe
 
 
 class PostgresLoader:
     """Loads data from a Postgres/PostGIS database into a pandas data frame"""
 
     def __init__(self, host, database, username, password, port=5432):
@@ -497,30 +498,30 @@
             database (str): Database to connect to
             username (str): Database user
             password (str): Database password
             port (int, optional): Database port. Defaults to 5432.
         """
 
         self._class_logger = logging.getLogger(__name__).getChild(self.__class__.__name__)
-        if os.environ.get('FUNCTION_TARGET') is not None:  #: this is an env var specific to cloud functions
-            self._class_logger.info('running in GCF, using unix socket')
+        if os.environ.get("FUNCTION_TARGET") is not None:  #: this is an env var specific to cloud functions
+            self._class_logger.info("running in GCF, using unix socket")
             self.engine = sqlalchemy.create_engine(
                 sqlalchemy.engine.url.URL.create(
-                    drivername='postgresql+pg8000',
+                    drivername="postgresql+pg8000",
                     username=username,
                     password=password,
                     database=database,
-                    query={'unix_sock': f'/cloudsql/{host}/.s.PGSQL.{port}'},  #: requires the pg8000 package
+                    query={"unix_sock": f"/cloudsql/{host}/.s.PGSQL.{port}"},  #: requires the pg8000 package
                 )
             )
         else:
-            self._class_logger.info('running locally, using traditional host connection')
+            self._class_logger.info("running locally, using traditional host connection")
             self.engine = sqlalchemy.create_engine(
                 sqlalchemy.engine.url.URL.create(
-                    drivername='postgresql',
+                    drivername="postgresql",
                     username=username,
                     password=password,
                     database=database,
                     host=host,
                     port=port,
                 )
             )
@@ -534,28 +535,28 @@
             crs (str): Coordinate reference system of the table's geometry column
             spatial_column (str): Name of the table's geometry or geography column
 
         Returns:
             pd.DataFrame.spatial: Table as a spatially enabled dataframe
         """
 
-        self._class_logger.info('Reading `%s` into dataframe', table_name)
+        self._class_logger.info("Reading `%s` into dataframe", table_name)
 
         dataframe = gpd.read_postgis(
-            f'select * from {table_name}', self.engine, index_col=index_column, crs=crs, geom_col=spatial_column
+            f"select * from {table_name}", self.engine, index_col=index_column, crs=crs, geom_col=spatial_column
         )
 
         spatial_dataframe = pd.DataFrame.spatial.from_geodataframe(dataframe, column_name=spatial_column)
-        for column in spatial_dataframe.select_dtypes(include=['datetime64[ns, UTC]']):
-            self._class_logger.debug('Converting column `%s` to ISO string format', column)
+        for column in spatial_dataframe.select_dtypes(include=["datetime64[ns, UTC]"]):
+            self._class_logger.debug("Converting column `%s` to ISO string format", column)
             spatial_dataframe[column] = spatial_dataframe[column].apply(pd.Timestamp.isoformat)
 
-        self._class_logger.debug('Dataframe shape: %s', spatial_dataframe.shape)
+        self._class_logger.debug("Dataframe shape: %s", spatial_dataframe.shape)
         if len(spatial_dataframe.index) == 0:
-            self._class_logger.warning('Dataframe contains no rows. Shape: %s', spatial_dataframe.shape)
+            self._class_logger.warning("Dataframe contains no rows. Shape: %s", spatial_dataframe.shape)
 
         return spatial_dataframe
 
 
 class RESTServiceLoader:
     """Downloads features from a layer within a map service or feature service (with queries enabled) based on its REST
     endpoint.
@@ -571,15 +572,15 @@
         """Create a representation of a REST FeatureService or MapService
 
         Args:
             service_url (str): The service's REST endpoint
             timeout (int, optional): Timeout for HTTP requests in seconds. Defaults to 5.
         """
 
-        if service_url[-1] == '/':
+        if service_url[-1] == "/":
             service_url = service_url[:-1]
         self.url = service_url
         self.timeout = timeout
 
         self._class_logger = logging.getLogger(__name__).getChild(self.__class__.__name__)
 
     def get_features(self, service_layer, chunk_size=100):
@@ -598,38 +599,40 @@
             chunk_size (int, optional): Number of features to download per chunk. Defaults to 100. If set to None, it
                 will use the service's maxRecordCount. Adjust if the service is failing frequently.
 
         Returns:
             pd.DataFrame.spatial: The service's features as a spatially-enabled dataframe
         """
 
-        self._class_logger.info('Getting features from %s...', service_layer.layer_url)
-        self._class_logger.debug('Checking for query capability...')
-        service_layer.check_capabilities('query')
+        self._class_logger.info("Getting features from %s...", service_layer.layer_url)
+        self._class_logger.debug("Checking for query capability...")
+        service_layer.check_capabilities("query")
         max_record_count = chunk_size
         if not max_record_count:
-            self._class_logger.debug('Getting max record count...')
+            self._class_logger.debug("Getting max record count...")
             max_record_count = service_layer.max_record_count
-        self._class_logger.debug('Getting object ids...')
+        self._class_logger.debug("Getting object ids...")
         oids = utils.retry(service_layer.get_object_ids)
 
         if len(oids) == 0:
-            warnings.warn(f'Layer {service_layer.layer_url} has no features')
+            warnings.warn(f"Layer {service_layer.layer_url} has no features")
             return None
 
-        self._class_logger.debug('Downloading %s features in chunks of %s...', len(oids), max_record_count)
+        self._class_logger.debug("Downloading %s features in chunks of %s...", len(oids), max_record_count)
         all_features_df = pd.DataFrame()
         for oid_subset in utils.chunker(oids, max_record_count):
             # sleep between 1.5 and 3 s to be friendly
             time.sleep(random.randint(150, 300) / 100)
-            all_features_df = pd.concat([
-                all_features_df,
-                utils.retry(service_layer.get_unique_id_list_as_dataframe, service_layer.oid_field, oid_subset)
-            ],
-                                        ignore_index=True)
+            all_features_df = pd.concat(
+                [
+                    all_features_df,
+                    utils.retry(service_layer.get_unique_id_list_as_dataframe, service_layer.oid_field, oid_subset),
+                ],
+                ignore_index=True,
+            )
         #: if you don't do ignore_index=True, the index won't be unique and this will trip up esri's spatial dataframe
         #: which tries calling [geom_col][0] to determine the geometry type, which then returns a series instead of a
         #: single value because the index isn't unique
 
         return all_features_df
 
     def get_feature_layers_info(self):
@@ -645,37 +648,37 @@
             dict: The parsed JSON info of the service's feature layers
         """
 
         response = utils.retry(self._get_service_info)
 
         try:
             response_json = response.json()
-        except (json.JSONDecodeError) as error:
-            raise RuntimeError(f'Could not parse response from {self.url}') from error
+        except json.JSONDecodeError as error:
+            raise RuntimeError(f"Could not parse response from {self.url}") from error
 
         try:
-            layers = [layer for layer in response_json['layers'] if layer['type'] in ['Feature Layer', 'Table']]
+            layers = [layer for layer in response_json["layers"] if layer["type"] in ["Feature Layer", "Table"]]
         except KeyError as error:
-            if 'layers' in str(error):
-                raise RuntimeError(f'Response from {self.url} does not contain layer information') from error
-            raise RuntimeError('Layer info did not contain layer type') from error
+            if "layers" in str(error):
+                raise RuntimeError(f"Response from {self.url} does not contain layer information") from error
+            raise RuntimeError("Layer info did not contain layer type") from error
 
         return layers
 
     def _get_service_info(self):
         """Get the basic info from the service's REST endpoint
 
         Raises:
             requests.HTTPError: If the response returns a status code considered an error
 
         Returns:
             requests.Response: Raw response object from a /query request.
         """
-        self._class_logger.debug('Getting service information...')
-        response = requests.get(f'{self.url}/query', params={'f': 'json'}, timeout=self.timeout)
+        self._class_logger.debug("Getting service information...")
+        response = requests.get(f"{self.url}/query", params={"f": "json"}, timeout=self.timeout)
 
         response.raise_for_status()
 
         return response
 
 
 class ServiceLayer:
@@ -684,15 +687,15 @@
     The methods in this object represent the individual steps of a more complete download process involving sanity
     checks, getting the list of unique IDs to download, and then downloading based on those unique IDS. Any queries,
     where clauses, or subsetting can be done by specifying the envelope_params, feature_params, and/or where_clause to
     limit the unique IDs used to download the features. The get_features method in the RESTServiceLoader class handles
     all of these steps and should be used instead of calling the methods in this class directly.
     """
 
-    def __init__(self, layer_url, timeout=5, envelope_params=None, feature_params=None, where_clause='1=1'):
+    def __init__(self, layer_url, timeout=5, envelope_params=None, feature_params=None, where_clause="1=1"):
         """Create an object representing a single layer
 
         Args:
             layer_url (str): The full URL to the desired layer
             timeout (int, optional): Timeout for HTTP requests in seconds. Defaults to 5.
             envelope_params (dict, optional): Bounding box and it's spatial reference to spatially limit feature
                 collection in the form {'geometry': '{xmin},{ymin},{xmax},{ymax}', 'inSR': '{wkid}'}. Defaults to None.
@@ -701,36 +704,36 @@
                 'true'. See the ArcGIS REST API documentation for more information.
             where_clause (str, optional): Where clause to refine the features returned. Defaults to '1=1'.
 
         """
 
         self._class_logger = logging.getLogger(__name__).getChild(self.__class__.__name__)
 
-        if layer_url[-1] == '/':
+        if layer_url[-1] == "/":
             layer_url = layer_url[:-1]
         self.layer_url = layer_url
         self.timeout = timeout
 
         self.layer_properties_json = self._get_layer_info()
-        self.max_record_count = self.layer_properties_json['maxRecordCount']
+        self.max_record_count = self.layer_properties_json["maxRecordCount"]
         self.oid_field = self._get_object_id_field()
         self._check_layer_type()
 
         self.envelope_params = None
         if envelope_params:
             try:
-                envelope_params['geometry'] and envelope_params['inSR']
+                envelope_params["geometry"] and envelope_params["inSR"]
             except KeyError as error:
                 raise ValueError(
-                    'envelope_params must contain both the envelope geometry and its spatial reference'
+                    "envelope_params must contain both the envelope geometry and its spatial reference"
                 ) from error
-            self.envelope_params = {'geometryType': 'esriGeometryEnvelope'}
+            self.envelope_params = {"geometryType": "esriGeometryEnvelope"}
             self.envelope_params.update(envelope_params)
 
-        self.feature_params = {'outFields': '*', 'returnGeometry': 'true'}
+        self.feature_params = {"outFields": "*", "returnGeometry": "true"}
         if feature_params:
             self.feature_params.update(feature_params)
 
         self.where_clause = where_clause
 
     def _get_layer_info(self):
         """Do a basic query to get the layer's information as a dictionary from the json response.
@@ -738,58 +741,56 @@
         Raises:
             RuntimeError: If the response does not contain 'capabilities', 'type', or 'maxRecordCount' keys.
 
         Returns:
             dict: The query's json response as a dictionary
         """
 
-        response_json = utils.retry(requests.get, self.layer_url, params={'f': 'json'}, timeout=self.timeout).json()
+        response_json = utils.retry(requests.get, self.layer_url, params={"f": "json"}, timeout=self.timeout).json()
         try:
             #: bogus boolean to make sure the keys exist
-            response_json['capabilities'] and response_json['type']  # and response_json['maxRecordCount']
+            response_json["capabilities"] and response_json["type"]  # and response_json['maxRecordCount']
         except KeyError as error:
             raise RuntimeError(
-                'Response does not contain layer information; ensure URL points to a valid layer'
+                "Response does not contain layer information; ensure URL points to a valid layer"
             ) from error
 
         try:
-            response_json['maxRecordCount']
+            response_json["maxRecordCount"]
         except KeyError as error:
             raise RuntimeError(
-                'Response does not contain maxRecordCount; ensure URL points to a valid layer and is not a Group Layer'
+                "Response does not contain maxRecordCount; ensure URL points to a valid layer and is not a Group Layer"
             ) from error
 
         return response_json
 
     def check_capabilities(self, capability):
         """Raise error if the layer does not support capability
 
         Args:
             capability (str): The capability in question; will be casefolded.
 
         Raises:
             RuntimeError: if the casefolded capability is not present in the layer's capabilities.
         """
-        layer_capabilities = self.layer_properties_json['capabilities'].casefold().split(',')
+        layer_capabilities = self.layer_properties_json["capabilities"].casefold().split(",")
         if capability.casefold() not in layer_capabilities:
-            raise RuntimeError(
-                f'{capability.casefold()} capability not in layer\'s capabilities ({layer_capabilities})'
-            )
+            raise RuntimeError(f"{capability.casefold()} capability not in layer's capabilities ({layer_capabilities})")
 
     def _check_layer_type(self):
         """Make sure the layer is a feature layer or table (and thus we can extract features from it)
 
         Args:
             response_json (dict): The JSON response from a basic query parsed as a dictionary.
 
         Raises:
             RuntimeError: If the REST response type is not Feature Layer or Table
         """
 
-        if self.layer_properties_json['type'] not in ['Feature Layer', 'Table']:
+        if self.layer_properties_json["type"] not in ["Feature Layer", "Table"]:
             raise RuntimeError(
                 f'Layer {self.layer_url} is a {self.layer_properties_json["type"]}, not a feature layer or table'
             )
 
     def _get_object_id_field(self):
         """Get the service's objectIdField attribute
 
@@ -797,44 +798,44 @@
             response_json (dict): The JSON response from a basic query parsed as a dictionary.
 
         Returns:
             str: objectIdField
         """
 
         try:
-            unique_id_field = self.layer_properties_json['objectIdField']
+            unique_id_field = self.layer_properties_json["objectIdField"]
         except KeyError:
-            self._class_logger.debug('No objectIdField found in %s, using OBJECTID instead', self.layer_url)
-            unique_id_field = 'OBJECTID'
+            self._class_logger.debug("No objectIdField found in %s, using OBJECTID instead", self.layer_url)
+            unique_id_field = "OBJECTID"
 
         return unique_id_field
 
     def get_object_ids(self):
         """Get the Object IDs of the feature service layer, using the bounding envelope and/or where clause if present.
 
         Raises:
             RuntimeError: If the response does not contain an 'objectIds' key.
 
         Returns:
             list(int): The Object IDs
         """
 
-        objectid_params = {'returnIdsOnly': 'true', 'f': 'json', 'where': self.where_clause}
+        objectid_params = {"returnIdsOnly": "true", "f": "json", "where": self.where_clause}
         if self.envelope_params is not None:
             objectid_params.update(self.envelope_params)
-        self._class_logger.debug('OID params: %s', objectid_params)
+        self._class_logger.debug("OID params: %s", objectid_params)
 
-        response = utils.retry(requests.get, f'{self.layer_url}/query', params=objectid_params, timeout=self.timeout)
+        response = utils.retry(requests.get, f"{self.layer_url}/query", params=objectid_params, timeout=self.timeout)
         oids = []
         try:
-            oids = sorted(response.json()['objectIds'])
+            oids = sorted(response.json()["objectIds"])
         except KeyError as error:
-            raise RuntimeError(f'Could not get object IDs from {self.layer_url}') from error
+            raise RuntimeError(f"Could not get object IDs from {self.layer_url}") from error
         except TypeError as error:
-            if '\'NoneType\' object is not iterable' in str(error):
+            if "'NoneType' object is not iterable" in str(error):
                 oids = []
 
         return oids
 
     def get_unique_id_list_as_dataframe(self, unique_id_field, unique_id_list):
         """Use a REST query to download specified features from a MapService or FeatureService layer.
 
@@ -848,34 +849,34 @@
             Runtime Error: If the chunk's HTTP response code is not 200 (ie, the request failed)
             Runtime Error: The response could not be parsed into JSON (a technically successful request but bad data)
             Runtime Error: If the number of features downloaded does not match the number of OIDs requested
 
         Returns:
             pd.DataFrame.spatial: Spatially-enabled dataframe of the service layer's features
         """
-        unique_id_params = {'f': 'json'}
+        unique_id_params = {"f": "json"}
         unique_id_params.update(self.feature_params)
-        unique_id_params.update({'where': f'{unique_id_field} in ({",".join([str(oid) for oid in unique_id_list])})'})
+        unique_id_params.update({"where": f'{unique_id_field} in ({",".join([str(oid) for oid in unique_id_list])})'})
 
-        self._class_logger.debug('OID range params: %s', unique_id_params)
-        response = requests.get(f'{self.layer_url}/query', params=unique_id_params, timeout=self.timeout)
+        self._class_logger.debug("OID range params: %s", unique_id_params)
+        response = requests.get(f"{self.layer_url}/query", params=unique_id_params, timeout=self.timeout)
 
         if response.status_code != 200:
-            raise RuntimeError(f'Bad chunk response HTTP status code ({response.status_code})')
+            raise RuntimeError(f"Bad chunk response HTTP status code ({response.status_code})")
 
         try:
             fs = arcgis.features.FeatureSet.from_json(response.text)
             features_df = fs.sdf.sort_values(by=unique_id_field)
 
         except ujson.JSONDecodeError as error:
-            raise RuntimeError('Could not parse chunk features from response') from error
+            raise RuntimeError("Could not parse chunk features from response") from error
 
         if len(features_df) != len(unique_id_list):
             raise RuntimeError(
-                f'Missing features. {len(unique_id_list)} OIDs requested, but {len(features_df)} features downloaded'
+                f"Missing features. {len(unique_id_list)} OIDs requested, but {len(features_df)} features downloaded"
             )
 
         return features_df
 
 
 class SalesforceApiUserCredentials:
     """A salesforce API user credential model"""
```

### Comparing `ugrc-palletjack-4.3.0/src/palletjack/load.py` & `ugrc-palletjack-4.3.1/src/palletjack/load.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 """Modify existing ArcGIS Online content (mostly hosted feature services). Contains classes for updating hosted feature
 service data, modifying the attachments on a hosted feature service, or modifying map symbology.
 """
 
 import json
 import logging
 import shutil
-import sys
 import warnings
 from datetime import datetime
 from pathlib import Path
-from tempfile import TemporaryDirectory
 
 import arcgis
-import geopandas as gpd
 import numpy as np
 import pandas as pd
 import pyogrio
-from arcgis.features import GeoAccessor, GeoSeriesAccessor
+from arcgis.features import GeoAccessor, GeoSeriesAccessor  # noqa: F401
 
 from palletjack import utils
 
 logger = logging.getLogger(__name__)
 
 
 class FeatureServiceUpdater:
@@ -31,26 +28,28 @@
     update_features, and truncate_and_load_features.
 
     It is the client's responsibility to separate out the new data into these different steps. If the extract/transform
     stages result in separate groups of records that need to be added, deleted, and updated, the client must call the
     three different methods with dataframes containing only the respective records for each operation.
 
     The method used to upload the data to AGOL saves the updated data as a new layer named upload in working_dir/upload.
-    gdb, zips the gdb, uploads it to AGOL, and then uses this as the source data for a call to the feature layer's
-    .append() method. The geodatabase upload.gdb will be created in working_dir if it doesn't already exist. Ideally,
-    working_dir should be a TemporaryDirectory unless persistent access to the gdb is desired.
+    gdb, zips the gdb, uploads it to AGOL (with the item name `gdb_item_prefix Temporary gdb upload`), and then uses
+    this as the source data for a call to the feature layer's .append() method. The geodatabase upload.gdb will be
+    created in working_dir if it doesn't already exist. Ideally, working_dir should be a TemporaryDirectory unless
+    persistent access to the gdb is desired.
     """
 
-    def __init__(self, gis, feature_service_itemid, working_dir=None, layer_index=0):
+    def __init__(self, gis, feature_service_itemid, working_dir=None, layer_index=0, gdb_item_prefix="palletjack"):
         self._class_logger = logging.getLogger(__name__).getChild(self.__class__.__name__)
         self.gis = gis
         self.feature_service_itemid = feature_service_itemid
         self.feature_layer = arcgis.features.FeatureLayer.fromitem(gis.content.get(feature_service_itemid))
         self.working_dir = working_dir if working_dir else None
         self.layer_index = layer_index
+        self.gdb_item_prefix = gdb_item_prefix
 
     def add_features(self, dataframe):
         """Adds new features to existing hosted feature layer from new dataframe.
 
         The new dataframe must have a 'SHAPE' column containing geometries of the same type as the live data.
 
         The new dataframe's columns and data must match the existing data's fields (with the exception of generated
@@ -66,18 +65,18 @@
                 lengths, or a specified field is missing from either new or live data.
 
         Returns:
             int: Number of features added
         """
 
         self._class_logger.info(
-            'Adding items to layer `%s` in itemid `%s` in-place', self.layer_index, self.feature_service_itemid
+            "Adding items to layer `%s` in itemid `%s` in-place", self.layer_index, self.feature_service_itemid
         )
         fields = FeatureServiceUpdater._get_fields_from_dataframe(dataframe)
-        self._class_logger.debug('Using fields %s', fields)
+        self._class_logger.debug("Using fields %s", fields)
 
         #: Field checks to prevent various AGOL errors
         utils.FieldChecker.check_fields(self.feature_layer.properties, dataframe, fields, add_oid=False)
 
         #: Upload
         append_count = self._upload_data(
             dataframe,
@@ -105,40 +104,40 @@
             RuntimeError: If any of the OIDs fail to delete
 
         Returns:
             int: The number of features deleted
         """
 
         self._class_logger.info(
-            'Deleting features from layer `%s` in itemid `%s`', self.layer_index, self.feature_service_itemid
+            "Deleting features from layer `%s` in itemid `%s`", self.layer_index, self.feature_service_itemid
         )
-        self._class_logger.debug('Delete string: %s', delete_oids)
+        self._class_logger.debug("Delete string: %s", delete_oids)
 
         #: Verify delete list
         oid_numeric = utils.DeleteUtils.check_delete_oids_are_ints(delete_oids)
         utils.DeleteUtils.check_for_empty_oid_list(oid_numeric, delete_oids)
-        delete_string = ','.join([str(oid) for oid in oid_numeric])
+        delete_string = ",".join([str(oid) for oid in oid_numeric])
         num_missing_oids = utils.DeleteUtils.check_delete_oids_are_in_live_data(
             delete_string, oid_numeric, self.feature_layer
         )
 
         #: Note: apparently not all services support rollback:
         #: https://developers.arcgis.com/rest/services-reference/enterprise/delete-features.htm
         deletes = utils.retry(
             self.feature_layer.delete_features,
             deletes=delete_string,
             rollback_on_failure=True,
         )
 
-        failed_deletes = [result['objectId'] for result in deletes['deleteResults'] if not result['success']]
+        failed_deletes = [result["objectId"] for result in deletes["deleteResults"] if not result["success"]]
         if failed_deletes:
-            raise RuntimeError(f'The following Object IDs failed to delete: {failed_deletes}')
+            raise RuntimeError(f"The following Object IDs failed to delete: {failed_deletes}")
 
         #: The REST API still returns success: True on missing OIDs, so we have to track this ourselves
-        actual_delete_count = len(deletes['deleteResults']) - num_missing_oids
+        actual_delete_count = len(deletes["deleteResults"]) - num_missing_oids
 
         return actual_delete_count
 
     def update_features(self, dataframe, update_geometry=True):
         """Updates existing features within a hosted feature layer using OBJECTID as the join field.
 
         The new dataframe's columns and data must match the existing data's fields (with the exception of generated
@@ -165,36 +164,36 @@
                 lengths, or a specified field is missing from either new or live data.
 
         Returns:
             int: Number of features updated
         """
 
         self._class_logger.info(
-            'Updating layer `%s` in itemid `%s` in-place', self.layer_index, self.feature_service_itemid
+            "Updating layer `%s` in itemid `%s` in-place", self.layer_index, self.feature_service_itemid
         )
 
         fields = FeatureServiceUpdater._get_fields_from_dataframe(dataframe)
-        self._class_logger.debug('Updating fields %s', fields)
+        self._class_logger.debug("Updating fields %s", fields)
 
         #: Add null geometries if update_geometry==False so that we can create a featureset from the dataframe
         #: (geometries will be ignored by upsert call)
         if not update_geometry:
-            self._class_logger.debug('Attribute-only update; inserting null geometries')
-            dataframe['SHAPE'] = utils.get_null_geometries(self.feature_layer.properties)
+            self._class_logger.debug("Attribute-only update; inserting null geometries")
+            dataframe["SHAPE"] = utils.get_null_geometries(self.feature_layer.properties)
 
         #: Field checks to prevent various AGOL errors
         utils.FieldChecker.check_fields(self.feature_layer.properties, dataframe, fields, add_oid=True)
 
         #: Upload data
         append_count = self._upload_data(
             dataframe,
             upsert=True,
-            upsert_matching_field='OBJECTID',
+            upsert_matching_field="OBJECTID",
             append_fields=fields,  #: Apparently this works if append_fields is all the fields, but not a subset?
-            update_geometry=update_geometry
+            update_geometry=update_geometry,
         )
         return append_count
 
     def truncate_and_load_features(self, dataframe, save_old=False):
         """Overwrite a hosted feature layer by truncating and loading the new data
 
         When the existing dataset is truncated, a copy is kept in memory as a spatially-enabled dataframe. If
@@ -213,40 +212,40 @@
             save_old (bool, optional): Save existing data to backup.gdb in working_dir. Defaults to False
 
         Returns:
             int: Number of features loaded
         """
 
         self._class_logger.info(
-            'Truncating and loading layer `%s` in itemid `%s`', self.layer_index, self.feature_service_itemid
+            "Truncating and loading layer `%s` in itemid `%s`", self.layer_index, self.feature_service_itemid
         )
         start = datetime.now()
 
         #: Save the data to disk if desired
         if save_old:
-            self._class_logger.info('Saving existing data to %s', self.working_dir)
+            self._class_logger.info("Saving existing data to %s", self.working_dir)
             saved_layer_path = utils.save_feature_layer_to_gdb(self.feature_layer, self.working_dir)
 
         fields = FeatureServiceUpdater._get_fields_from_dataframe(dataframe)
 
         #: Field checks to prevent various AGOL errors
         utils.FieldChecker.check_fields(self.feature_layer.properties, dataframe, fields, add_oid=False)
 
-        self._class_logger.info('Truncating existing features...')
+        self._class_logger.info("Truncating existing features...")
         self._truncate_existing_data()
 
         try:
-            self._class_logger.info('Loading new data...')
+            self._class_logger.info("Loading new data...")
             append_count = self._upload_data(dataframe, upsert=False)
-            self._class_logger.debug('Total truncate and load time: %s', datetime.now() - start)
+            self._class_logger.debug("Total truncate and load time: %s", datetime.now() - start)
         except Exception:
             if save_old:
-                self._class_logger.error('Append failed. Data saved to %s', saved_layer_path)
+                self._class_logger.error("Append failed. Data saved to %s", saved_layer_path)
                 raise
-            self._class_logger.error('Append failed. Old data not saved (save_old set to False)')
+            self._class_logger.error("Append failed. Old data not saved (save_old set to False)")
             raise
 
         return append_count
 
     @staticmethod
     def _get_fields_from_dataframe(dataframe):
         """Get the fields from a dataframe, excluding Shape_Area and Shape_Length
@@ -255,15 +254,15 @@
             dataframe (pd.DataFrame): Dataframe to get fields from
 
         Returns:
             list[str]: List of the columns of the dataframe, excluding Shape_Area and Shape_Length
         """
 
         fields = list(dataframe.columns)
-        for auto_gen_field in ['Shape_Area', 'Shape_Length']:
+        for auto_gen_field in ["Shape_Area", "Shape_Length"]:
             try:
                 fields.remove(auto_gen_field)
             except ValueError:
                 continue
 
         return fields
 
@@ -284,50 +283,48 @@
             ValueError: If the field used as a key for upsert matching is not present in either the new or live data
             RuntimeError: If the append operation fails
 
         Returns:
             int: The number of records upserted
         """
         try:
-            if append_kwargs['upsert'] \
-                and (
-                        append_kwargs['upsert_matching_field'] not in append_kwargs['append_fields']
-                        or
-                        append_kwargs['upsert_matching_field'] not in dataframe.columns
-                    ):
+            if append_kwargs["upsert"] and (
+                append_kwargs["upsert_matching_field"] not in append_kwargs["append_fields"]
+                or append_kwargs["upsert_matching_field"] not in dataframe.columns
+            ):
                 raise ValueError(
                     f'Upsert matching field {append_kwargs["upsert_matching_field"]} not found in either append fields or existing fields.'
                 )
         except KeyError:
             pass
-        self._class_logger.debug('Saving data to gdb and zipping...')
+        self._class_logger.debug("Saving data to gdb and zipping...")
         zipped_gdb_path = self._save_to_gdb_and_zip(dataframe)
 
-        self._class_logger.debug('Uploading gdb to AGOL...')
+        self._class_logger.debug("Uploading gdb to AGOL...")
         gdb_item = self._upload_gdb(zipped_gdb_path)
 
-        self._class_logger.debug('Appending data from gdb to feature layer...')
+        self._class_logger.debug("Appending data from gdb to feature layer...")
         try:
             result, messages = utils.retry(
                 self.feature_layer.append,
                 item_id=gdb_item.id,
-                upload_format='filegdb',
-                source_table_name='upload',
+                upload_format="filegdb",
+                source_table_name="upload",
                 return_messages=True,
                 rollback=True,
-                **append_kwargs
+                **append_kwargs,
             )
             if not result:
-                raise RuntimeError('Append failed but did not error')
+                raise RuntimeError("Append failed but did not error")
         except Exception as error:
-            raise RuntimeError('Failed to append data from gdb, changes should have been rolled back') from error
+            raise RuntimeError("Failed to append data from gdb, changes should have been rolled back") from error
 
         self._cleanup(gdb_item, zipped_gdb_path)
 
-        return messages['recordCount']
+        return messages["recordCount"]
 
     def _save_to_gdb_and_zip(self, dataframe):
         """Save a spatially-enabled dataframe to a gdb, zip it, and return path to the zipped file.
 
         Requires self.working_dir to be set. Uses pyogrio to save the dataframe to the gdb, then uses
         shutil.make_archive to zip the gdb. The zipped gdb is saved in self.working_dir.
 
@@ -339,30 +336,30 @@
             ValueError: If self.working_dir is not set or the empty upload.gdb doesn't exist in it
 
         Returns:
             pathlib.Path: The path to the zipped GDB
         """
 
         try:
-            gdb_path = Path(self.working_dir) / 'upload.gdb'
+            gdb_path = Path(self.working_dir) / "upload.gdb"
         except TypeError as error:
-            raise AttributeError('working_dir not specified on FeatureServiceUpdater') from error
+            raise AttributeError("working_dir not specified on FeatureServiceUpdater") from error
 
         gdf = utils.sedf_to_gdf(dataframe)
 
         try:
-            gdf.to_file(gdb_path, layer='upload', engine='pyogrio', driver='OpenFileGDB')
+            gdf.to_file(gdb_path, layer="upload", engine="pyogrio", driver="OpenFileGDB")
         except pyogrio.errors.DataSourceError as error:
             raise ValueError(
-                f'Error writing layer to {gdb_path}. Verify {self.working_dir} exists and is writable.'
+                f"Error writing layer to {gdb_path}. Verify {self.working_dir} exists and is writable."
             ) from error
         try:
-            zipped_gdb_path = shutil.make_archive(gdb_path, 'zip', root_dir=gdb_path.parent, base_dir=gdb_path.name)
+            zipped_gdb_path = shutil.make_archive(gdb_path, "zip", root_dir=gdb_path.parent, base_dir=gdb_path.name)
         except OSError as error:
-            raise ValueError(f'Error zipping {gdb_path}') from error
+            raise ValueError(f"Error zipping {gdb_path}") from error
 
         return zipped_gdb_path
 
     def _upload_gdb(self, zipped_gdb_path):
         """Add a zipped gdb to AGOL as an item to self.gis
 
         Args:
@@ -375,22 +372,22 @@
             arcgis.gis.Item: Reference to the resulting Item object in self.gis
         """
 
         try:
             gdb_item = utils.retry(
                 self.gis.content.add,
                 item_properties={
-                    'type': 'File Geodatabase',
-                    'title': 'Temporary gdb upload',
-                    'snippet': 'Temporary gdb upload from palletjack'
+                    "type": "File Geodatabase",
+                    "title": f"{self.gdb_item_prefix} Temporary gdb upload",
+                    "snippet": "Temporary gdb upload from palletjack",
                 },
-                data=zipped_gdb_path
+                data=zipped_gdb_path,
             )
         except Exception as error:
-            raise RuntimeError(f'Error uploading {zipped_gdb_path} to AGOL') from error
+            raise RuntimeError(f"Error uploading {zipped_gdb_path} to AGOL") from error
         return gdb_item
 
     def _cleanup(self, gdb_item, zipped_gdb_path):
         """Remove the zipped gdb from disk and the gdb item from AGOL
 
         Args:
             gdb_item (arcgis.gis.Item): Reference to the gdb item in self.gis
@@ -399,39 +396,39 @@
         Raises:
             RuntimeError: If there are errors deleting the gdb item or the zipped gdb
         """
 
         try:
             gdb_item.delete()
         except Exception as error:
-            warnings.warn(f'Error deleting gdb item {gdb_item.id} from AGOL')
+            warnings.warn(f"Error deleting gdb item {gdb_item.id} from AGOL")
             warnings.warn(repr(error))
 
         try:
             Path(zipped_gdb_path).unlink()
         except Exception as error:
-            warnings.warn(f'Error deleting zipped gdb {zipped_gdb_path}')
+            warnings.warn(f"Error deleting zipped gdb {zipped_gdb_path}")
             warnings.warn(repr(error))
 
     def _truncate_existing_data(self):
         """Remove all existing features from the live dataset
 
         Raises:
             RuntimeError: If the truncate fails
 
         Returns:
             pd.DataFrame: The feature layer's data as a spatially-enabled dataframe prior to truncating
         """
 
-        self._class_logger.debug('Truncating...')
+        self._class_logger.debug("Truncating...")
         truncate_result = utils.retry(self.feature_layer.manager.truncate, asynchronous=True, wait=True)
         self._class_logger.debug(truncate_result)
-        if truncate_result['status'] != 'Completed':
+        if truncate_result["status"] != "Completed":
             raise RuntimeError(
-                f'Failed to truncate existing data from layer id {self.layer_index} in itemid {self.feature_service_itemid}'
+                f"Failed to truncate existing data from layer id {self.layer_index} in itemid {self.feature_service_itemid}"
             )
 
 
 class FeatureServiceAttachmentsUpdater:
     """Add or overwrite attachments in a feature service using a dataframe of the desired "new" attachments.
 
     Updates the attachments based on a dataframe containing two columns: a join key present in the live data (the
@@ -462,38 +459,38 @@
             attachments_df (pd.DataFrame): New attachment data, including the join key and a path to the "new"
                 attachment
 
         Returns:
             pd.DataFrame: Attachments dataframe with corresponding live OIDs and GUIDs.
         """
 
-        self._class_logger.debug('Using %s as the join field between live and new data', attachment_join_field)
-        subset_df = live_features_as_df.reindex(columns=['OBJECTID', 'GlobalID', attachment_join_field])
-        merged_df = subset_df.merge(attachments_df, on=attachment_join_field, how='inner')
-        self._class_logger.debug('%s features common to both live and new data', len(merged_df.index))
+        self._class_logger.debug("Using %s as the join field between live and new data", attachment_join_field)
+        subset_df = live_features_as_df.reindex(columns=["OBJECTID", "GlobalID", attachment_join_field])
+        merged_df = subset_df.merge(attachments_df, on=attachment_join_field, how="inner")
+        self._class_logger.debug("%s features common to both live and new data", len(merged_df.index))
 
         return merged_df
 
     def _get_current_attachment_info_by_oid(self, live_data_subset_df):
         """Merge the live attachment data using the ObjectID as the join
 
         Args:
             live_data_subset_df (pd.DataFrame): Live data with 'OBJECTID', 'GlobalID', and new attachment data
 
         Returns:
             pd.DataFrame: Live and new attachment data in one dataframe
         """
 
         live_attachments_df = pd.DataFrame(self.feature_layer.attachments.search())
-        live_attachments_subset_df = live_attachments_df.reindex(columns=['PARENTOBJECTID', 'NAME', 'ID'])
+        live_attachments_subset_df = live_attachments_df.reindex(columns=["PARENTOBJECTID", "NAME", "ID"])
         merged_df = live_data_subset_df.merge(
-            live_attachments_subset_df, left_on='OBJECTID', right_on='PARENTOBJECTID', how='left'
+            live_attachments_subset_df, left_on="OBJECTID", right_on="PARENTOBJECTID", how="left"
         )
         #: Cast ID field to nullable int to avoid conversion to float for np.nans
-        merged_df['ID'] = merged_df['ID'].astype('Int64')
+        merged_df["ID"] = merged_df["ID"].astype("Int64")
 
         return merged_df
 
     def _create_attachment_action_df(self, attachment_eval_df, attachment_path_field):
         """Create a dataframe containing the action needed for each feature resulting from the attachment join.
 
         If the live feature doesn't have an attachment, add the attachment. If it does, compare the file names and only
@@ -505,31 +502,34 @@
             attachment_path_field (str): The column that holds the attachment path
 
         Returns:
             pd.DataFrame: attachment_eval_df with 'operation' and 'new_filename' columns added
         """
 
         #: Get the file name from the full path
-        attachment_eval_df['new_filename'] = attachment_eval_df[attachment_path_field].apply(
+        attachment_eval_df["new_filename"] = attachment_eval_df[attachment_path_field].apply(
             lambda path: Path(path).name
         )
 
         #: Overwrite if different names, add if no existing name, do nothing if names are the same
-        attachment_eval_df['operation'] = np.nan
-        attachment_eval_df.loc[attachment_eval_df['NAME'] != attachment_eval_df['new_filename'],
-                               'operation'] = 'overwrite'
-        attachment_eval_df.loc[attachment_eval_df['NAME'].isna(), 'operation'] = 'add'
+        attachment_eval_df["operation"] = np.nan
+        attachment_eval_df.loc[attachment_eval_df["NAME"] != attachment_eval_df["new_filename"], "operation"] = (
+            "overwrite"
+        )
+        attachment_eval_df.loc[attachment_eval_df["NAME"].isna(), "operation"] = "add"
 
-        value_counts = attachment_eval_df['operation'].value_counts(dropna=False)
-        for operation in ['add', 'overwrite', np.nan]:
+        value_counts = attachment_eval_df["operation"].value_counts(dropna=False)
+        for operation in ["add", "overwrite", np.nan]:
             if operation not in value_counts:
                 value_counts[operation] = 0
         self._class_logger.debug(
-            'Calculated attachment operations: adds: %s, overwrites: %s, none: %s', value_counts['add'],
-            value_counts['overwrite'], value_counts[np.nan]
+            "Calculated attachment operations: adds: %s, overwrites: %s, none: %s",
+            value_counts["add"],
+            value_counts["overwrite"],
+            value_counts[np.nan],
         )
 
         return attachment_eval_df
 
     def _add_attachments_by_oid(self, attachment_action_df, attachment_path_field):
         """Add attachments using the feature's OID based on the 'operation' field of the dataframe
 
@@ -538,33 +538,33 @@
                 attachment_path_field columns
             attachment_path_field (str): The column that holds the attachment path
 
         Returns:
             int: The number of features that successfully have attachments added.
         """
 
-        adds_dict = attachment_action_df[attachment_action_df['operation'] == 'add'].to_dict(orient='index')
+        adds_dict = attachment_action_df[attachment_action_df["operation"] == "add"].to_dict(orient="index")
         adds_count = 0
 
         for row in adds_dict.values():
-            target_oid = row['OBJECTID']
+            target_oid = row["OBJECTID"]
             filepath = row[attachment_path_field]
 
-            self._class_logger.debug('Add %s to OID %s', filepath, target_oid)
+            self._class_logger.debug("Add %s to OID %s", filepath, target_oid)
             try:
                 result = self.feature_layer.attachments.add(target_oid, filepath)
             except Exception:
-                self._class_logger.error('AGOL error while adding %s to OID %s', filepath, target_oid, exc_info=True)
-                self.failed_dict[target_oid] = ('add', filepath)
+                self._class_logger.error("AGOL error while adding %s to OID %s", filepath, target_oid, exc_info=True)
+                self.failed_dict[target_oid] = ("add", filepath)
                 continue
 
-            self._class_logger.debug('%s', result)
-            if not result['addAttachmentResult']['success']:
-                warnings.warn(f'Failed to attach {filepath} to OID {target_oid}')
-                self.failed_dict[target_oid] = ('add', filepath)
+            self._class_logger.debug("%s", result)
+            if not result["addAttachmentResult"]["success"]:
+                warnings.warn(f"Failed to attach {filepath} to OID {target_oid}")
+                self.failed_dict[target_oid] = ("add", filepath)
                 continue
 
             adds_count += 1
 
         return adds_count
 
     def _overwrite_attachments_by_oid(self, attachment_action_df, attachment_path_field):
@@ -575,57 +575,57 @@
                 attachment_path_field columns
             attachment_path_field (str): The column that holds the attachment path
 
         Returns:
             int: The number of features that successfully have their attachments overwritten.
         """
 
-        overwrites_dict = attachment_action_df[attachment_action_df['operation'] == 'overwrite'].to_dict(orient='index')
+        overwrites_dict = attachment_action_df[attachment_action_df["operation"] == "overwrite"].to_dict(orient="index")
         overwrites_count = 0
 
         for row in overwrites_dict.values():
-            target_oid = row['OBJECTID']
+            target_oid = row["OBJECTID"]
             filepath = row[attachment_path_field]
-            attachment_id = row['ID']
-            old_name = row['NAME']
+            attachment_id = row["ID"]
+            old_name = row["NAME"]
 
             self._class_logger.debug(
-                'Overwriting %s (attachment ID %s) on OID %s with %s', old_name, attachment_id, target_oid, filepath
+                "Overwriting %s (attachment ID %s) on OID %s with %s", old_name, attachment_id, target_oid, filepath
             )
             try:
                 result = self.feature_layer.attachments.update(target_oid, attachment_id, filepath)
             except Exception:
                 self._class_logger.error(
-                    'AGOL error while overwriting %s (attachment ID %s) on OID %s with %s',
+                    "AGOL error while overwriting %s (attachment ID %s) on OID %s with %s",
                     old_name,
                     attachment_id,
                     target_oid,
                     filepath,
-                    exc_info=True
+                    exc_info=True,
                 )
-                self.failed_dict[target_oid] = ('update', filepath)
+                self.failed_dict[target_oid] = ("update", filepath)
                 continue
 
-            if not result['updateAttachmentResult']['success']:
+            if not result["updateAttachmentResult"]["success"]:
                 warnings.warn(
-                    f'Failed to update {old_name}, attachment ID {attachment_id}, on OID {target_oid} with {filepath}'
+                    f"Failed to update {old_name}, attachment ID {attachment_id}, on OID {target_oid} with {filepath}"
                 )
-                self.failed_dict[target_oid] = ('update', filepath)
+                self.failed_dict[target_oid] = ("update", filepath)
                 continue
 
             overwrites_count += 1
 
         return overwrites_count
 
     @staticmethod
     def _check_attachment_dataframe_for_invalid_column_names(attachment_dataframe, invalid_names):
         invalid_names_index = pd.Index(invalid_names)
         intersection = attachment_dataframe.columns.intersection(invalid_names_index)
         if not intersection.empty:
-            raise RuntimeError(f'Attachment dataframe contains the following invalid names: {list(intersection)}')
+            raise RuntimeError(f"Attachment dataframe contains the following invalid names: {list(intersection)}")
 
     def update_attachments(
         self, feature_layer_itemid, attachment_join_field, attachment_path_field, attachments_df, layer_number=0
     ):
         """Update a feature layer's attachments based on info from a dataframe of desired attachment file names
 
         Depends on a dataframe populated with a join key for the live data and the downloaded or locally-available
@@ -642,35 +642,35 @@
                 to the attachment
             layer_number (int, optional): The layer within the Item ID to update. Defaults to 0.
 
         Returns:
             (int, int): Tuple of counts of successful overwrites and adds.
         """
 
-        self._class_logger.info('Updating attachments...')
+        self._class_logger.info("Updating attachments...")
         #: These names are present in the live attachment data downloaded from AGOL. Because we merge the dataframes
         #: later, we need to make sure they're not the same. There may be better ways of handling this that allows the
         #: client names to be preserved, but for now force them to fix this.
         self._check_attachment_dataframe_for_invalid_column_names(
-            attachments_df, invalid_names=['OBJECTID', 'PARENTOBJECTID', 'NAME', 'ID']
+            attachments_df, invalid_names=["OBJECTID", "PARENTOBJECTID", "NAME", "ID"]
         )
-        self._class_logger.debug('Using layer %s from item ID %s', layer_number, feature_layer_itemid)
+        self._class_logger.debug("Using layer %s from item ID %s", layer_number, feature_layer_itemid)
         self.feature_layer = self.gis.content.get(feature_layer_itemid).layers[layer_number]
         live_features_as_df = pd.DataFrame.spatial.from_layer(self.feature_layer)
         live_data_subset_df = self._get_live_oid_and_guid_from_join_field_values(
             live_features_as_df, attachment_join_field, attachments_df
         )
         #: TODO: Make sure layer supports attachments so we don't get an arcgis error.
         #: Check out the feature layer .properties and FeatureLayerManager.add_to_definition to check/enable?
         attachment_eval_df = self._get_current_attachment_info_by_oid(live_data_subset_df)
         attachment_action_df = self._create_attachment_action_df(attachment_eval_df, attachment_path_field)
 
         overwrites_count = self._overwrite_attachments_by_oid(attachment_action_df, attachment_path_field)
         adds_count = self._add_attachments_by_oid(attachment_action_df, attachment_path_field)
-        self._class_logger.info('%s attachments added, %s attachments overwritten', adds_count, overwrites_count)
+        self._class_logger.info("%s attachments added, %s attachments overwritten", adds_count, overwrites_count)
 
         return overwrites_count, adds_count
 
     @staticmethod
     def build_attachments_dataframe(input_dataframe, join_column, attachment_column, out_dir):
         """Create an attachments dataframe by subsetting down to just the two fields and dropping any rows
            with null/empty attachments
@@ -681,20 +681,22 @@
             attachment_column (str): Filename for each attachment
             out_dir (str or Path): Output directory, will be used to build full path to attachment
 
         Returns:
             pd.DataFrame: Dataframe with join key, attachment name, and full attachment paths
         """
 
-        input_dataframe[attachment_column].replace('', np.nan, inplace=True)  #: pandas doesn't see empty strings as NAs
-        attachments_dataframe = input_dataframe[[join_column, attachment_column]] \
-                                            .copy().dropna(subset=[attachment_column])
+        input_dataframe[attachment_column].replace("", np.nan, inplace=True)  #: pandas doesn't see empty strings as NAs
+        attachments_dataframe = (
+            input_dataframe[[join_column, attachment_column]].copy().dropna(subset=[attachment_column])
+        )
         #: Create the full path by prepending the output directory using .apply and a lambda function
-        attachments_dataframe['full_file_path'] = attachments_dataframe[attachment_column] \
-                                                    .apply(lambda filename: str(Path(out_dir, filename)))
+        attachments_dataframe["full_file_path"] = attachments_dataframe[attachment_column].apply(
+            lambda filename: str(Path(out_dir, filename))
+        )
 
         return attachments_dataframe
 
 
 class ColorRampReclassifier:
     """Updates the interval ranges on a webmap's layer's classification renderer based on the layer's current data.
 
@@ -721,18 +723,18 @@
             layer_name (str): The exact name of the layer
             feature_layer_number (int): The number of the layer with the feature service to update. Defaults to 0.
 
         Returns:
             spatially-enabled data frame: The layer's data, including geometries.
         """
 
-        self._class_logger.info('Getting dataframe from `%s` on `%s`', layer_name, self.webmap_item.title)
+        self._class_logger.info("Getting dataframe from `%s` on `%s`", layer_name, self.webmap_item.title)
         webmap_object = arcgis.mapping.WebMap(self.webmap_item)
         layer = webmap_object.get_layer(title=layer_name)
-        feature_layer = self.gis.content.get(layer['itemId'])
+        feature_layer = self.gis.content.get(layer["itemId"])
         layer_dataframe = pd.DataFrame.spatial.from_layer(feature_layer.layers[feature_layer_number])
 
         return layer_dataframe
 
     def _get_layer_id(self, layer_name):
         """Get the ID number of layer_name in self.webmap_item
 
@@ -743,17 +745,17 @@
             ValueError: If the layer is not found in the webmap
 
         Returns:
             int: The index (0-based) of the the layer in the web map
         """
 
         data = self.webmap_item.get_data()
-        for layer_id, layer in enumerate(data['operationalLayers']):
-            if layer['title'] == layer_name:
-                self._class_logger.debug('Layer `%s` has id `%s`', layer_name, layer_id)
+        for layer_id, layer in enumerate(data["operationalLayers"]):
+            if layer["title"] == layer_name:
+                self._class_logger.debug("Layer `%s` has id `%s`", layer_name, layer_id)
                 return layer_id
 
         #: If we haven't matched the title and returned a valid id, raise an error.
         raise ValueError(f'Could not find "{layer_name}" in {self.webmap_item.title}')
 
     @staticmethod
     def _calculate_new_stops(dataframe, column, stops):
@@ -765,15 +767,15 @@
             stops (int, optional): Number of stops to create.
 
         Returns:
             List: New stops cast as ints
         """
 
         if column not in dataframe.columns:
-            raise ValueError(f'Column `{column}` not in dataframe')
+            raise ValueError(f"Column `{column}` not in dataframe")
         minval = dataframe[column].min()
         mean = dataframe[column].mean()
         std_dev = dataframe[column].std()
         upper = mean + std_dev  #: AGOL's default upper value for unclassed ramps seems to be mean + 1 std dev
 
         new_stops = np.linspace(minval, upper, stops)
         new_stops_ints = [int(stop) for stop in new_stops]
@@ -789,25 +791,25 @@
 
         Returns:
             Bool: Success or failure of update operation
         """
 
         #: Get short reference to the stops dictionary from the webmap's data json
         data = self.webmap_item.get_data()
-        renderer = data['operationalLayers'][layer_number]['layerDefinition']['drawingInfo']['renderer']
-        stops = renderer['visualVariables'][0]['stops']
+        renderer = data["operationalLayers"][layer_number]["layerDefinition"]["drawingInfo"]["renderer"]
+        stops = renderer["visualVariables"][0]["stops"]
 
         #: Overwrite the value, update the webmap item
         for stop, new_value in zip(stops, new_stops):
-            stop['value'] = new_value
+            stop["value"] = new_value
         self._class_logger.info(
-            'Updating stop values on layer number `%s` in `%s`', layer_number, self.webmap_item.title
+            "Updating stop values on layer number `%s` in `%s`", layer_number, self.webmap_item.title
         )
-        result = self.webmap_item.update(item_properties={'text': json.dumps(data)})
-        self._class_logger.debug('Update result: %s', result)
+        result = self.webmap_item.update(item_properties={"text": json.dumps(data)})
+        self._class_logger.debug("Update result: %s", result)
 
         return result
 
     def update_color_ramp_values(self, layer_name, column_name, stops=5):
         """Update the color ramp ranges for layer_name in self.webmap_item.
 
         Does not alter colors or introduce additional stops; only overwrites the values for existing breaks.
```

### Comparing `ugrc-palletjack-4.3.0/src/palletjack/transform.py` & `ugrc-palletjack-4.3.1/src/palletjack/transform.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Transform pandas dataframes in preparation for loading to AGOL.
 """
+
 import locale
 import logging
 import warnings
 from datetime import datetime
 
 import arcgis
 import pandas as pd
-from arcgis import GeoAccessor, GeoSeriesAccessor
+from arcgis import GeoAccessor, GeoSeriesAccessor  # noqa: F401
 
 from palletjack import utils
 
 module_logger = logging.getLogger(__name__)
 
 
 class APIGeocoder:
@@ -55,55 +56,54 @@
             pd.DataFrame.spatial: Geocoded data as a spatially-enabled DataFrame
         """
 
         start = datetime.now()
 
         #: Should this return? Should it raise an error instead?
         if dataframe.empty:
-            warnings.warn('No records to geocode (empty dataframe)', RuntimeWarning)
+            warnings.warn("No records to geocode (empty dataframe)", RuntimeWarning)
 
         dataframe_length = len(dataframe.index)
         reporting_interval = utils.calc_modulus_for_reporting_interval(dataframe_length)
-        self._class_logger.info('Geocoding %s rows...', dataframe_length)
+        self._class_logger.info("Geocoding %s rows...", dataframe_length)
 
         street_col_index = dataframe.columns.get_loc(street_col)
         zone_col_index = dataframe.columns.get_loc(zone_col)
         new_rows = []
         for i, row in enumerate(dataframe.itertuples(index=False)):
             if i % reporting_interval == 0:
-                self._class_logger.info('Geocoding row %s of %s, %s%%', i, dataframe_length, i / dataframe_length * 100)
+                self._class_logger.info("Geocoding row %s of %s, %s%%", i, dataframe_length, i / dataframe_length * 100)
             row_dict = row._asdict()
             results = utils.Geocoding.geocode_addr(
                 row[street_col_index],
                 row[zone_col_index],
                 self.api_key,
                 rate_limits,
                 spatialReference=str(wkid),
-                **api_args
+                **api_args,
             )
             self._class_logger.debug(
-                '%s of %s: %s, %s = %s', i, dataframe_length, row[street_col_index], row[zone_col_index], results
+                "%s of %s: %s, %s = %s", i, dataframe_length, row[street_col_index], row[zone_col_index], results
             )
-            row_dict['x'], row_dict['y'], row_dict['score'], row_dict['matchAddress'] = results
+            row_dict["x"], row_dict["y"], row_dict["score"], row_dict["matchAddress"] = results
             new_rows.append(row_dict)
 
-        spatial_dataframe = pd.DataFrame.spatial.from_xy(pd.DataFrame(new_rows), 'x', 'y', sr=int(wkid))
+        spatial_dataframe = pd.DataFrame.spatial.from_xy(pd.DataFrame(new_rows), "x", "y", sr=int(wkid))
 
         end = datetime.now()
-        self._class_logger.info('%s Records geocoded in %s', len(spatial_dataframe.index), (end - start))
+        self._class_logger.info("%s Records geocoded in %s", len(spatial_dataframe.index), (end - start))
         try:
-            self._class_logger.debug('Average time per record: %s', (end - start) / len(spatial_dataframe.index))
+            self._class_logger.debug("Average time per record: %s", (end - start) / len(spatial_dataframe.index))
         except ZeroDivisionError:
-            warnings.warn('Empty spatial dataframe after geocoding', RuntimeWarning)
+            warnings.warn("Empty spatial dataframe after geocoding", RuntimeWarning)
         return spatial_dataframe
 
 
 class FeatureServiceMerging:
-    """Get the live dataframe from a feature service and update it from another dataframe
-    """
+    """Get the live dataframe from a feature service and update it from another dataframe"""
 
     @staticmethod
     def update_live_data_with_new_data(live_dataframe, new_dataframe, join_column):
         """Update a dataframe with data from another
 
         Args:
             live_dataframe (pd.DataFrame): The dataframe containing info to be updated
@@ -119,27 +119,27 @@
             pd.DataFrame: The updated dataframe, with data types converted via .convert_dtypes()
         """
 
         try:
             live_dataframe.set_index(join_column, inplace=True)
             new_dataframe.set_index(join_column, inplace=True)
         except KeyError as error:
-            raise ValueError('Join column not found in live or new dataframes') from error
+            raise ValueError("Join column not found in live or new dataframes") from error
 
-        indicator_dataframe = live_dataframe.merge(new_dataframe, on=join_column, how='outer', indicator=True)
-        new_only_dataframe = indicator_dataframe[indicator_dataframe['_merge'] == 'right_only']
+        indicator_dataframe = live_dataframe.merge(new_dataframe, on=join_column, how="outer", indicator=True)
+        new_only_dataframe = indicator_dataframe[indicator_dataframe["_merge"] == "right_only"]
         if not new_only_dataframe.empty:
             keys_not_found = list(new_only_dataframe.index)
             warnings.warn(
-                f'The following keys from the new data were not found in the existing dataset: {keys_not_found}',
-                RuntimeWarning
+                f"The following keys from the new data were not found in the existing dataset: {keys_not_found}",
+                RuntimeWarning,
             )
 
         live_dataframe.update(new_dataframe)
-        return (live_dataframe.reset_index().convert_dtypes())
+        return live_dataframe.reset_index().convert_dtypes()
 
     @staticmethod
     def get_live_dataframe(gis, feature_service_itemid, layer_index=0):
         """Get a spatially-enabled dataframe representation of a hosted feature layer
 
         Args:
             gis (arcgis.gis.GIS): GIS object of the desired organization
@@ -155,22 +155,21 @@
 
         try:
             feature_layer = arcgis.features.FeatureLayer.fromitem(
                 gis.content.get(feature_service_itemid), layer_id=layer_index
             )
             live_dataframe = feature_layer.query(as_df=True)
         except Exception as error:
-            raise RuntimeError('Failed to load live dataframe') from error
+            raise RuntimeError("Failed to load live dataframe") from error
 
         return live_dataframe
 
 
 class DataCleaning:
-    """Static methods for cleaning dataframes prior to uploading to AGOL
-    """
+    """Static methods for cleaning dataframes prior to uploading to AGOL"""
 
     @staticmethod
     def switch_to_nullable_int(dataframe, fields_that_should_be_ints):
         """Convert specified fields to panda's nullable Int64 type to preserve int to EsriFieldTypeInteger mapping
 
         Args:
             dataframe (pd.DataFrame): Input dataframe with columns to be converted
@@ -183,18 +182,18 @@
         Returns:
             pd.DataFrame: Input dataframe with columns converted to nullable Int64
         """
 
         retyped = dataframe.copy()
         try:
             for field in fields_that_should_be_ints:
-                retyped[field] = DataCleaning._switch_series_to_numeric_dtype(retyped[field], 'Int64')
+                retyped[field] = DataCleaning._switch_series_to_numeric_dtype(retyped[field], "Int64")
         except (TypeError, ValueError) as error:
             raise TypeError(
-                'Cannot convert one or more fields to nullable ints. Check for non-int/non-np.nan values.'
+                "Cannot convert one or more fields to nullable ints. Check for non-int/non-np.nan values."
             ) from error
         return retyped
 
     @staticmethod
     def switch_to_float(dataframe, fields_that_should_be_floats):
         """Convert specified fields to float, converting empty strings to None first as required
 
@@ -209,18 +208,18 @@
         Returns:
             pd.DataFrame: Input dataframe with columns converted to float
         """
 
         retyped = dataframe.copy()
         try:
             for field in fields_that_should_be_floats:
-                retyped[field] = DataCleaning._switch_series_to_numeric_dtype(retyped[field], 'float')
+                retyped[field] = DataCleaning._switch_series_to_numeric_dtype(retyped[field], "float")
         except (TypeError, ValueError) as error:
             raise TypeError(
-                'Cannot convert one or more fields to floats. Check for non-float/non-null values.'
+                "Cannot convert one or more fields to floats. Check for non-float/non-null values."
             ) from error
         return retyped
 
     @staticmethod
     def _switch_series_to_numeric_dtype(series, dtype):
         """Switch the dtype of a series to the specified dtype
 
@@ -231,17 +230,17 @@
             series (pd.Series): The series to be converted
             dtype (str): The dtype to convert to
 
         Returns:
             pd.Series: The converted series
         """
 
-        if series.dtype == 'object':
+        if series.dtype == "object":
             series = series.astype(str).apply(locale.delocalize)
-            series.replace('', None, inplace=True)
+            series.replace("", None, inplace=True)
         return series.astype(dtype)
 
     @staticmethod
     def switch_to_datetime(dataframe, date_fields, **to_datetime_kwargs):
         """Convert specified fields to datetime dtypes to ensure proper date formatting for AGOL
 
         Args:
@@ -250,17 +249,17 @@
             **to_datetime_kwargs (keyword arguments, optional): Arguments to pass through to pd.to_datetime
 
         Returns:
             pd.DataFrame: The source dataframe with converted fields.
         """
 
         for field in date_fields:
-            dataframe[field] = pd.to_datetime(dataframe[field], **to_datetime_kwargs) \
-                                    .dt.as_unit('ns') \
-                                    .dt.tz_localize(None)
+            dataframe[field] = (
+                pd.to_datetime(dataframe[field], **to_datetime_kwargs).dt.as_unit("ns").dt.tz_localize(None)
+            )
 
         return dataframe
 
     @staticmethod
     def rename_dataframe_columns_for_agol(dataframe):
         """Rename all the columns in a dataframe to valid AGOL column names
```

### Comparing `ugrc-palletjack-4.3.0/src/palletjack/utils.py` & `ugrc-palletjack-4.3.1/src/palletjack/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         nonlocal tries
 
         try:
             return worker_method(*args, **kwargs)
 
         #: ArcGIS API for Python loves throwing bog-standard Exceptions, so we can't narrow this down further
         except Exception as error:
-            if tries <= max_tries:  #pylint: disable=no-else-return
+            if tries <= max_tries:  # pylint: disable=no-else-return
                 wait_time = delay**tries
                 module_logger.debug(
                     'Exception "%s" thrown on "%s". Retrying after %s seconds...', error, worker_method, wait_time
                 )
                 sleep(wait_time)
                 tries += 1
                 return _inner_retry(worker_method, *args, **kwargs)
@@ -81,16 +81,16 @@
 
     Returns:
         Dict: Mapping {'original name': 'cleaned_name'}
     """
 
     rename_dict = {}
     for column in columns:
-        no_specials = re.sub(r'[^a-zA-Z0-9_]', '_', column)
-        match = re.match(r'(^[0-9_]+)', no_specials)
+        no_specials = re.sub(r"[^a-zA-Z0-9_]", "_", column)
+        match = re.match(r"(^[0-9_]+)", no_specials)
         if match:
             number = match.groups()[0]
             rename_dict[column] = no_specials.removeprefix(number) + number
             continue
         rename_dict[column] = no_specials
     return rename_dict
 
@@ -103,30 +103,30 @@
         featurelayer (arcgis.features.FeatureLayer): Live data
         new_dataframe (pd.DataFrame): New data
 
     Raises:
         RuntimeError: If new data contains a field not present in the live data
     """
 
-    live_fields = {field['name'] for field in featurelayer.properties.fields}
+    live_fields = {field["name"] for field in featurelayer.properties.fields}
     new_fields = set(new_dataframe.columns)
     #: Remove SHAPE field from set (live "featurelayer.properties['fields']" does not expose the 'SHAPE' field)
     try:
-        new_fields.remove('SHAPE')
+        new_fields.remove("SHAPE")
     except KeyError:
         pass
     new_dif = new_fields - live_fields
     live_dif = live_fields - new_fields
     if new_dif:
         raise RuntimeError(
-            f'New dataset contains the following fields that are not present in the live dataset: {new_dif}'
+            f"New dataset contains the following fields that are not present in the live dataset: {new_dif}"
         )
     if live_dif:
         module_logger.warning(
-            'New dataset does not contain the following fields that are present in the live dataset: %s', live_dif
+            "New dataset does not contain the following fields that are present in the live dataset: %s", live_dif
         )
 
 
 #: Unused?
 def check_index_column_in_feature_layer(featurelayer, index_column):
     """Ensure index_column is present for any future operations
 
@@ -134,17 +134,17 @@
         featurelayer (arcgis.features.FeatureLayer): The live feature layer
         index_column (str): The index column meant to link new and live data
 
     Raises:
         RuntimeError: If index_column is not in featurelayer's fields
     """
 
-    featurelayer_fields = [field['name'] for field in featurelayer.properties.fields]
+    featurelayer_fields = [field["name"] for field in featurelayer.properties.fields]
     if index_column not in featurelayer_fields:
-        raise RuntimeError(f'Index column {index_column} not found in feature layer fields {featurelayer_fields}')
+        raise RuntimeError(f"Index column {index_column} not found in feature layer fields {featurelayer_fields}")
 
 
 #: unused?
 def rename_fields(dataframe, field_mapping):
     """Rename fields based on field_mapping
 
     Args:
@@ -156,15 +156,15 @@
 
     Returns:
         pd.DataFrame: Dataframe with renamed fields
     """
 
     for original_name in field_mapping.keys():
         if original_name not in dataframe.columns:
-            raise ValueError(f'Field {original_name} not found in dataframe.')
+            raise ValueError(f"Field {original_name} not found in dataframe.")
 
     renamed_df = dataframe.rename(columns=field_mapping)
 
     return renamed_df
 
 
 #: This isn't used anymore... but it feels like a shame to lose it.
@@ -192,26 +192,25 @@
         featurelayer (arcgis.features.FeatureLayer): The target feature layer
         field_name (str): The AGOL-valid field name to check
 
     Raises:
         RuntimeError: If the field is not unique (or if it's indexed but not unique)
     """
 
-    fields = [field['fields'] for field in featurelayer.properties.indexes]
+    fields = [field["fields"] for field in featurelayer.properties.indexes]
     if field_name not in fields:
         raise RuntimeError(f'{field_name} does not have a "unique constraint" set within the feature layer')
     for field in featurelayer.properties.indexes:
-        if field['fields'] == field_name:
-            if not field['isUnique']:
+        if field["fields"] == field_name:
+            if not field["isUnique"]:
                 raise RuntimeError(f'{field_name} does not have a "unique constraint" set within the feature layer')
 
 
 class Geocoding:
-    """Methods for geocoding an address
-    """
+    """Methods for geocoding an address"""
 
     @staticmethod
     def geocode_addr(street, zone, api_key, rate_limits, **api_args):
         """Geocode an address through the UGRC Web API geocoder
 
         Invalid results are returned with an x,y of 0,0, a score of 0.0, and a match address of 'No Match'
 
@@ -225,28 +224,28 @@
                 added to this dict.
 
         Returns:
             tuple[int]: The match's x coordinate, y coordinate, score, and match address
         """
 
         sleep(random.uniform(rate_limits[0], rate_limits[1]))
-        url = f'https://api.mapserv.utah.gov/api/v1/geocode/{street}/{zone}'
-        api_args['apiKey'] = api_key
+        url = f"https://api.mapserv.utah.gov/api/v1/geocode/{street}/{zone}"
+        api_args["apiKey"] = api_key
 
         try:
             geocode_result_dict = retry(Geocoding._geocode_api_call, url, api_args)
         except Exception as error:
             module_logger.error(error)
-            return (0, 0, 0., 'No API response')
+            return (0, 0, 0.0, "No API response")
 
         return (
-            geocode_result_dict['location']['x'],
-            geocode_result_dict['location']['y'],
-            geocode_result_dict['score'],
-            geocode_result_dict['matchAddress'],
+            geocode_result_dict["location"]["x"],
+            geocode_result_dict["location"]["y"],
+            geocode_result_dict["score"],
+            geocode_result_dict["matchAddress"],
         )
 
     @staticmethod
     def _geocode_api_call(url, api_args):
         """Makes a requests.get call to the geocoding API.
 
         Meant to be called through a retry wrapper so that the RuntimeErrors get tried again a couple times before
@@ -264,60 +263,57 @@
             dict: The 'results' dictionary of the response json (location, score, and matchAddress)
         """
 
         response = requests.get(url, params=api_args)
 
         #: The server times out and doesn't respond
         if response is None:
-            module_logger.debug('GET call did not return a response')
-            raise RuntimeError('No response from GET; request timeout?')
+            module_logger.debug("GET call did not return a response")
+            raise RuntimeError("No response from GET; request timeout?")
 
         #: The point does geocode
         if response.status_code == 200:
-            return response.json()['result']
+            return response.json()["result"]
 
         #: The point doesn't geocode
         if response.status_code == 404:
             return {
-                'location': {
-                    'x': 0,
-                    'y': 0
-                },
-                'score': 0.,
-                'matchAddress': 'No Match',
+                "location": {"x": 0, "y": 0},
+                "score": 0.0,
+                "matchAddress": "No Match",
             }
 
         #: If we haven't returned, raise an error to trigger _retry
-        raise RuntimeError(f'Did not receive a valid geocoding response; status code: {response.status_code}')
+        raise RuntimeError(f"Did not receive a valid geocoding response; status code: {response.status_code}")
 
     @staticmethod
     def validate_api_key(api_key):
         """Check to see if a Web API key is valid by geocoding a single, known address point
 
         Args:
             api_key (str): API Key
 
         Raises:
             RuntimeError: If there was a network or other error attempting to geocode the known point
             ValueError: If the API responds with an invalid key message
             UserWarning: If the API responds with some other abnormal result
         """
 
-        url = 'https://api.mapserv.utah.gov/api/v1/geocode/326 east south temple street/slc'
+        url = "https://api.mapserv.utah.gov/api/v1/geocode/326 east south temple street/slc"
 
         try:
-            response = retry(requests.get, url=url, params={'apiKey': api_key})
+            response = retry(requests.get, url=url, params={"apiKey": api_key})
         except Exception as error:
             raise RuntimeError(
-                'Could not determine key validity; check your API key and/or network connection'
+                "Could not determine key validity; check your API key and/or network connection"
             ) from error
         response_json = response.json()
-        if response_json['status'] == 200:
+        if response_json["status"] == 200:
             return
-        if response_json['status'] == 400 and 'Invalid API key' in response_json['message']:
+        if response_json["status"] == 400 and "Invalid API key" in response_json["message"]:
             raise ValueError(f'API key validation failed: {response_json["message"]}')
 
         warnings.warn(f'Unhandled API key validation response {response_json["status"]}: {response_json["message"]}')
 
 
 def calc_modulus_for_reporting_interval(n, split_value=500):
     """Calculate a number that can be used as a modulus for splitting n up into 10 or 20 intervals, depending on
@@ -361,36 +357,36 @@
         pygsheets.Client: Authorized pygsheets client
     """
 
     try:
         return pygsheets.authorize(service_file=credentials)
     except (FileNotFoundError, TypeError) as err:
         module_logger.debug(err)
-        module_logger.debug('Credentials file not found, trying as environment variable')
+        module_logger.debug("Credentials file not found, trying as environment variable")
     try:
         return pygsheets.authorize(custom_credentials=credentials)
     except Exception as err:
-        raise RuntimeError('Could not authenticate to Google API') from err
+        raise RuntimeError("Could not authenticate to Google API") from err
 
 
 def sedf_to_gdf(dataframe):
     """Convert an Esri Spatially Enabled DataFrame to a GeoPandas GeoDataFrame
 
     Args:
         dataframe (pd.DataFrame.spatial): Esri spatially enabled dataframe to convert
 
     Returns:
         GeoPandas.DataFrame: dataframe converted to GeoDataFrame
     """
 
     gdf = gpd.GeoDataFrame(dataframe, geometry=dataframe.spatial.name)
     try:
-        gdf.set_crs(dataframe.spatial.sr['latestWkid'], inplace=True)
+        gdf.set_crs(dataframe.spatial.sr["latestWkid"], inplace=True)
     except KeyError:
-        gdf.set_crs(dataframe.spatial.sr['wkid'], inplace=True)
+        gdf.set_crs(dataframe.spatial.sr["wkid"], inplace=True)
 
     return gdf
 
 
 def save_feature_layer_to_gdb(feature_layer, directory):
     """Save a feature_layer to a gdb for safety as backup.gdb/{layer name}_{todays date}
 
@@ -398,30 +394,30 @@
         feature_layer (arcgis.features.FeatureLayer): The FeatureLayer object to save to disk.
         directory (str or Path): The directory to save the data to.
 
     Returns:
         Path: The full path to the output file, named with the layer name and today's date.
     """
 
-    module_logger.debug('Downloading existing data...')
+    module_logger.debug("Downloading existing data...")
     dataframe = feature_layer.query().sdf
 
     if dataframe.empty:
-        return f'No data to save in feature layer {feature_layer.properties.name}'
+        return f"No data to save in feature layer {feature_layer.properties.name}"
 
     gdf = sedf_to_gdf(dataframe)
 
-    out_path = Path(directory, 'backup.gdb')
+    out_path = Path(directory, "backup.gdb")
     out_layer = f'{feature_layer.properties.name}_{datetime.date.today().strftime("%Y_%m_%d")}'
-    module_logger.debug('Saving existing data to %s', out_path)
+    module_logger.debug("Saving existing data to %s", out_path)
     try:
-        gdf.to_file(out_path, layer=out_layer, engine='pyogrio', driver='OpenFileGDB')
+        gdf.to_file(out_path, layer=out_layer, engine="pyogrio", driver="OpenFileGDB")
     except pyogrio.errors.DataSourceError as error:
         raise ValueError(
-            f'Error writing {out_layer} to {out_path}. Verify {Path(directory)} exists and is writable.'
+            f"Error writing {out_layer} to {out_path}. Verify {Path(directory)} exists and is writable."
         ) from error
 
     return out_path
 
 
 class FieldChecker:
     """Check the fields of a new dataframe against live data. Each method will raise errors if its checks fail.
@@ -474,109 +470,111 @@
             ValueError: If the field types or spatial types are incompatible, the new data has multiple geometry types,
                 or the new data is not a valid spatially-enabled dataframe.
             NotImplementedError: If the live data has a field that has not yet been mapped to a pandas dtype.
         """
 
         #: Converting dtypes to str and comparing seems to be the only way to break out into shorts and longs, singles
         #: and doubles. Otherwise, checking subclass is probably more pythonic.
-        short_ints = ['uint8', 'uint16', 'int8', 'int16']
-        long_ints = ['int', 'uint32', 'uint64', 'int32', 'int64']
+        short_ints = ["uint8", "uint16", "int8", "int16"]
+        long_ints = ["int", "uint32", "uint64", "int32", "int64"]
 
         #: Leaving the commented types here for future implementation if necessary
         esri_to_pandas_types_mapping = {
-            'esriFieldTypeInteger': ['int'] + short_ints + long_ints,
-            'esriFieldTypeSmallInteger': short_ints,
-            'esriFieldTypeDouble': ['float', 'float32', 'float64'],
-            'esriFieldTypeSingle': ['float32'],
-            'esriFieldTypeString': ['str', 'object', 'string'],
-            'esriFieldTypeDate': ['datetime64[ns]'],
-            'esriFieldTypeGeometry': ['geometry'],
-            'esriFieldTypeOID': ['int'] + short_ints + long_ints,
+            "esriFieldTypeInteger": ["int"] + short_ints + long_ints,
+            "esriFieldTypeSmallInteger": short_ints,
+            "esriFieldTypeDouble": ["float", "float32", "float64"],
+            "esriFieldTypeSingle": ["float32"],
+            "esriFieldTypeString": ["str", "object", "string"],
+            "esriFieldTypeDate": ["datetime64[ns]"],
+            "esriFieldTypeGeometry": ["geometry"],
+            "esriFieldTypeOID": ["int"] + short_ints + long_ints,
             #  'esriFieldTypeBlob': [],
-            'esriFieldTypeGlobalID': ['str', 'object', 'string'],
+            "esriFieldTypeGlobalID": ["str", "object", "string"],
             #  'esriFieldTypeRaster': [],
-            'esriFieldTypeGUID': ['str', 'object', 'string'],
+            "esriFieldTypeGUID": ["str", "object", "string"],
             #  'esriFieldTypeXML': [],
         }
 
         #: geometry checking gets its own function
-        if 'SHAPE' in fields:
+        if "SHAPE" in fields:
             self._check_geometry_types()
-            fields.remove('SHAPE')
+            fields.remove("SHAPE")
 
-        fields_to_check = self.fields_dataframe[self.fields_dataframe['name'].isin(fields)].set_index('name')
+        fields_to_check = self.fields_dataframe[self.fields_dataframe["name"].isin(fields)].set_index("name")
 
         invalid_fields = []
         int_fields_as_floats = []
         datetime_fields_with_timezone = []
         for field in fields:
             #: check against the str.lower to catch normal dtypes (int64) and the new, pd.NA-aware dtypes (Int64)
             new_dtype = str(self.new_dataframe[field].dtype).lower()
-            live_type = fields_to_check.loc[field, 'type']
+            live_type = fields_to_check.loc[field, "type"]
 
             try:
                 if new_dtype not in esri_to_pandas_types_mapping[live_type]:
                     invalid_fields.append((field, live_type, str(self.new_dataframe[field].dtype)))
-                if new_dtype in ['float', 'float32', 'float64'
-                                ] and live_type in ['esriFieldTypeInteger', 'esriFieldTypeSmallInteger']:
+                if new_dtype in ["float", "float32", "float64"] and live_type in [
+                    "esriFieldTypeInteger",
+                    "esriFieldTypeSmallInteger",
+                ]:
                     int_fields_as_floats.append(field)
-                if 'datetime64' in new_dtype and new_dtype != 'datetime64[ns]' and live_type == 'esriFieldTypeDate':
+                if "datetime64" in new_dtype and new_dtype != "datetime64[ns]" and live_type == "esriFieldTypeDate":
                     datetime_fields_with_timezone.append(field)
             except KeyError:
                 # pylint: disable-next=raise-missing-from
                 raise NotImplementedError(f'Live field "{field}" type "{live_type}" not yet mapped to a pandas dtype')
 
         if invalid_fields:
             if int_fields_as_floats:
                 raise IntFieldAsFloatError(
-                    f'Field type incompatibilities (field, live type, new type): {invalid_fields}\n' \
-                    'Check the following int fields for null/np.nan values and convert to panda\'s nullable int '\
+                    f"Field type incompatibilities (field, live type, new type): {invalid_fields}\n"
+                    "Check the following int fields for null/np.nan values and convert to panda's nullable int "
                     f'dtype: {", ".join(int_fields_as_floats)}'
                 )
             if datetime_fields_with_timezone:
                 raise TimezoneAwareDatetimeError(
-                    f'Field type incompatibilities (field, live type, new type): {invalid_fields}\n' \
-                    'Check the following datetime fields for timezone aware dtypes values and convert to '\
-                    'timezone-naive dtypes using pd.to_datetime(df[\'field\']).dt.tz_localize(None): '\
+                    f"Field type incompatibilities (field, live type, new type): {invalid_fields}\n"
+                    "Check the following datetime fields for timezone aware dtypes values and convert to "
+                    "timezone-naive dtypes using pd.to_datetime(df['field']).dt.tz_localize(None): "
                     f'{", ".join(datetime_fields_with_timezone)}'
                 )
-            raise ValueError(f'Field type incompatibilities (field, live type, new type): {invalid_fields}')
+            raise ValueError(f"Field type incompatibilities (field, live type, new type): {invalid_fields}")
 
     def _check_geometry_types(self):
         """Raise an error if the live and new data geometry types are incompatible.
 
         Args:
             live_data_properties (dict): FeatureLayer.properties of live data
             new_dataframe (pd.DataFrame): New data to be added/updated
 
         Raises:
             ValueError: If the new data is not a valid spatially-enabled dataframe, has multiple geometry types, or has
                 a geometry type that doesn't match the live data.
         """
 
         esri_to_sedf_geometry_mapping = {
-            'esriGeometryPoint': 'point',
-            'esriGeometryMultipoint': 'multipoint',
-            'esriGeometryPolyline': 'polyline',
-            'esriGeometryPolygon': 'polygon',
-            'esriGeometryEnvelope': 'envelope',
+            "esriGeometryPoint": "point",
+            "esriGeometryMultipoint": "multipoint",
+            "esriGeometryPolyline": "polyline",
+            "esriGeometryPolygon": "polygon",
+            "esriGeometryEnvelope": "envelope",
         }
 
-        if 'SHAPE' not in self.new_dataframe.columns:
-            raise ValueError('New dataframe does not have a SHAPE column')
+        if "SHAPE" not in self.new_dataframe.columns:
+            raise ValueError("New dataframe does not have a SHAPE column")
 
-        if self.new_dataframe['SHAPE'].isna().any():
+        if self.new_dataframe["SHAPE"].isna().any():
             raise ValueError(
                 f'New dataframe has missing geometries at index {list(self.new_dataframe[self.new_dataframe["SHAPE"].isna()].index)}'
             )
 
         live_geometry_type = self.live_data_properties.geometryType
         new_geometry_types = self.new_dataframe.spatial.geometry_type
         if len(new_geometry_types) > 1:
-            raise ValueError('New dataframe has multiple geometry types')
+            raise ValueError("New dataframe has multiple geometry types")
         if esri_to_sedf_geometry_mapping[live_geometry_type] != new_geometry_types[0].lower():
             raise ValueError(
                 f'New dataframe geometry type "{new_geometry_types[0]}" incompatible with live geometry type "{live_geometry_type}"'
             )
 
     def check_for_non_null_fields(self, fields):
         """Raise an error if the new data contains nulls in a field that the live data says is not nullable.
@@ -591,16 +589,16 @@
             ValueError: If the new data contains nulls in a field that the live data says is not nullable and doesn't
                 have a default value.
         """
 
         columns_with_nulls = self.new_dataframe.columns[self.new_dataframe.isna().any()].tolist()
         # fields_dataframe = pd.DataFrame(self.live_data_properties['fields'])
         non_nullable_live_columns = self.fields_dataframe[
-            ~(self.fields_dataframe['nullable']) &
-            ~(self.fields_dataframe['defaultValue'].astype(bool))]['name'].tolist()
+            ~(self.fields_dataframe["nullable"]) & ~(self.fields_dataframe["defaultValue"].astype(bool))
+        ]["name"].tolist()
 
         columns_to_check = [column for column in columns_with_nulls if column in fields]
 
         #: If none of the columns have nulls, we don't need to check further
         if not columns_to_check:
             return
 
@@ -621,62 +619,63 @@
             fields (List[str]): Fields to check
 
         Raises:
             ValueError: If the string fields in the new data contain a value longer than the corresponding field in the
                 live data allows.
         """
 
-        if 'length' not in self.fields_dataframe.columns:
-            module_logger.debug('No fields with length property')
+        if "length" not in self.fields_dataframe.columns:
+            module_logger.debug("No fields with length property")
             return
 
         length_limited_fields = self.fields_dataframe[
-            (self.fields_dataframe['type'].isin(['esriFieldTypeString', 'esriFieldTypeGlobalID'])) &
-            (self.fields_dataframe['length'].astype(bool))]
+            (self.fields_dataframe["type"].isin(["esriFieldTypeString", "esriFieldTypeGlobalID"]))
+            & (self.fields_dataframe["length"].astype(bool))
+        ]
 
-        columns_to_check = length_limited_fields[length_limited_fields['name'].isin(fields)]
+        columns_to_check = length_limited_fields[length_limited_fields["name"].isin(fields)]
 
-        for field, live_max_length in columns_to_check[['name', 'length']].to_records(index=False):
+        for field, live_max_length in columns_to_check[["name", "length"]].to_records(index=False):
             new_data_lengths = self.new_dataframe[field].str.len()
             new_max_length = new_data_lengths.max()
             if new_max_length > live_max_length:
                 raise ValueError(
-                    f'Row {new_data_lengths.argmax()}, column {field} in new data exceeds the live data max length of {live_max_length}'
+                    f"Row {new_data_lengths.argmax()}, column {field} in new data exceeds the live data max length of {live_max_length}"
                 )
 
     def check_fields_present(self, fields, add_oid):
         """Raise an error if the fields to be operated on aren't present in either the live or new data.
 
         Args:
             fields (List[str]): The fields to be operated on.
             add_oid (bool): Add OBJECTID to fields if its not already present (for operations that are dependent on
                 OBJECTID, such as upsert)
 
         Raises:
             RuntimeError: If any of fields are not in live or new data.
         """
 
-        live_fields = set(self.fields_dataframe['name'])
+        live_fields = set(self.fields_dataframe["name"])
         new_fields = set(self.new_dataframe.columns)
         working_fields = set(fields)
-        working_fields.discard('SHAPE')  #: The fields from the feature layer properties don't include the SHAPE field.
+        working_fields.discard("SHAPE")  #: The fields from the feature layer properties don't include the SHAPE field.
         if add_oid:
-            working_fields.add('OBJECTID')
+            working_fields.add("OBJECTID")
 
         live_dif = working_fields - live_fields
         new_dif = working_fields - new_fields
 
         error_message = []
         if live_dif:
             error_message.append(f'Fields missing in live data: {", ".join(live_dif)}')
         if new_dif:
             error_message.append(f'Fields missing in new data: {", ".join(new_dif)}')
 
         if error_message:
-            raise RuntimeError('. '.join(error_message))
+            raise RuntimeError(". ".join(error_message))
 
     def check_srs_wgs84(self):
         """Raise an error if the new spatial reference system isn't WGS84 as required by geojson.
 
         Raises:
             ValueError: If the new SRS value can't be cast to an int (please log an issue if this occurs)
             ValueError: If the new SRS value isn't 4326.
@@ -688,44 +687,44 @@
             new_srs = self.new_dataframe.spatial.sr.wkid
         except AttributeError:
             new_srs = self.new_dataframe.spatial.sr[0]
 
         try:
             new_srs = int(new_srs)
         except ValueError as error:
-            raise ValueError('Could not cast new SRS to int') from error
+            raise ValueError("Could not cast new SRS to int") from error
         if new_srs != 4326:
             raise ValueError(
-                f'New dataframe SRS {new_srs} is not wkid 4326. Reproject with appropriate transformation.'
+                f"New dataframe SRS {new_srs} is not wkid 4326. Reproject with appropriate transformation."
             )
 
     def check_nullable_ints_shapely(self):
         """Raise a warning if null values occur within nullable integer fields of the dataframe
 
         Apparently due to a convention within shapely, any null values in an integer field are converted to 0.
 
         Raises:
             UserWarning: If we're using shapely instead of arcpy, the new dataframe uses nullable int dtypes, and there
                 is one or more pd.NA values within a nullable int column.
         """
 
         #: Only occurs if client is using shapely instead of arcpy
-        if importlib.util.find_spec('arcpy'):
+        if importlib.util.find_spec("arcpy"):
             return
 
-        nullable_ints = {'Int8', 'Int16', 'Int32', 'Int64', 'UInt8', 'UInt16', 'UInt32', 'UInt64'}
+        nullable_ints = {"Int8", "Int16", "Int32", "Int64", "UInt8", "UInt16", "UInt32", "UInt64"}
         nullable_int_columns = [
             column for column in self.new_dataframe.columns if str(self.new_dataframe[column].dtype) in nullable_ints
         ]
         columns_with_nulls = [column for column in nullable_int_columns if self.new_dataframe[column].isnull().any()]
 
         if columns_with_nulls:
             warnings.warn(
-                'The following columns have null values that will be replaced by 0 due to shapely conventions: '\
-                    f'{", ".join(columns_with_nulls)}'
+                "The following columns have null values that will be replaced by 0 due to shapely conventions: "
+                f'{", ".join(columns_with_nulls)}'
             )
 
 
 def get_null_geometries(feature_layer_properties):
     """Generate placeholder geometries near 0, 0 with type based on provided feature layer properties dictionary.
 
     Args:
@@ -744,39 +743,32 @@
     #     'esriGeometryPolyline': 'polyline',
     #     'esriGeometryPolygon': 'polygon',
     #     'esriGeometryEnvelope': 'envelope',
     # }
 
     live_geometry_type = feature_layer_properties.geometryType
 
-    if live_geometry_type == 'esriGeometryPoint':
-        return arcgis.geometry.Point({'x': 0, 'y': 0, 'spatialReference': {'wkid': 4326}}).JSON
+    if live_geometry_type == "esriGeometryPoint":
+        return arcgis.geometry.Point({"x": 0, "y": 0, "spatialReference": {"wkid": 4326}}).JSON
 
-    if live_geometry_type == 'esriGeometryPolyline':
-        return arcgis.geometry.Polyline({
-            'paths': [[[0, 0], [.1, .1], [.2, .2]]],
-            'spatialReference': {
-                'wkid': 4326
-            }
-        }).JSON
+    if live_geometry_type == "esriGeometryPolyline":
+        return arcgis.geometry.Polyline(
+            {"paths": [[[0, 0], [0.1, 0.1], [0.2, 0.2]]], "spatialReference": {"wkid": 4326}}
+        ).JSON
+
+    if live_geometry_type == "esriGeometryPolygon":
+        return arcgis.geometry.Polygon(
+            {"rings": [[[0, 0.1], [0.1, 0.1], [0.1, 0], [0, 0]]], "spatialReference": {"wkid": 4326}}
+        ).JSON
 
-    if live_geometry_type == 'esriGeometryPolygon':
-        return arcgis.geometry.Polygon({
-            'rings': [[[0, .1], [.1, .1], [.1, 0], [0, 0]]],
-            'spatialReference': {
-                'wkid': 4326
-            }
-        }).JSON
-
-    raise NotImplementedError(f'Null value generator for live geometry type {live_geometry_type} not yet implemented')
+    raise NotImplementedError(f"Null value generator for live geometry type {live_geometry_type} not yet implemented")
 
 
 class DeleteUtils:
-    """Verify Object IDs used for delete operations
-    """
+    """Verify Object IDs used for delete operations"""
 
     @staticmethod
     def check_delete_oids_are_ints(oid_list):
         """Raise an error if a list of strings can't be parsed as ints
 
         Args:
             oid_list (list[int]): List of Object IDs to delete
@@ -792,15 +784,15 @@
         bad_oids = []
         for oid in oid_list:
             try:
                 numeric_oids.append(int(oid))
             except ValueError:
                 bad_oids.append(oid)
         if bad_oids:
-            raise TypeError(f'Couldn\'t convert OBJECTID(s) `{bad_oids}` to integer')
+            raise TypeError(f"Couldn't convert OBJECTID(s) `{bad_oids}` to integer")
         return numeric_oids
 
     @staticmethod
     def check_for_empty_oid_list(oid_list, numeric_oids):
         """Raise an error if the parsed Object ID list is empty
 
         Args:
@@ -808,15 +800,15 @@
             numeric_oids (list[int]): The cast-to-int Object IDs
 
         Raises:
             ValueError: If numeric_oids is empty
         """
 
         if not numeric_oids:
-            raise ValueError(f'No OBJECTIDs found in {oid_list}')
+            raise ValueError(f"No OBJECTIDs found in {oid_list}")
 
     @staticmethod
     def check_delete_oids_are_in_live_data(oid_string, numeric_oids, feature_layer):
         """Warn if a delete Object ID doesn't exist in the live data, return number missing
 
         Args:
             oid_string (str): Comma-separated string of delete Object IDs
@@ -827,26 +819,25 @@
             UserWarning: If any of the Object IDs in numeric_oids don't exist in the live data.
 
         Returns:
             int: Number of Object IDs missing from live data
         """
 
         query_results = feature_layer.query(object_ids=oid_string, return_ids_only=True)
-        query_oids = query_results['objectIds']
+        query_oids = query_results["objectIds"]
         oids_not_in_layer = set(numeric_oids) - set(query_oids)
 
         if oids_not_in_layer:
-            warnings.warn(f'OBJECTIDs {oids_not_in_layer} were not found in the live data')
+            warnings.warn(f"OBJECTIDs {oids_not_in_layer} were not found in the live data")
 
         return len(oids_not_in_layer)
 
 
 class Chunking:
-    """Divide a dataframe into chunks to satisfy upload size requirements for append operation.
-    """
+    """Divide a dataframe into chunks to satisfy upload size requirements for append operation."""
 
     @staticmethod
     def _ceildiv(num, denom):
         """Perform ceiling division: 5/4 = 2
 
         Args:
             num (int or float): Numerator
@@ -877,15 +868,15 @@
             list[pd.DataFrame]: A list of dataframes with at most chunk_size rows per dataframe
         """
 
         df_length = len(dataframe)
 
         if df_length == 1:
             raise ValueError(
-                f'Dataframe chunk is only one row (index {dataframe.index[0]}), further chunking impossible'
+                f"Dataframe chunk is only one row (index {dataframe.index[0]}), further chunking impossible"
             )
 
         starts = range(0, df_length, chunk_size)
         ends = [start + chunk_size if start + chunk_size < df_length else df_length for start in starts]
         list_of_dataframes = [dataframe.iloc[start:end] for start, end in zip(starts, ends)]
 
         return list_of_dataframes
@@ -904,16 +895,16 @@
             max_bytes (int, optional): Maximum size in bytes any one geojson string can be. Defaults to 100000000 (AGOL
                 text uploads are limited to 100 MB?)
 
         Returns:
             list[str]: A list of the dataframe chunks converted to geojson
         """
 
-        geojson_size = sys.getsizeof(dataframe.spatial.to_featureset().to_geojson.encode('utf-16'))
-        module_logger.debug('Initial file size: %s', geojson_size)
+        geojson_size = sys.getsizeof(dataframe.spatial.to_featureset().to_geojson.encode("utf-16"))
+        module_logger.debug("Initial file size: %s", geojson_size)
 
         chunked_dataframes = Chunking._recursive_dataframe_chunking(dataframe, max_bytes)
 
         chunked_geojsons = [
             fix_numeric_empty_strings(chunk.spatial.to_featureset(), feature_layer_fields).to_geojson
             for chunk in chunked_dataframes
         ]
@@ -939,24 +930,24 @@
 
         Args:
             dataframe (pd.DataFrame.spatial): A spatially-enabled dataframe to divide
             max_bytes (int): The max utf-16 encoded geojson size for any one chunk
         """
 
         #: Calculate number of chunks needed and the guesstimate max number of rows to achieve that size
-        geojson_size = sys.getsizeof(dataframe.spatial.to_featureset().to_geojson.encode('utf-16'))
+        geojson_size = sys.getsizeof(dataframe.spatial.to_featureset().to_geojson.encode("utf-16"))
         chunks_needed = Chunking._ceildiv(geojson_size, max_bytes)
         max_rows = Chunking._ceildiv(len(dataframe), chunks_needed)
 
         #: Chunk the dataframe and then check if the resulting chunks are now within the proper size, calling again on
         #: the offending chunks if not
         list_of_dataframes = Chunking._chunk_dataframe(dataframe, max_rows)
         return_dataframes = []  #: Holds result of valid and recursive chunks
         for chunk_dataframe in list_of_dataframes:
-            chunk_geojson_size = sys.getsizeof(chunk_dataframe.spatial.to_featureset().to_geojson.encode('utf-16'))
+            chunk_geojson_size = sys.getsizeof(chunk_dataframe.spatial.to_featureset().to_geojson.encode("utf-16"))
             if chunk_geojson_size > max_bytes:
                 return_dataframes.extend(Chunking._recursive_dataframe_chunking(chunk_dataframe, max_bytes))
             else:
                 return_dataframes.append(chunk_dataframe)
 
         return return_dataframes
 
@@ -965,23 +956,23 @@
     """Replace empty strings with None for numeric fields that allow nulls
     Args:
         feature_set (arcgis.features.FeatureSet): Feature set to clean
         fields (Dict): fields from feature layer
     """
 
     fields_to_fix = {
-        field['name']
+        field["name"]
         for field in feature_layer_fields
-        if field['type'] in ['esriFieldTypeDouble', 'esriFieldTypeInteger', 'esriFieldTypeDate'] and field['nullable']
+        if field["type"] in ["esriFieldTypeDouble", "esriFieldTypeInteger", "esriFieldTypeDate"] and field["nullable"]
     }
-    fields_to_fix -= {'Shape__Length', 'Shape__Area'}
+    fields_to_fix -= {"Shape__Length", "Shape__Area"}
 
     for feature in feature_set.features:
         for field_name in fields_to_fix:
-            if feature.attributes[field_name] == '':
+            if feature.attributes[field_name] == "":
                 feature.attributes[field_name] = None
 
     return feature_set
 
 
 def chunker(sequence, chunk_size):
     """Break sequence into chunk_size chunks
@@ -990,8 +981,8 @@
         sequence (iterable): Any iterable sequence
         chunk_size (int): Desired number of elements in each chunk
 
     Returns:
         generator: Generator of original sequence broken into chunk_size lists
     """
 
-    return (sequence[position:position + chunk_size] for position in range(0, len(sequence), chunk_size))
+    return (sequence[position : position + chunk_size] for position in range(0, len(sequence), chunk_size))
```

### Comparing `ugrc-palletjack-4.3.0/src/ugrc_palletjack.egg-info/PKG-INFO` & `ugrc-palletjack-4.3.1/src/ugrc_palletjack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: ugrc-palletjack
-Version: 4.3.0
+Version: 4.3.1
 Summary: Updating AGOL feature services with data from external tables.
 Home-page: https://github.com/agrc/palletjack
 Author: Jake Adams, UGRC
 Author-email: jdadams@utah.gov
-License: UNKNOWN
 Project-URL: Issue Tracker, https://github.com/agrc/palletjack/issues
 Keywords: gis
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
@@ -95,9 +93,7 @@
 The github pages are served from the `gh-pages` branch. After you make edits to the code and update the docstrings, rebase this branch onto the updated `main` branch. To prevent github pages from trying to generate a site from the contents of `docs/palletjack` with jekyll, add a `.nojekyll` file to `docs/palletjack`.
 
 To generate the docs, run `pdoc --html -o docs\ c:\palletjack\repo\src\palletjack --force`. The code's docstrings should be Google-style docstrings with proper indentation to ensure the argument lists, etc are parsed and displayed correctly.
 
 `docs/README.md` is included at the top package level by adding the line `.. include:: ../../docs/README.md` in `__init__.py`'s docstring. This tells pdoc to insert that markdown into the HTML generated for that docstring, and the include directive can be used for more in-depth documentation anywhere else as well. Note that `pdoc` tries to create links for anything surrounded by backticks, which are also used for code blocks. You may need to manually edit the HTML to remove the links if they change the content of your code blocks (such as in the example import statement).
 
 Once the contents of `docs/palletjack` look correct, force push the `gh-pages` branch to github. This will trigger the action to republish the site. The docs are then accessible at [agrc.github.io/palletjack/palletjack/index.html].
-
-
```

### Comparing `ugrc-palletjack-4.3.0/src/ugrc_palletjack.egg-info/SOURCES.txt` & `ugrc-palletjack-4.3.1/src/ugrc_palletjack.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 LICENSE
 README.md
-setup.cfg
+pyproject.toml
 setup.py
 src/palletjack/__init__.py
 src/palletjack/errors.py
 src/palletjack/extract.py
 src/palletjack/load.py
 src/palletjack/transform.py
 src/palletjack/utils.py
```

